# 🪙 Juro Code Translator 🪙

> Uma abordagem inovadora, divertida e matematicamente robusta para criptografia de texto baseada em Álgebra Linear e Cifra de Hill!

Imagine misturar matemática de nível universitário com uma camada de ofuscação de dados totalmente personalizada e divertida. Esse é o **Juro Code Translator**, um codificador e decodificador digital executado 100% no navegador.

🔗 **[Experimente o Juro Code Translator Ao Vivo Agora!](https://aceleradox.github.io/text-to-code-/juro_code.html)**

---

## 🚀 O que é o Juro Code?

O **Juro Code** não é apenas um conversor de texto simples. Ele utiliza o conceito real de **Cifra de Hill (Hill Cipher)** para transformar strings de texto comuns em vetores numéricos, multiplicá-los por matrizes inversíveis e gerar uma saída totalmente ofuscada através de tokens e hexadecimais únicos.

O resultado é uma ferramenta rápida, responsiva e com uma interface limpa que permite enviar mensagens secretas que só quem tem o algoritmo consegue decifrar!

---

## 🧠 Como Funciona? (A Matemática por Trás)

O coração do projeto bate no ritmo da **Álgebra Linear**. O processo de criptografia e decriptografia segue regras matemáticas exatas:

1. **Vetorização**: O texto inserido é transformado em seus valores numéricos correspondentes (tabela ASCII/Unicode) e agrupado em pares, formando **Matrizes Coluna $2 \times 1$**.
2. **Criptografia por Multiplicação**: Cada par de caracteres passa por uma multiplicação matricial utilizando uma matriz chave estática $A$:
   $$A = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}$$
3. **Determinante Unitário**: A mágica da reversibilidade perfeita acontece porque o determinante da matriz $A$ é exatamente igual a **1** ($\det(A) = 2 \cdot 1 - 1 \cdot 1 = 1$). Isso garante que a decodificação seja exata e livre de divisões complexas ou dízimas periódicas.
4. **Decriptografia Perfeita**: Para recuperar a mensagem original, o sistema aplica a **Matriz Inversa** $A^{-1}$:
   $$A^{-1} = \begin{pmatrix} 1 & -1 \\ -1 & 2 \end{pmatrix}$$
5. **Camada de Ofuscação (Juro Tokens)**: Após o cálculo, os valores resultantes são convertidos em hexadecimal e mapeados para uma linguagem de tokens customizada, deixando o código final com um visual único e divertido.

---

## ✨ Funcionalidades Principais

* ⚡ **Criptografia em Tempo Real**: Codifique mensagens instantaneamente.
* 🔓 **Decriptografia Precisa**: Retorne ao texto original sem perda de dados.
* 🖥️ **Interface Responsiva**: Design moderno, intuitivo e adaptado para PCs e celulares.
* 🌐 **Zero Dependências**: Construído puramente com tecnologia web nativa (HTML5, CSS3 e JavaScript Vanilla).

---

## 🛠️ Tecnologias Utilizadas

O projeto foi desenvolvido focando na leveza e no desempenho do lado do cliente (*client-side*):

* **HTML5** – Estruturação semântica da aplicação.
* **CSS3** – Estilização moderna, layout responsivo e elementos visuais atraentes.
* **JavaScript (ES6+)** – Manipulação de matrizes, lógica criptográfica e controle de eventos.

---

## 🤝 Como Contribuir

Adoraria ver a comunidade expandindo o Juro Code! Se você quiser sugerir melhorias para o algoritmo, sinta-se à vontade para:

1. Fazer um **Fork** do projeto.
2. Criar uma branch para sua modificação (`git checkout -b feature/NovaMelhoria`).
3. Fazer o **Commit** de suas alterações (`git commit -m 'Adicionando mod 256 para segurança global'`).
4. Enviar um **Push** para a branch (`git push origin feature/NovaMelhoria`).
5. Abrir um **Pull Request**.

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<p align="center">Feito com 💻 e 🔢 por <a href="https://github.com">AceleradoX</a></p>
