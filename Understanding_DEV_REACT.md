# Tabela de Conteúdos

- [Git e GitHub](#github)
- [HTML](#html)
  - [Tipos de Listas](#tipos-de-listas)
  - [Imagens](#imagens)
  - [Tabelas, Vídeo, Áudio, details + summary](#tabelas)
- [CSS](#css-fundamentos)
  - [Margens, Padding, Bordas, Outline, Box Model](#css---margens-padding-bordas-outline-box-model)
  - [Formatação para Links, Listas e Tabelas](#css---formatação-para-links-listas-e-tabelas)
  - [FlexBox](#flex)
  - [Grid Layout](#grid)
  - [Responsividade](#mediaquery)
  - [Referências](#conteúdos-complementares)
  - [Bootstrap](#bootstrap)
- [JavaScript](#javascript)
  - [Condicionais](#condicionais)
  - [Estruturas de Repetição](#estruturas-de-repetição)
  - [Variáveis (var, let, const)](#variáveis-var-let-const)
  - [Métodos map, reduce, filter](#métodos-map-reduce-filter)
  - [Arrays Multidimensionais](#arrays-multidimensionais)
  - [Métodos de Numbers](#métodos-de-numbers)
  - [Processamento Assíncrono](#processamento-assincrono)
  - [Consumo de API com AJAX](#consumo-de-api-com-ajax)
  - [Consumo de API com fetch e Async/Await](#consumo-de-api-com-fetch-e-asyncawait)
  - [LocalStorage e SessionStorage](#localstorage-sessionstorage)
- [Node.js](#nodejs)
  - [Criando o Primeiro Servidor HTTP](#criando-o-primeiro-servidor-http)
  - [Express: Criando uma API com o Framework Express](#express)
  - [Express: Roteamento](#express-roteamento)
  - [Express: Rotas Dinâmicas](#express-rotas-dinâmicas)
  - [Segurança em Aplicações Web - CORS](#cors)
  - [Middlewares](#middlewares)
  - [Conceitos Básicos de API REST](#api-rest)
  - [Status Codes](#status-codes)
  - [Trabalhando com Arquivos Estáticos](#arquivos-estáticos)
  - [CommonJS Modules vs. ES6 Modules](#commonjs-es6)
  - [Segurança em Aplicações Web - Autenticação com JWT](#jwt)
  - [Construindo um CRUD](#crud)

<br>

# GIT E GITHUB <a id="github"></a>

## 1. Criar repositório no GitHub

Passo a passo: [Como Criar um repositório](https://docs.github.com/pt/get-started/quickstart/create-a-repo)

## 2. `git clone github.com/repositorio`

Crie uma cópia de trabalho em um repositório local.

## 3. `git add .` ou `git add arquivo.html`

Você pode selecionar todos ou apenas um arquivo em específico para adicionar ao commit separadamente. Este é o primeiro passo no fluxo de trabalho básico do Git. Para realmente confirmar estas mudanças (isto é, fazer um **commit**).

## 4. `git commit -m "comente sobre o commit"`

Agora o arquivo é enviado para o HEAD, mas ainda não para o repositório remoto.

## 5. `git push origin main/master`

Altere main/master para qualquer ramo (branch) desejado, enviando suas alterações para ele.

## `git pull`

Puxar alterações do repositório remoto para atualizar seu repositório local com a mais nova versão.

## `git status`

Ver o status atual do Git para saber se precisa commitar algo ou não.

### O PROCESSO É (PARA TRABALHO INDIVIDUAL)

    clone ➜ add ➜ commit ➜ push

---

# Outros comandos importantes:

## `git log`

Visualizar os pontos na linha do tempo (commits).

## `git show`

Apresentar um determinado ponto na história.

## `git branch`

Gerenciar novas linhas do tempo.
![branches](/assets/branches.png "ramificações")

## `git checkout`

Manipular as linhas do tempo.

## `git reset`

Voltar para um ponto na linha do tempo.

## `git merge`

Unir as linhas do tempo.

## `git fork`

Criar uma bifurcação de um repositório.
_Como usar:_ [Utilizando fork](https://docs.github.com/pt/github/getting-started-with-github/quickstart/fork-a-repo)

## `git stash`

Salvar trabalho no estado atual para continuar com outra tarefa, e voltar depois.
_Documentação:_ [Git Stash](https://git-scm.com/docs/git-stash)

# Fluxo de Trabalho

![fluxo de trabalho git](/assets/trees.png "Trees")

## Material complementar | Git e Github

[Playlist no YouTube - Curso Em Vídeo](https://www.youtube.com/playlist?list=PLHz_AreHm4dm7ZULPAmadvNhH6vk9oNZA)

---

<br><br>

<a id="html"></a>

# HTML - Introdução

## O que é HTML?

HTML (HyperText Markup Language) é a linguagem de marcação padrão utilizada para criar e estruturar conteúdo na web. Ele fornece uma estrutura básica para a criação de páginas da web, permitindo a inclusão de texto, imagens, links e outros elementos interativos.

## Para que serve o HTML?

HTML é usado para definir a estrutura de uma página da web. Ele determina como o conteúdo é organizado e apresentado aos visitantes. Com o uso de tags e elementos, os desenvolvedores podem criar páginas com texto formatado, imagens, links e outros elementos que constituem a experiência de navegação na web.

---

# Elementos, Tags e Atributos

## Elementos em HTML

Os elementos HTML são os blocos de construção básicos de uma página da web. Eles podem ser cabeçalhos, parágrafos, imagens, links e muitos outros tipos de conteúdo.

## Tags HTML

As tags HTML são usadas para marcar os elementos em um documento HTML. Elas geralmente consistem em um nome de tag envolto por colchetes angulares ("<" e ">"). Por exemplo, `<p>` é a tag para parágrafos, `<img>` é a tag para imagens e `<a>` é a tag para links.

## Atributos HTML

As tags HTML podem ter atributos que fornecem informações adicionais sobre o elemento. Os atributos são especificados na tag de abertura e geralmente têm um nome e um valor. Por exemplo, a tag `<img>` pode ter um atributo `src` que define a fonte da imagem.

---

# Estrutura de um arquivo HTML, Comentários e Tags de Cabeçalho

## Estrutura de um arquivo HTML

Um arquivo HTML começa com uma declaração `<!DOCTYPE>` que define a versão do HTML sendo usada. Em seguida, o documento é envolto por uma tag `<html>`, que contém as seções `<head>` e `<body>`.

## Comentários em HTML

Comentários são usados para adicionar notas ou explicações no código HTML. Eles não são exibidos na página do navegador e são escritos entre `<!--` e `-->`.

## Tags de Cabeçalho HTML

As tags de cabeçalho, que ficam na seção `<head>` do documento, fornecem informações sobre a página, como título, codificação de caracteres e links para folhas de estilo.

---

# HTML - Tags semânticas

## Tags semânticas em HTML - Resumo

As tags semânticas ajudam a estruturar o conteúdo de uma maneira significativa para os mecanismos de busca e para a acessibilidade. Algumas das tags semânticas mais comuns são:

- `<header>`: Define o cabeçalho da página ou de uma seção.
- `<main>`: Define o conteúdo principal da página.
- `<footer>`: Define o rodapé da página ou de uma seção.
- `<section>`: Define uma seção genérica.
- `<nav>`: Define um bloco de navegação.
- `<article>`: Define um conteúdo autônomo e independente.
- `<aside>`: Define um conteúdo relacionado ou auxiliar.

---

## Exemplos de Tags semânticas em HTML

`<header>`: Define o cabeçalho da página ou de uma seção. Geralmente contém logotipos, títulos e elementos de navegação.

```html
<header>
  <h1>Meu Site</h1>
  <nav>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Sobre</a></li>
    </ul>
  </nav>
</header>
```

`<main>`: Define o conteúdo principal da página. Deve conter o conteúdo central da página, excluindo cabeçalhos, rodapés e barras laterais.

```html
<main>
  <h2>Artigo Principal</h2>
  <p>Este é o conteúdo principal da página.</p>
</main>
```

`<footer>`: Define o rodapé da página ou de uma seção. Geralmente contém informações de contato, links de redes sociais e direitos autorais.

```html
<footer>
  <p>&copy; 2023 Meu Site. Todos os direitos reservados.</p>
</footer>
```

`<section>`: Define uma seção genérica da página. Pode ser usada para agrupar conteúdo relacionado.

```html
<section>
  <h3>Seção de Notícias</h3>
  <p>Confira as últimas notícias sobre tecnologia.</p>
</section>
```

`<nav>`: Define um bloco de navegação. Geralmente contém links para outras partes do site.

```html
<nav>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Produtos</a></li>
    <li><a href="#">Contato</a></li>
  </ul>
</nav>
```

`<article>`: Define um conteúdo autônomo e independente, como um post de blog, notícia ou artigo.

```html
<article>
  <h2>Novo Produto Lançado</h2>
  <p>Apresentamos o mais recente produto da nossa empresa.</p>
</article>
```

`<aside>`: Define um conteúdo relacionado ou auxiliar, como uma barra lateral de widgets.

```html
<aside>
  <h3>Artigos Relacionados</h3>
  <ul>
    <li><a href="#">Dicas de Produtividade</a></li>
    <li><a href="#">Como Usar Nossos Produtos</a></li>
  </ul>
</aside>
```

## HTML - Materiais Complementares

Existem vários materiais complementares disponíveis para aprender HTML:

- [W3Schools - HTML Tutorial](https://www.w3schools.com/html/): Um guia abrangente para aprender HTML.
- [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML): Documentação detalhada do HTML pela Mozilla.

# HTML - Elementos estruturais não semânticos

## Elementos estruturais não semânticos

Além das tags semânticas, existem elementos não semânticos que são usados para organizar e estilizar o layout da página. Dois dos elementos mais comuns são:

- `<div>`: É uma divisão genérica usada para agrupar outros elementos e aplicar estilos.
- `<span>`: É usado para aplicar estilos a uma parte específica do texto dentro de um elemento.

Esses elementos não têm um significado semântico intrínseco, mas desempenham um papel importante na criação de layouts complexos.

---

# HTML - Principais Tags

![html](/assets/1596625644452.jpeg "principais tags")

## Principais Tags do HTML

- `<h1>` a `<h6>`: Tags de título, usadas para criar cabeçalhos de diferentes níveis.
- `<p>`: Tag de parágrafo, usada para inserir texto.
- `<img>`: Tag de imagem, usada para incluir imagens.
- `<a>`: Tag de âncora, usada para criar links.
- Listas: `<ul>` (lista não ordenada), `<ol>` (lista ordenada) e `<li>` (item de lista).

Essas tags são fundamentais para estruturar o conteúdo de uma página e criar links e listas.

---

# HTML - Um Pouco sobre Formatação

## Formatação com HTML

- `<b>`: Texto em negrito.
- `<strong>`: Texto importante, enfatizado em negrito.
- `<i>`: Texto em itálico.
- `<em>`: Texto enfatizado, em itálico.
- `<big>`: Texto maior que o normal.
- `<small>`: Texto menor que o normal.
- `<del>` e `<s>`: Texto tachado, usado para indicar remoção.
- `<mark>`: Texto destacado, geralmente com uma cor de fundo.

Essas tags são usadas para aplicar formatação e ênfase ao texto, ajudando a transmitir informações visuais e semânticas aos leitores.

### Tipos de Listas

Existem diferentes tipos de listas em HTML:

- `<ul>`: Lista não ordenada. Itens são marcados com bullets.
- `<ol>`: Lista ordenada. Itens são numerados.
- `<li>`: Item de lista em uma lista `<ul>` ou `<ol>`.
- `<dl>`: Lista de definição. Cada item tem uma descrição associada.

Além disso, você pode usar a tag `<datalist>` para criar uma lista de opções úteis para formulários ou seções de dúvidas frequentes.

### Imagens

A tag `<img>` é usada para incluir imagens em uma página. Você deve especificar o atributo `src` para indicar o caminho da imagem. Por exemplo:

```html
<img src="caminho/para/imagem.jpg" alt="Descrição da imagem" />
```

O atributo alt fornece uma descrição alternativa para a imagem, o que é importante para acessibilidade e SEO.

## HTML - Indentação do Código HTML

A indentação do código HTML é uma prática recomendada para melhorar a legibilidade e a organização do seu código. Use espaços ou tabulações para alinhar elementos aninhados de forma clara.

## HTML - Tipos de Link

Existem vários tipos de links em HTML:

### Links para outras páginas:

```html
<a href="outra_pagina.html">Clique aqui</a>
```

### Links para endereços de e-mail:

```html
<a href="mailto:email@example.com">Enviar e-mail</a>
```

### Links para números de telefone:

```html
<a href="tel:+123456789">Ligar</a>
```

<a id="tabelas"> </a>

## HTML - Tabelas, Vídeo, Áudio, details + summary

Tabelas:

- Tabelas Simples

```html
<table>
  <tr>
    <th>Produto</th>
    <th>Preço</th>
  </tr>
  <tr>
    <td>Item 1</td>
    <td>R$ 10</td>
  </tr>
</table>
```

- Tabelas completas

```html
<table>
  <thead>
    <tr>
      <th>Produto</th>
      <th>Preço</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Item 1</td>
      <td>R$ 10</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Total</td>
    </tr>
  </tfoot>
</table>
```

# HTML - Formulários

Os formulários HTML permitem que os usuários insiram dados interativamente. Aqui está um exemplo básico de um formulário:

```html
<form>
  <label for="nome">Nome:</label>
  <input type="text" id="nome" name="nome" placeholder="Digite seu nome" />

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Digite seu email" />

  <input type="submit" value="Enviar" />
</form>
```

### CSS Fundamentos

#### Seletores CSS

Em CSS, os seletores são usados para aplicar estilos a elementos específicos em uma página web. Aqui estão alguns tipos comuns de seletores:

- Elemento Selector: Selecione elementos HTML diretamente. Exemplo: p { ... }

- ID Selector: Selecione um elemento pelo atributo "id". Exemplo: #header { ... }

- Classe Selector: Selecione elementos por sua classe. Exemplo: .destaque { ... }

- Universal Selector: Selecione todos os elementos na página. Exemplo: \* { ... }

#### Sintaxe CSS e Onde Declarar

A sintaxe básica de uma regra CSS consiste em um seletor seguido por um bloco de declarações. As declarações são compostas por uma propriedade e um valor. Aqui está um exemplo:

```css
seletor {
  propriedade: valor;
}
```

Você pode declarar estilos CSS dentro de uma tag `<style>` no cabeçalho do documento HTML ou em um arquivo externo com a extensão .css e vinculá-lo ao HTML.

#### Comentários em CSS

Os comentários em CSS são usados para adicionar notas ou explicar o código. Eles não afetam o estilo da página. Comentários de uma linha começam com //, enquanto comentários de várias linhas são envolvidos por /_ ... _/.

```css
/* Isto é um comentário de várias linhas
   que explica o propósito deste estilo. */

// Este é um comentário de uma linha.
```

#### Propriedades de CSS: Background e Color

- Background: A propriedade background é usada para definir a cor de fundo de um elemento, além de imagens de fundo e outras configurações relacionadas.

```css
elemento {
  background-color: cor;
  background-image: url("imagem.jpg");
  /* Outras propriedades de background */
}
```

- Color: A propriedade color define a cor do texto dentro de um elemento.

```css
elemento {
  color: cor;
}
```

#### Formatação de Texto e Fontes

Para formatar texto e fontes, você pode usar propriedades como `font-family`, `font-size`, `font-weight`, `text-align` e mais.

```css
texto {
  font-family: Arial, sans-serif;
  font-size: 16px;
  font-weight: bold;
  text-align: center;
  /* Outras propriedades de formatação */
}
```

#### Elementos Block-level vs. Inline

- Elementos Block-level: Esses elementos ocupam toda a largura disponível e começam em uma nova linha, como `<div>`, `<p>`, `<h1>`, `<ul>`, etc.

- Elementos Inline: Esses elementos ocupam apenas o espaço necessário e não forçam uma nova linha, como `<span>`, `<a>`, `<strong>`, etc.

Lembre-se de que a escolha entre esses elementos afeta o layout e o comportamento da página.

#### Elementos `<details>` e `<summary>`

O elemento HTML `<details>` é usado para criar um bloco de informações que pode ser expandido ou recolhido pelo usuário. O texto dentro do elemento `<summary>` é usado como o cabeçalho para controlar a exibição do conteúdo oculto.

```html
<details>
  <summary>Clique para mostrar mais informações</summary>
  <p>Aqui está o conteúdo adicional que pode ser expandido ou recolhido.</p>
</details>
```

##### Exemplo 1: FAQ Interativo

```html
<details>
  <summary>O que é HTML?</summary>
  <p>
    HTML (HyperText Markup Language) é uma linguagem de marcação usada para
    estruturar o conteúdo em páginas da web.
  </p>
</details>

<details>
  <summary>O que é CSS?</summary>
  <p>
    CSS (Cascading Style Sheets) é uma linguagem usada para estilizar a
    apresentação das páginas da web, incluindo layout, cores e fontes.
  </p>
</details>
```

##### Exemplo 2: Instruções de Uso

```html
<details>
  <summary>Como usar nosso serviço?</summary>
  <p>Passo 1: Faça o registro em nosso site.</p>
  <p>Passo 2: Selecione o produto desejado em nossa loja online.</p>
  <p>Passo 3: Adicione o produto ao carrinho e finalize a compra.</p>
  <p>Passo 4: Aguarde a entrega em sua casa!</p>
</details>
```

# CSS - Cores

Você pode definir cores usando nomes de cores, valores hexadecimais ou valores RGB. Exemplos:

```css
p {
  color: red; /* Nome da cor */
  background-color: #00ff00; /* Valor hexadecimal */
  border: 1px solid rgb(255, 0, 0); /* Valor RGB */
}
```

## CSS - Margens, Padding, Bordas, Outline, Box Model

- Margens: Espaçamento externo de um elemento.
- Padding: Espaçamento interno de um elemento.
- Bordas: Linhas ao redor de um elemento.
- Outline: Contorno ao redor de um elemento.
- Box Model: Modelo de caixa que inclui conteúdo, padding, border e margin.
  Exemplo:

```css
Copy code div {
  margin: 10px;
  padding: 20px;
  border: 1px solid black;
  outline: 2px solid blue;
}
```

## CSS - Formatação para Links, Listas e Tabelas

- Formatação de Links:

```css
a {
  color: blue;
  text-decoration: none; /* Remove sublinhado */
}
```

- Formatação de Listas:

```css
ul {
  list-style-type: circle; /* Tipo de marcador */
  margin-left: 20px; /* Espaçamento à esquerda */
}
```

- Formatação de Tabelas:

```css
table {
  border-collapse: collapse; /* Colapsar bordas de células */
  width: 100%;
}
th,
td {
  border: 1px solid black;
  padding: 10px;
}
```

## Conteúdos Complementares

- [Curso de HTML e CSS - Aula 12 - Cores em CSS](https://www.youtube.com/watch?v=uKjKnztS3cY&pp=ygUbQ29yZXMgZW0gQ1NTIGN1cnNvIGVtIHZpZGVv)
- [Curso de HTML e CSS - Aula 13 - Fontes em CSS](https://www.youtube.com/watch?v=FLuQonci9wU&pp=ygUcZm9udGVzIGVtIENTUyBjdXJzbyBlbSB2aWRlbw%3D%3D)

<a id="listas"></a>

# CSS - Formatação para Listas e Tabelas

## Formatação de Listas

Você pode personalizar a aparência de listas em CSS. Aqui estão alguns exemplos:

```css
/* Alterando o tipo de marcador e espaçamento */
ul {
  list-style-type: square; /* Tipo de marcador */
  margin-left: 20px; /* Espaçamento à esquerda */
}
```

## Formatação de Tabelas

Você pode estilizar tabelas em CSS. Aqui está um exemplo:

```css
/* Estilizando células da tabela */
table {
  border-collapse: collapse; /* Colapsar bordas de células */
  width: 100%;
}
th,
td {
  border: 1px solid black;
  padding: 10px;
}
```

<a id="flex"></a>

# Flexbox

O Flexbox é um modelo de layout que facilita o design de layouts flexíveis e responsivos em CSS. Aqui está um exemplo de uso básico:

```css
/* Usando Flexbox para alinhar itens horizontalmente */
.container {
  display: flex;
  justify-content: center; /* Alinhar itens no centro horizontalmente */
  align-items: center; /* Alinhar itens no centro verticalmente */
}
```

<a id="grid"></a>

# Grid Layout

O Grid Layout é outro modelo de layout que permite criar layouts complexos de maneira eficiente. Aqui está um exemplo de uso:

```css
/* Criando uma grade de layout */
.container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr; /* Define 3 colunas */
  grid-gap: 10px; /* Espaçamento entre células */
}
```

<a id="mediaquery"></a>

# CSS - Responsividade (Media Query, viewport)

Para criar designs responsivos em CSS, você pode usar media queries e a unidade de medida `vw` (viewport width). Exemplos:

```css
/* Media query para telas menores que 600px */
@media (max-width: 600px) {
  body {
    font-size: 16px; /* Reduzir o tamanho da fonte */
  }
}

/* Usando vw para ajustar o tamanho com base na largura da tela */
header {
  font-size: 4vw; /* Tamanho de fonte responsivo */
  padding: 2vw; /* Preenchimento responsivo */
}
```

<a id="bootstrap"></a>

# CSS - Bootstrap

Bootstrap é um popular framework front-end de código aberto que simplifica o desenvolvimento web. Ele fornece uma coleção de estilos, componentes e ferramentas que tornam a criação de sites e aplicativos web responsivos mais eficiente. Aqui estão algumas informações importantes sobre Bootstrap:

- **O que é Bootstrap**: Bootstrap é uma biblioteca de código aberto que fornece um conjunto de estilos e componentes prontos para uso.

- **Como Funciona:** Bootstrap fornece classes CSS predefinidas que podem ser aplicadas a elementos HTML, o que permite criar um layout responsivo e atraente.

- **Instalação:** Você pode incluir o Bootstrap em seu projeto por meio de um arquivo CSS e um arquivo JavaScript. Existem várias maneiras de fazer isso, incluindo o download direto dos arquivos ou o uso de CDNs (Content Delivery Networks).

- **Layout:** Bootstrap oferece um sistema de grade flexível que permite criar layouts responsivos com facilidade. Você pode usar classes como container, row e col para organizar o conteúdo da página.

Bootstrap é uma ferramenta valiosa para desenvolvedores front-end, pois acelera o processo de desenvolvimento e ajuda a manter a consistência e a qualidade visual de seus projetos web.

<a id="javascript"></a>

# Javascript

<a id="variaveis"></a>

## JavaScript - Variáveis

Em JavaScript, as variáveis são usadas para armazenar dados. Elas podem ser comparadas a "caixas" em que você pode colocar informações. Aqui estão os principais tipos de variáveis em JavaScript:

### Variáveis com var

Antes do ES6 (ECMAScript 2015), a maneira mais comum de declarar variáveis em JavaScript era usando a palavra-chave var. No entanto, o uso de var é menos preferível em comparação com let e const, devido ao seu escopo de função. Aqui está um exemplo:

```javascript
var nome = "Evandro";
```

### Variáveis com let

A palavra-chave let é usada para declarar variáveis que têm escopo de bloco. Isso significa que elas só estão acessíveis dentro do bloco em que foram declaradas. Exemplo:

```javascript
let idade = 20;
```

### Variáveis com const

A palavra-chave const é usada para declarar variáveis constantes, ou seja, variáveis cujo valor não pode ser alterado após a atribuição inicial. Exemplo:

```javascript
const pi = 3.14159;
```

### Tipos de Dados

JavaScript possui diversos tipos de dados, incluindo números, strings, booleanos, arrays, objetos, entre outros.

```javascript
let numero = 42; // Número inteiro
let texto = "Olá, Mundo!"; // String
let estaChovendo = true; // Booleano
let frutas = ["maçã", "banana", "laranja"]; // Array
let pessoa = { nome: "Evandro", idade: 20 }; // Objeto
```

<a id="condicionais"></a>

## Condicionais

As estruturas condicionais permitem que você tome decisões em seu código, com base em condições especificadas. Em JavaScript, você pode usar as estruturas `if`, `else if` e `else` para criar condicionais.

Estrutura `if`
A estrutura `if` permite que você execute um bloco de código se uma condição for verdadeira. Veja um exemplo:

```javascript
let idade = 18;

if (idade >= 18) {
  console.log("Você é maior de idade.");
}
```

Estrutura `else` e `else if`
Você pode usar `else` para especificar um bloco de código que será executado se a condição do `if` for falsa. Você também pode usar `else if` para verificar múltiplas condições. Exemplo:

```javascript
let hora = 14;

if (hora < 12) {
  console.log("Bom dia!");
} else if (hora < 18) {
  console.log("Boa tarde!");
} else {
  console.log("Boa noite!");
}
```

## Operadores de Comparação

JavaScript possui diversos operadores de comparação, incluindo `==`, `!=`, `<`, `>`, `<=` e `>=`. Eles são usados para comparar valores. Exemplo:

```javascript
let numero = 42;

if (numero == 42) {
  console.log("O número é igual a 42.");
}
```

## Exemplos Completos

Aqui estão exemplos completos que mostram como usar variáveis e condicionais em JavaScript:

```javascript
// Exemplo 1: Usando variáveis
let nome = "Alice";
let idade = 25;
let estaChovendo = false;

// Exemplo 2: Estrutura condicional if
if (idade >= 18) {
  console.log(nome + " é maior de idade.");
} else {
  console.log(nome + " é menor de idade.");
}

// Exemplo 3: Estrutura condicional else if
if (estaChovendo) {
  console.log("É melhor levar um guarda-chuva.");
} else if (idade >= 18) {
  console.log("Pode sair sem guarda-chuva.");
} else {
  console.log("É melhor ficar em casa.");
}
```

## Operadores de Lógicos

Além dos operadores de comparação, JavaScript também oferece operadores lógicos para combinar condições. Os principais operadores lógicos são:

`&&` (E lógico): Retorna verdadeiro se ambas as condições forem verdadeiras.

`||` (OU lógico): Retorna verdadeiro se pelo menos uma das condições for verdadeira.

`!` (NÃO lógico): Inverte o valor de verdadeiro para falso e vice-versa.

### Estruturas de Controle

Estrutura `switch`

A estrutura `switch` é usada para verificar o valor de uma expressão e executar um bloco de código correspondente ao valor. É uma alternativa mais limpa e eficiente do que uma série de `if...else if...else`.

```javascript
let diaDaSemana = "quarta";

switch (diaDaSemana) {
  case "segunda":
    console.log("É segunda-feira.");
    break;
  case "quarta":
    console.log("É quarta-feira.");
    break;
  default:
    console.log("Outro dia da semana.");
}
```

**Operador Ternário**

O operador ternário é uma forma concisa de criar condicionais em uma única linha. Ele é frequentemente usado para atribuir valores com base em uma condição.

```javascript
let temperatura = 25;
let clima = temperatura > 30 ? "Quente" : "Frio";
console.log("O clima é " + clima);
```

<a id="repeticao"></a>

# JavaScript - Estruturas de Repetição

## Loop `for`

O loop `for` é usado quando você sabe antecipadamente quantas vezes deseja executar um bloco de código. É composto por três partes: inicialização, condição e iteração.

Exemplo:

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Número: " + i);
}
```

## Loop `while`

O loop `while` é usado quando você deseja que um bloco de código seja executado enquanto uma condição seja verdadeira.

Exemplo:

```javascript
let contador = 0;
while (contador < 5) {
  console.log("Contador: " + contador);
  contador++;
}
```

Loop `do...while`
O loop `do...while` é semelhante ao `while`, mas garante que o bloco de código seja executado pelo menos uma vez, mesmo se a condição for falsa.

Exemplo:

```javascript
let x = 0;
do {
  console.log("Número x: " + x);
  x++;
} while (x < 3);
```

## Estruturas de Repetição Avançadas

Loop `for...of`
O loop `for...of` é usado para iterar sobre elementos iteráveis, como arrays e strings.

Exemplo:

```javascript
let frutas = ["maçã", "banana", "laranja"];
for (let fruta of frutas) {
  console.log(fruta);
}
```

Loop `for...in`
O loop for...in é usado para iterar sobre as propriedades de um objeto.

Exemplo:

```javascript
let pessoa = { nome: "João", idade: 30, cidade: "São Paulo" };
for (let propriedade in pessoa) {
  console.log(propriedade + ": " + pessoa[propriedade]);
}
```

## Prática com Estruturas de Repetição

Exemplo 1: Soma de Números

```javascript
let soma = 0;

for (let i = 1; i <= 5; i++) {
  soma += i;
}

console.log("A soma dos números de 1 a 5 é: " + soma);
```

Exemplo 2: Encontrar Elemento em um Array

```javascript
let numeros = [10, 20, 30, 40, 50];
let alvo = 30;

let encontrado = false;

for (let numero of numeros) {
  if (numero === alvo) {
    encontrado = true;
    break;
  }
}

if (encontrado) {
  console.log("Elemento encontrado!");
} else {
  console.log("Elemento não encontrado.");
}
```

Exemplo 3: Iterar sobre Propriedades de um Objeto

```javascript
let carro = { marca: "Toyota", modelo: "Corolla", ano: 2020 };

for (let propriedade in carro) {
  console.log(propriedade + ": " + carro[propriedade]);
}
```

<a id="arrays"></a>

# Arrays em JavaScript

Um array é uma estrutura de dados que pode armazenar múltiplos valores. Em JavaScript, os arrays são usados para armazenar uma coleção ordenada de elementos, que podem ser de diferentes tipos, como números, strings, objetos, funções, etc.

**Criando um Array**
Em JavaScript, você pode criar um array de várias maneiras:

1. Array Literal:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];
```

2. Construtor Array:

```javascript
let frutas = new Array("Maçã", "Banana", "Laranja");
```

**Acessando Elementos do Array**

Os elementos de um array podem ser acessados pelo seu índice. Os índices em JavaScript começam em 0, ou seja, o primeiro elemento tem índice 0, o segundo tem índice 1 e assim por diante:

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];
console.log(frutas[0]); // Acessa o primeiro elemento (Maçã)
console.log(frutas[1]); // Acessa o segundo elemento (Banana)
```

### Propriedades e Métodos de Arrays

Arrays em JavaScript têm várias propriedades e métodos úteis, como:

`length`: Propriedade que retorna o número de elementos em um array.

```javascript
let frutas = ["Maçã", "Banana", "Laranja"];
console.log(frutas.length); // Retorna 3
```

`push()`: Método que adiciona um elemento ao final do array.

```javascript
frutas.push("Pera");
```

`pop()`: Método que remove o último elemento do array.

```javascript
let ultimaFruta = frutas.pop(); // Remove "Pera" e a armazena em ultimaFruta
```

`unshift()`: Método que adiciona um elemento no início do array.

```javascript
frutas.unshift("Manga");
```

`shift()`: Método que remove o primeiro elemento do array.

```javascript
let primeiraFruta = frutas.shift(); // Remove "Manga" e a armazena em primeiraFruta
```

**Iteração em Arrays**

Para percorrer os elementos de um array, você pode usar loops como `for`, `for...of` ou métodos específicos de array como `forEach()`:

- Usando `for`:

```javascript
for (let i = 0; i < frutas.length; i++) {
  console.log(frutas[i]);
}
```

- Usando `for...of`:

```javascript
for (let fruta of frutas) {
  console.log(fruta);
}
```

- Usando `forEach()`:

```javascript
frutas.forEach(function (fruta) {
  console.log(fruta);
});
```

**Manipulação de Arrays**

Você pode fazer várias operações em arrays, como adicionar, remover, pesquisar elementos e muito mais. Alguns exemplos:

- Adicionar Elementos:

```javascript
frutas.push("Pera"); // Adiciona ao final
frutas.unshift("Manga"); // Adiciona no início
```

- Remover Elementos:

```javascript
frutas.pop(); // Remove o último elemento
frutas.shift(); // Remove o primeiro elemento
```

- Pesquisar Elementos:

```javascript
let indice = frutas.indexOf("Banana"); // Retorna o índice de "Banana"
```

- Fatiar um Array:

```javascript
let citricas = frutas.slice(1, 3); // Retorna ["Banana", "Laranja"]
```

# Notas Importantes

- Os arrays em JavaScript são dinâmicos, o que significa que você pode alterar seu tamanho a qualquer momento, adicionando ou removendo elementos.

- Os elementos de um array não precisam ser do mesmo tipo.

- Os índices negativos contam a partir do final do array. Por exemplo, -1 representa o último elemento, -2 o penúltimo e assim por diante.

- Arrays podem ser utilizados para implementar pilhas (usando push e pop) e filas (usando push e shift), além de várias outras estruturas de dados.

- Use o método Array.isArray(arr) para verificar se uma variável é um array.

- Arrays são uma parte fundamental da programação em JavaScript e são amplamente utilizados para armazenar, manipular e processar dados em muitos tipos de aplicativos.

<a id="funcoes"></a>

# Funções

As funções são blocos de código reutilizáveis que podem ser definidos e chamados em JavaScript. Elas desempenham um papel fundamental na modularização do código e permitem que você execute ações específicas de maneira organizada. Aqui está uma explicação abrangente sobre funções em JavaScript:

Definindo Funções
Em JavaScript, você pode definir funções de várias maneiras. A forma mais comum é usando a declaração de função:

```javascript
function saudacao() {
  console.log("Olá, Entra21!");
}
```

Também é possível definir funções anônimas e atribuí-las a variáveis:

```javascript
const saudacao = function () {
  console.log("Olá, E21!");
};
```

**Chamando Funções**

Após definir uma função, você pode chamá-la para executar o código dentro dela:

```javascript
saudacao(); // Chama a função e exibe "Olá, E21!" no console.
```

**Parâmetros e Retorno**

Funções podem receber parâmetros e retornar valores:

```javascript
function somar(a, b) {
  return a + b;
}

let resultado = somar(3, 5); // A variável 'resultado' conterá 8.
```

**Escopo de Função**

Variáveis declaradas dentro de funções são locais ao escopo da função. Isso significa que elas não são acessíveis fora da função.

```javascript
function exemplo() {
  let dentroDaFuncao = "Esta variável está visível apenas dentro da função.";
}
console.log(dentroDaFuncao); // Isso resultará em um erro.
```

**Arrow Functions**

As Arrow Functions são uma sintaxe mais curta para definir funções:

```javascript
const saudacao = () => {
  console.log("Olá, E21!");
};
```

**Funções Callback**

Funções podem ser passadas como argumentos para outras funções. Isso é comum em JavaScript, especialmente ao lidar com assincronia. Essas funções são chamadas funções de callback.

```javascript
function fazerAlgo(callback) {
  // Realize alguma operação
  callback();
}

fazerAlgo(function () {
  console.log("Feito!");
});
```

<a id="eventos"></a>

## Tratamento de Eventos em JavaScript

O tratamento de eventos é fundamental em desenvolvimento web, permitindo que você responda a ações do usuário, como cliques, pressionamentos de tecla, movimentos do mouse, etc. Aqui está uma introdução ao tratamento de eventos em JavaScript:

**Adicionando Event Listeners**

Você pode usar o método `addEventListener` para atribuir eventos a elementos HTML:

```javascript
const botao = document.getElementById("botao");

meuBotao.addEventListener("click", function () {
  console.log("O botão foi clicado!");
});
```

**Tipos de Eventos Comuns**

- `click`: Disparado quando um elemento é clicado.
- `mouseover`: Disparado quando o cursor do mouse entra em um elemento.
- `mouseout`: Disparado quando o cursor do mouse sai de um elemento.
- `keydown`: Disparado quando uma tecla é pressionada.
- `submit`: Disparado quando um formulário é enviado.

**Removendo Event Listeners**

Para remover um evento, use `removeEventListener` com a mesma função de callback:

```javascript
meuBotao.removeEventListener("click", minhaFuncao);
```

**Objeto de Evento**

Quando um evento é acionado, um objeto de evento é passado para a função do manipulador de eventos, contendo informações sobre o evento, como o alvo, tipo de evento e muito mais.

```javascript
meuBotao.addEventListener("click", function (event) {
  console.log("Tipo de evento: " + event.type);
});
```

**Prevenindo Comportamentos Padrão**

Você pode usar `event.preventDefault()` para evitar que o comportamento padrão de um evento aconteça. Isso é útil, por exemplo, para impedir que um formulário seja enviado.

```javascript
const meuFormulario = document.getElementById("formulario");

meuFormulario.addEventListener("submit", function (event) {
  event.preventDefault(); // Evita o envio do formulário.
});
```

<a id="var-let-const"></a>

# As diferenças entre var x let x const

`var`, `let`, e `const`
Em JavaScript, existem três palavras-chave para declarar variáveis: `var`, `let` e `const`. Cada uma delas se comporta de forma ligeiramente diferente em relação ao escopo e à capacidade de reatribuição:

`var`: É uma palavra-chave mais antiga e possui escopo de função, o que significa que a variável declarada com `var` fica visível em toda a função em que foi declarada. Além disso, `var` permite a reatribuição.

`let`: Introduzido no ECMAScript 6 (ES6), `let` tem escopo de bloco, o que significa que a variável está visível apenas dentro do bloco em que foi declarada. Ela também pode ser reatribuída.

`const`: Também introduzido no ES6, `const` tem escopo de bloco, mas a diferença crucial é que as variáveis declaradas com `const` não podem ser reatribuídas após a sua inicialização. No entanto, elas ainda podem ser mutadas (se forem objetos ou arrays).

<a id="map-reduce-filter"></a>

# Métodos map, reduce, filter

Em JavaScript, arrays têm métodos úteis que podem simplificar o processo de manipulação de dados. Aqui estão alguns dos métodos mais comuns:

`map`: O método `map` é usado para criar um novo array com base no array original, aplicando uma função a cada elemento e retornando os resultados em um novo array.

`reduce`: O método `reduce` é usado para reduzir um array a um único valor. Ele executa uma função para cada elemento do array, acumulando um valor à medida que percorre o array.

`filter`: O método `filter` é usado para criar um novo array com todos os elementos que passam em um teste especificado em uma função.

<a id="matrizes"></a>

# Arrays Multidimensionais

Arrays multidimensionais são arrays que contêm outros arrays como elementos. Isso permite criar estruturas de dados complexas, como matrizes e tabelas. Cada dimensão é acessada aninhando colchetes adicionais:

```javascript
const matriz = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
];

console.log(matriz[1][2]); // Acessa o elemento 6 na segunda linha, terceira coluna.
```

<a id="metodos-numbers"></a>

# Métodos de Numbers

O tipo de dado `Number` em JavaScript possui métodos que permitem executar operações matemáticas e formatar números. Alguns métodos comuns incluem:

`toFixed`: Usado para especificar o número de casas decimais que um número terá.

`parseInt` e `parseFloat`: São usados para converter uma string em um número inteiro ou decimal, respectivamente.

`toExponential` e `toPrecision`: São usados para formatar números em notação exponencial ou com precisão específica.

## Precedência de Operadores Aritméticos

A precedência de operadores aritméticos determina a ordem em que as operações matemáticas são executadas em uma expressão. Em JavaScript, a precedência segue uma hierarquia padrão, com multiplicação e divisão tendo precedência sobre adição e subtração. Parênteses podem ser usados para forçar a ordem desejada.

## Precedência de Operadores Lógicos

A precedência de operadores lógicos determina a ordem em que operações lógicas são avaliadas. Em JavaScript, os operadores lógicos têm precedência, com o "E lógico" (`&&`) tendo uma precedência mais alta que o "OU lógico" (`||`).

## Avaliação de Curto-Circuito

A avaliação de curto-circuito é um conceito fundamental em JavaScript, usado em operações lógicas. Ela permite que você interrompa a avaliação de uma expressão lógica assim que o resultado for determinado. Por exemplo, no caso do operador `&&`, se o primeiro operando for `false`, o segundo operando não será avaliado.

<a id="processamento-assincrono"></a>

## Processamento Assíncrono

JavaScript, por padrão, é single-threaded e assíncrono. Isso significa que certas operações, como solicitações de rede, não bloqueiam a execução do código. O processamento assíncrono em JavaScript é crucial para operações intensivas de E/S.

- **Promises e Callbacks:**

Promises são objetos que representam a conclusão ou o fracasso eventual de uma operação assíncrona. Elas melhoram a legibilidade e a manipulação de erros em comparação com os callbacks. Exemplo:

```javascript
const minhaPromise = new Promise((resolve, reject) => {
  // operação assíncrona
  if (sucesso) {
    resolve("Sucesso!");
  } else {
    reject("Erro!");
  }
});

minhaPromise
  .then((resultado) => console.log(resultado))
  .catch((erro) => console.error(erro));
```

- Callbacks são funções passadas como argumentos para outras funções, para serem executadas mais tarde. No entanto, eles podem levar a um padrão chamado "Callback Hell" quando há muitos deles aninhados.

**Async/Await:**

- Async/Await é uma maneira mais limpa de trabalhar com código assíncrono, introduzida no ECMAScript 2017 (ES8). Permite escrever código assíncrono como se fosse síncrono, tornando-o mais legível.

```javascript
async function minhaFuncao() {
  try {
    const resultado = await operacaoAssincrona();
    console.log(resultado);
  } catch (erro) {
    console.error(erro);
  }
}
```

# Consumo de API

<a id="consumo-de-api-com-ajax"></a>

### Consumo de API com AJAX

- AJAX (Asynchronous JavaScript and XML) é uma técnica que permite atualizações parciais de uma página, sem a necessidade de recarregar a página inteira. O objeto XMLHttpRequest é frequentemente usado para realizar solicitações HTTP assíncronas.

- JSON (JavaScript Object Notation) é um formato leve de troca de dados. É fácil de ler e escrever para humanos e fácil de analisar e gerar para máquinas.
  XML (eXtensible Markup Language) é outro formato de dados comum.

<a id="consumo-de-api-com-fetch-e-asyncawait"></a>

### Consumo de API com Fetch e Async/Await

- **Fetch API:**

O Fetch API fornece uma interface JavaScript para acessar e manipular partes do pipeline HTTP, como solicitações e respostas. É uma alternativa moderna ao XMLHttpRequest.

```javascript
fetch("https://api.exemplo.com/dados")
  .then((response) => response.json())
  .then((data) => console.log(data))
  .catch((error) => console.error("Erro:", error));
```

- **Async/Await com Fetch:**

```javascript
async function obterDados() {
  try {
    const response = await fetch("https://api.exemplo.com/dados");
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Erro:", error);
  }
}
```

<a id="localstorage-sessionstorage"></a>

# LocalStorage e SessionStorage

Esses mecanismos permitem armazenar dados no navegador do cliente.

- LocalStorage:

  Armazena dados com um tempo de vida maior.

- SessionStorage:

  Armazena dados para a duração de uma sessão.

<a id="nodejs"></a>

# Node.js

<a id="criando-o-primeiro-servidor-http"></a>

## Criando o primeiro servidor HTTP

Node.js permite criar servidores HTTP de forma fácil e eficiente.

- Exemplo:

```javascript
const http = require("http");

const server = http.createServer((req, res) => {
  res.writeHead(200, { "Content-Type": "text/plain" });
  res.end("Hello, Node.js!");
});

const PORT = 3000;
server.listen(PORT, () => {
  console.log(`Servidor rodando em http://localhost:${PORT}/`);
});
```

## Módulo HTTP - Rotas

Node.js facilita a criação de rotas para diferentes URLs.

- Exemplo:

```javascript
const http = require("http");

const server = http.createServer((req, res) => {
  if (req.url === "/") {
    res.writeHead(200, { "Content-Type": "text/plain" });
    res.end("Página inicial");
  } else if (req.url === "/sobre") {
    res.writeHead(200, { "Content-Type": "text/plain" });
    res.end("Página sobre nós");
  } else {
    res.writeHead(404, { "Content-Type": "text/plain" });
    res.end("Página não encontrada");
  }
});

const PORT = 3000;
server.listen(PORT, () => {
  console.log(`Servidor rodando em http://localhost:${PORT}/`);
});
```

<a id="express"></a>

### Express: Criando uma API com o framework Express

Express é um framework para Node.js que simplifica o desenvolvimento de aplicativos web.

Instalação:

```bash
npm install express
```

Exemplo de API básica:

```javascript
const express = require("express");
const app = express();
const PORT = 3000;

app.get("/api/exemplo", (req, res) => {
  res.json({ mensagem: "Olá, esta é uma resposta da API!" });
});

app.listen(PORT, () => {
  console.log(`Servidor Express rodando em http://localhost:${PORT}`);
});
```

<a id="express-roteamento"></a>

### Express: Roteamento

Express oferece um sistema de roteamento para organizar as diferentes partes de uma aplicação.

Exemplo:

```javascript
const express = require("express");
const app = express();
const PORT = 3000;

app.get("/", (req, res) => {
  res.send("Página inicial");
});

app.get("/sobre", (req, res) => {
  res.send("Página sobre nós");
});

app.listen(PORT, () => {
  console.log(`Servidor Express rodando em http://localhost:${PORT}`);
});
```

<a id="express-rotas-dinâmicas"></a>

### Express: Rotas Dinâmicas

Express suporta rotas dinâmicas que podem processar parâmetros variáveis.

Exemplo:

```javascript
const express = require("express");
const app = express();
const PORT = 3000;

app.get("/usuario/:id", (req, res) => {
  const userId = req.params.id;
  res.send(`Detalhes do usuário ${userId}`);
});

app.listen(PORT, () => {
  console.log(`Servidor Express rodando em http://localhost:${PORT}`);
});
```

<a id="cors"></a>

### Segurança em Aplicações Web - CORS

Cross-Origin Resource Sharing (CORS) é uma política de segurança que permite ou restringe recursos em uma página web, comumente aplicada a requisições AJAX.

<a id="middlewares"></a>

### Middlewares

Middlewares são funções que têm acesso ao objeto de solicitação (request), ao objeto de resposta (response) e à próxima função de middleware no ciclo de solicitação-resposta do Express.

<a id="api-rest"></a>

### Conceitos Básicos de API REST

API REST (Representational State Transfer) é um estilo de arquitetura que define um conjunto de regras para criar serviços web.

Recursos:

Em uma API REST, os recursos (dados ou serviços) são identificados por URLs.

Métodos HTTP:

- GET: Recupera um recurso.
- POST: Cria um novo recurso.
- PUT: Atualiza um recurso existente.
- DELETE: Remove um recurso.

<a id="status-codes"></a>

### Status Codes

Códigos de status HTTP indicam o resultado da solicitação. Alguns exemplos são:

- 200 OK: Solicitação bem-sucedida.
- 404 Not Found: Recurso não encontrado.
- 500 Internal Server Error: Erro interno do servidor.

<a id="arquivos-estáticos"></a>

### Trabalhando com Arquivos Estáticos

Node.js pode servir arquivos estáticos, como HTML, CSS e imagens, para os clientes.

<a id="commonjs-es6"></a>

### CommonJS Modules vs. ES6 Modules

Node.js suporta tanto o sistema de módulos CommonJS quanto o ES6. A diferença principal está na forma como os módulos são importados/exportados.

<a id="jwt"></a>

### Segurança em Aplicações Web - Autenticação com JWT

JSON Web Token (JWT) é um padrão para autenticação. Ele é composto por informações compactadas e assinadas para troca segura de informações.

<a id="crud"></a>

# Node.js - Construindo um CRUD

CRUD (Create, Read, Update, Delete) é um conjunto de operações básicas em sistemas de gerenciamento de banco de dados.

Exemplo:

- Criar (Create): POST /usuarios
- Ler (Read): GET /usuarios
- Atualizar (Update): PUT /usuarios/:id
- Excluir (Delete): DELETE /usuarios/:id
