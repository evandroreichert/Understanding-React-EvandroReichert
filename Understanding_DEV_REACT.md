# Tabela de Conteúdos

- [Git e GitHub](#github)
- [HTML](#html)
  - [Tipos de Listas](#tipos-de-listas)
  - [Imagens](#imagens)

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

## Tags semânticas em HTML

As tags semânticas ajudam a estruturar o conteúdo de uma maneira significativa para os mecanismos de busca e para a acessibilidade. Algumas das tags semânticas mais comuns são:

- `<header>`: Define o cabeçalho da página ou de uma seção.
- `<main>`: Define o conteúdo principal da página.
- `<footer>`: Define o rodapé da página ou de uma seção.
- `<section>`: Define uma seção genérica.
- `<nav>`: Define um bloco de navegação.
- `<article>`: Define um conteúdo autônomo e independente.
- `<aside>`: Define um conteúdo relacionado ou auxiliar.

---

# HTML - Elementos estruturais não semânticos 

## Elementos estruturais não semânticos

Além das tags semânticas, existem elementos não semânticos que são usados para organizar e estilizar o layout da página. Dois dos elementos mais comuns são:

- `<div>`: É uma divisão genérica usada para agrupar outros elementos e aplicar estilos.
- `<span>`: É usado para aplicar estilos a uma parte específica do texto dentro de um elemento.

Esses elementos não têm um significado semântico intrínseco, mas desempenham um papel importante na criação de layouts complexos.

---

# HTML - Principais Tags 

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

