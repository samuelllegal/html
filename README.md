# html
informações básicas de html para construir uma estrutura básica de site
Referência oficial: [https://developer.mozilla.org/pt-BR/docs/Web/HTML](MDN Web Docs (HTML)).

## Estrutura básica de uma página HTML
```HTML
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Título da Página</title>
    <link rel="stylesheet" href="estilo.css">
    <script src="script.js"></script>
</head>
<body>
    <h1>Olá, mundo!</h1>
</body>
</html>
```
## Tags de metadados (no <head>)
`<title>`: Define o título da página (aparece na aba do navegador).
`<meta>`: Fornece metadados, como charset e viewport:
    `<meta charset="UTF-8">`: Define a codificação de caracteres.
    `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Torna a página responsiva em dispositivos móveis.
`<link>`: Vincula arquivos externos, como CSS:
```HTML
<link rel="stylesheet" href="estilo.css">
```
`<script>`: Adiciona ou referencia scripts JavaScript.
```
<script src="script.js"></script>
```

## Estrutura de texto:
Cabeçalhos:
    Títulos: `<h1>` até `<h6>`
Parágrafos: 
    Parágrafo: `<p>`
Formatos de texto:
    `<strong>`: Destaca texto com importância (normalmente em negrito).
    `<em>`: Texto com ênfase (normalmente em itálico).
    `<b>`: Texto em negrito sem importância semântica.
    `<i>`: Texto em itálico sem importância semântica.
    `<mark>`: Destaca texto com fundo amarelo.
    `<u>`: Texto sublinhado.
    `<small>`: Texto menor.
    `<del>`: Texto riscado.
    `<ins>`: Texto inserido, geralmente sublinhado.
    `<br>`: Quebra de linha.
    `<hr>`: Linha horizontal.

## Links e imagens:
Link: `<a href="https://exemplo.com">`Texto do link`</a>`
Imagem: `<img src="imagem.jpg" alt="Descrição da imagem">`

## Listas:
Ordenada: `<ol>`
Não ordenada: `<ul>`
Itens: `<li>`
Lista de descrição: `<dl>`
    Título da descrição: `<dt>`
    Detalhe da descrição: `<dd>`

## Tabelas
Cria tabelas: `<table>`
Define uma linha: `<tr>`
Define um cabeçalho de coluna: `<th>`
Define uma célula: `<td>`
Adiciona um título para a tabela: `<caption>`

## Trabalhe com formulários
### Criação de formulários básicos:
```
<form action="/enviar" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
    
    <button type="submit">Enviar</button>
</form>
```
Principais elementos: `<input>`, `<textarea>`, `<button>`, `<select>`, `<option>`

## novos recursos do HTML5
### Áudio:
```
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Seu navegador não suporta o elemento de áudio.
</audio>
```
### Vídeo:
```
<video controls width="600">
    <source src="video.mp4" type="video/mp4">
    Seu navegador não suporta o elemento de vídeo.
</video>
```
## Semântica:
Use tags como `<header>`, `<footer>`, `<article>`, `<section>`, `<nav>`, `<aside>` para organizar o conteúdo.


## APIs do HTML5
### Canvas: Para criar gráficos e animações.
### Geolocation: Para obter a localização do usuário.
### Local Storage: Para armazenar dados no navegador.

















