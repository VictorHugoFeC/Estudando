# Para criar um arquivo na linguagem 
* **HTML:**
index.html
* **CSS:**
main.css
* **JavaScript:**
app.js

## Primeiro passo de HTML
```html
<!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="UTF-8">
    <title>Teste</title>
  </head>
 <body>

 </body>
</html>
```
Para vincular a um CSS coloque o "link".
```html
<link rel="stylesheet" href="main.css">
```
Agora estruturando o body, pode adicionar a estrutura do seu código usando "h1", "p", "ul" e muito mais.
```html
<!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="UTF-8">
    <title>Teste</title>
   <link rel="stylesheet" href="main.css">
  </head>
<body>
 <h1>Projeto teste</h1>
<p>Esse code serve para revisar a linguagem</p>
  <ul>
   <li>Ponto 1</li>
   <li>Ponto 2</li>
   <li>Ponto 3</li>
  </ul>  
</body>
</html>
```
## CSS Externo
### Regras de CSS
Você seleciona uma sala e define as regras de como ela deve ser.
```css
body {
 font-family: monospace;
}
ul {
 font-family: helvética;
}
```
## Seletores
Uma ID é para definir o estilo de um elemento, enquanto classes podem definir vários estilos de elementos.
```css
li {
 list-style: circle;
}
.list {
 list-style: square;
}
#msg {
 font-family: monospace;
}
```
## Adicionar um tema claro
Adicionando temas de cores claras para seu site, use código de cor hexadecimais.
```css
.light-theme {
 color: #000000;
 background: #00FF00;
}
```
No arquivo em HTML, coloque no seu body class="light-theme", para aplicar no seu código corretamente o tema claro.
```html
<body class="light-theme>
```
## Adicionar um tema escuro
Defina para o tema escuro da seguinte forma.
```css
:root {
 --green: #00FF00;
 --white: #ffffff;
 --black: #000000;
}
```
No final adicione uma cor para fonte e para tela de fundo, e var vai ser utilizado para especificar variáveis
```css
.light-theme {
  --bg: var(--green);
  --fontColor: var(--black);
}
.dark.theme {
  --bg: var(--black);
  --fontColor: var(--green);
}
```
Substitua o "body" atual no CSS

