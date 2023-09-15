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
- [JavaScript](#javascript)
  - [Variáveis](#variaveis)
  - [Condicionais](#condicionais)

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
*Como usar:* [Utilizando fork](https://docs.github.com/pt/github/getting-started-with-github/quickstart/fork-a-repo)

## `git stash`
Salvar trabalho no estado atual para continuar com outra tarefa, e voltar depois.
*Documentação:* [Git Stash](https://git-scm.com/docs/git-stash)

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
<img src="caminho/para/imagem.jpg" alt="Descrição da imagem">
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
  <input type="text" id="nome" name="nome" placeholder="Digite seu nome">
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Digite seu email">
  
  <input type="submit" value="Enviar">
</form>
```

### CSS Fundamentos 

#### Seletores CSS
  
Em CSS, os seletores são usados para aplicar estilos a elementos específicos em uma página web. Aqui estão alguns tipos comuns de seletores:

- Elemento Selector: Selecione elementos HTML diretamente. Exemplo: p { ... }

- ID Selector: Selecione um elemento pelo atributo "id". Exemplo: #header { ... }

- Classe Selector: Selecione elementos por sua classe. Exemplo: .destaque { ... }

- Universal Selector: Selecione todos os elementos na página. Exemplo: * { ... }

#### Sintaxe CSS e Onde Declarar

A sintaxe básica de uma regra CSS consiste em um seletor seguido por um bloco de declarações. As declarações são compostas por uma propriedade e um valor. Aqui está um exemplo:

```css
seletor {
    propriedade: valor;
}
```

Você pode declarar estilos CSS dentro de uma tag `<style>` no cabeçalho do documento HTML ou em um arquivo externo com a extensão .css e vinculá-lo ao HTML.

#### Comentários em CSS

Os comentários em CSS são usados para adicionar notas ou explicar o código. Eles não afetam o estilo da página. Comentários de uma linha começam com //, enquanto comentários de várias linhas são envolvidos por /* ... */.

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
    background-image: url('imagem.jpg');
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
  <p>HTML (HyperText Markup Language) é uma linguagem de marcação usada para estruturar o conteúdo em páginas da web.</p>
</details>

<details>
  <summary>O que é CSS?</summary>
  <p>CSS (Cascading Style Sheets) é uma linguagem usada para estilizar a apresentação das páginas da web, incluindo layout, cores e fontes.</p>
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
Copy code
div {
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
th, td {
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
th, td {
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

Operadores de Comparação
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