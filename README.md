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
## Tags de metadados (no `<head>`)
`<title>` : Define o título da página (aparece na aba do navegador)

`<meta>` : Fornece metadados, como charset e viewport

`<meta charset="UTF-8">` Define a codificação de caracteres

`<meta name="viewport" content="width=device-width, initial-scale=1.0">` Torna a página responsiva em dispositivos móveis

`<link>`: Vincula arquivos externos, como CSS

`<script>`: Adiciona ou referencia scripts JavaScript.

```HTML
<meta charset="UTF-8">
```

```HTML
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
    

```HTML
<link rel="stylesheet" href="estilo.css">
```

```HTML
<script src="script.js"></script>
```

## Estrutura de texto:
### Cabeçalhos:

Títulos: `<h1>` até `<h6>`

### Parágrafos: 

Parágrafo: `<p>`

### Formatos de texto:

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

```HTML
<a href="#">`Texto do link`</a>
```

Imagem: `<img src="imagem.jpg" alt="Descrição da imagem">`

```HTML
<img src="imagem.jpg" alt="Descrição da imagem">
```

## Listas:
Ordenada: `<ol type="A">`

`1` (padrão) → 1, 2, 3...

`A` → A, B, C...

`a` → a, b, c...

`I` → I, II, III...

`i` → i, ii, iii...

```HTML
<ol>
<li></li>
<li></li>
<li></li>
</ol>
```

Não ordenada: `<ul style="list-style-type: disc;">`

`disc` (padrão) → ●

`circle` → ○

`square` → ■

`none` → Remove os marcadores.

```HTML
<ul>
<li></li>
<li></li>
<li></li>
</ol>
```

Itens: `<li>`

Define a lista: `<dl>`

Define o termo: `<dt>`
    
Define a descrição do termo: `<dd>`

```HTML
<dl>
    <dt>HTML</dt>
    <dd>Linguagem de marcação para criar páginas web.</dd>

    <dt>CSS</dt>
    <dd>Linguagem para estilizar páginas web.</dd>

    <dt>JavaScript</dt>
    <dd>Linguagem de programação para tornar as páginas interativas.</dd>
</dl>

```

## Tabelas
### basico
```HTML
<table border="1">
    <tr>
        <th>Cabeçalho 1</th>
        <th>Cabeçalho 2</th>
    </tr>
    <tr>
        <td>Dado 1</td>
        <td>Dado 2</td>
    </tr>
    <tr>
        <td>Dado 4</td>
        <td>Dado 5</td>
    </tr>
</table>
```
Cria tabelas: `<table>`

Define um cabeçalho de coluna: `<th>`

Define uma linha: `<tr>`

Define uma célula: `<td>`

Adiciona um título para a tabela: `<caption>`

Define o cabeçalho da tabela: `<thead>`

Define o corpo principal da tabela: `<tbody>`

Define o rodapé da tabela: `<tfoot>`

### completo
```HTML
<table border="1">
    <caption>Relatório de Vendas</caption>
    <thead>
        <tr>
            <th>Produto</th>
            <th>Preço</th>
            <th>Quantidade</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Celular</td>
            <td>R$ 1500</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Notebook</td>
            <td>R$ 3500</td>
            <td>5</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="2">Total</td>
            <td>15</td>
        </tr>
    </tfoot>
</table>
```

Mesclar colunas: `colspan`

Mesclar linhas: `rowspan`

## Trabalhe com formulários
`<form>`: Contém elementos de formulário
    
`<input>`: Campos de entrada (texto, senha, email, etc.)
    
Tipos mais comuns: `text`, `email`, `password`, `submit`, `radio`, `checkbox`, `file`, etc
    
`<textarea>`: Área de texto para múltiplas linhas
    
`<button>`: Botão clicável
    
`<label>`: Rotula um campo do formulário
    
`<select>`: Caixa de seleção (dropdown)
    
`<option>`: Opções dentro de `<select>`
    
`<fieldset>`: Agrupa elementos do formulário
    
`<legend>`: Adiciona uma legenda para o <fieldset>

### Criação de formulários básicos:
```HTML
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

`<header>`: Cabeçalho da página ou seção
    
`<nav>`: Menu de navegação
    
`<main>`: Conteúdo principal da página
    
`<section>`: Seção de conteúdo relacionada
    
`<article>`: Conteúdo independente (ex.: post de blog)
    
`<aside>`: Conteúdo relacionado, como barras laterais
    
`<footer>`: Rodapé da página ou seção

## Elementos interativos
`<details>`: Cria uma seção de detalhes expansível
    
`<summary>`: Título visível de um <details>
    
`<dialog>`: Cria uma caixa de diálogo (popup)

## Outras tags úteis
`<div>`: Container genérico para agrupar elementos
    
`<span>`: Container inline para estilizar ou agrupar texto

`<iframe>`: Incorpora outro documento HTML dentro da página

## APIs do HTML5
### Canvas: Para criar gráficos e animações.
### Geolocation: Para obter a localização do usuário.
### Local Storage: Para armazenar dados no navegador.

















