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
Abaixo, a estrutura básica com o vínculo para o arquivo de estilos (CSS) e a organização do conteúdo no `<body>`.

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
Utilizamos Variáveis CSS (:root) para facilitar a troca de cores entre temas.
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
O JavaScript manipula o DOM para alternar as classes do corpo do site e mudar o tema em tempo real.
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




