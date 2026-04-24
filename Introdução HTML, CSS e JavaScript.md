# Resumo de Fundamentos Web: HTML, CSS & JS

Repositório dedicado ao estudo e revisão da estrutura básica de uma página web, com foco na implementação de **Temas (Claro/Escuro)**.

---

## Estrutura de Arquivos
| Linguagem | Arquivo Padrão | Função |
| :--- | :--- | :--- |
| **HTML** | `index.html` | Estrutura e conteúdo |
| **CSS** | `main.css` | Estilização e layout |
| **JavaScript** | `app.js` | Interatividade e lógica |

---

## 1. HTML: O Esqueleto
O arquivo `index.html` define a hierarquia dos elementos. Note que o script é carregado ao final do `body` para garantir que o DOM esteja pronto antes da execução da lógica.

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Projeto de Revisão</title>
    <link rel="stylesheet" href="main.css">
</head>
<body class="light-theme">
    <h1>Projeto Teste</h1>
    <p>Este código serve para revisar os fundamentos da web.</p>
    
    <ul>
        <li>Ponto 1</li>
        <li>Ponto 2</li>
        <li>Ponto 3</li>
    </ul>

    <div>
        <button class="btn">Dark</button>
    </div>

    <script src="app.js"></script>
</body>
</html>
```
## 2. CSS: Estilização e Temas
A estratégia utilizada foca no uso de Custom Properties (Variáveis CSS). Isso permite que a troca de cores ocorra apenas alternando a classe no elemento pai (body).
```Css
/* Definição de cores globais */
:root {
    --green: #00FF00;
    --white: #ffffff;
    --black: #000000;
}

/* Regras para Tema Claro */
.light-theme {
    --bg: var(--green);
    --fontColor: var(--black);
    --btnBg: var(--black);
    --btnFontColor: var(--white);
}

/* Regras para Tema Escuro */
.dark-theme {
    --bg: var(--black);
    --fontColor: var(--green);
    --btnBg: var(--white);
    --btnFontColor: var(--black);
}

/* Aplicando as variáveis */
* {
    color: var(--fontColor);
    font-family: Helvetica, sans-serif;
}

body {
    background: var(--bg);
}
```
Estilizando o Botão
```Css
.btn {
    position: absolute;
    top: 20px;
    left: 250px;
    height: 50px;
    width: 50px;
    border-radius: 50%;
    border: none;
    cursor: pointer;
    background-color: var(--btnBg);
    color: var(--btnFontColor);
}

.btn:focus { outline: none; }
```
## 3. JavaScript: Interatividade
O arquivo app.js é responsável por dar "vida" à página. Ele utiliza o DOM (Document Object Model) para observar o comportamento do usuário e reagir modificando o HTML e o CSS dinamicamente.
```JavaScripr
// Seleciona o botão pela classe
const switcher = document.querySelector('.btn');

// Escuta o evento de clique
switcher.addEventListener('click', function() {
    // Alterna entre as classes de tema
    document.body.classList.toggle('dark-theme');
    document.body.classList.toggle('light-theme');

    // Atualiza o texto do botão conforme o tema atual
    const className = document.body.className;
    if(className == "light-theme") {
        this.textContent = "Dark";
    } else {
        this.textContent = "Light";
    }

    console.log('Tema atual: ' + className);
});
```
