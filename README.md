<a id="readme-top"></a>

<!-- PROJECT SHIELDS (opcional) -->
<!--
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/usuario/repositorio.svg)]()
-->

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h1>IFRN - Campus Macau</h1>
  <h3>Curso Técnico Integrado em Informática</h3>
  <h4>Autoria Web</h4>
  <p><strong>Prof. Guilherme Leal Santos</strong></p>
</div>

---

## Sumário

- [Sumário](#sumário)
- [Sobre o material](#sobre-o-material)
- [Aula 01 - Introdução ao HTML](#aula-01---introdução-ao-html)
  - [Objetivos](#objetivos)
  - [Conteúdo abordado](#conteúdo-abordado)
    - [Estrutura básica do documento](#estrutura-básica-do-documento)
    - [Títulos e parágrafos](#títulos-e-parágrafos)
    - [Ênfase, destaque e texto inline](#ênfase-destaque-e-texto-inline)
    - [Listas](#listas)
    - [Links e navegação](#links-e-navegação)
    - [Imagens e mídia](#imagens-e-mídia)
    - [Estrutura semântica da página](#estrutura-semântica-da-página)
    - [Tabelas](#tabelas)
    - [Formulários](#formulários)
  - [Exemplos](#exemplos)
    - [Lista não ordenada](#lista-não-ordenada)
    - [Menu de navegação](#menu-de-navegação)
    - [Imagem com descrição](#imagem-com-descrição)
    - [Formulário simples](#formulário-simples)
    - [Tabela simples](#tabela-simples)
  - [Boas práticas](#boas-práticas)
  - [Recursos adicionais](#recursos-adicionais)

---

## Sobre o material

Este repositório reúne os conteúdos da disciplina **Autoria Web**. O objetivo é servir como apoio às aulas, facilitando a consulta, a organização do conteúdo e a evolução do material ao longo do curso.

---

## Aula 01 - Introdução ao HTML

**Data:** 30/04

### Objetivos

Ao final desta aula, o estudante deverá ser capaz de:

- Compreender a estrutura básica de um documento HTML.
- Identificar as principais tags semânticas.
- Organizar textos, listas, links, imagens, tabelas e formulários.
- Aplicar boas práticas de acessibilidade e organização do conteúdo.

### Conteúdo abordado

#### Estrutura básica do documento

- `<!DOCTYPE html>` informa ao navegador que o documento segue o padrão HTML5.
- `<html>` é o elemento raiz da página.
- `<head>` reúne metadados, título, links externos e configurações.
- `<title>` define o texto exibido na aba do navegador.
- `<meta>` adiciona informações como codificação, viewport e descrição.
- `<body>` contém o conteúdo visível da página.

#### Títulos e parágrafos

- `<h1>` a `<h6>` representam níveis de título.
- `<p>` representa um parágrafo.
- `<br>` insere quebra de linha dentro de um bloco de texto.

#### Ênfase, destaque e texto inline

- `<strong>` indica importância forte.
- `<em>` indica ênfase.
- `<span>` é um contêiner inline genérico.

#### Listas

- `<ul>` cria uma lista não ordenada.
- `<ol>` cria uma lista ordenada.
- `<li>` representa cada item da lista.

#### Links e navegação

- `<a>` cria hiperlinks.
- `<nav>` agrupa links de navegação.

#### Imagens e mídia

- `<img>` insere imagens.
- `<audio>` insere conteúdo de áudio.
- `<video>` insere conteúdo de vídeo.

#### Estrutura semântica da página

- `<header>` define o cabeçalho.
- `<main>` define o conteúdo principal.
- `<section>` define uma seção temática.
- `<article>` define conteúdo independente.
- `<aside>` define conteúdo complementar.
- `<footer>` define o rodapé.
- `<div>` é um contêiner genérico sem semântica.

#### Tabelas

- `<table>` cria a tabela.
- `<tr>` cria linhas.
- `<th>` cria células de cabeçalho.
- `<td>` cria células de dados.
- `<thead>` agrupa o cabeçalho.
- `<tbody>` agrupa o corpo da tabela.
- `<caption>` adiciona legenda à tabela.

#### Formulários

- `<form>` define o formulário.
- `<label>` associa rótulos aos campos.
- `<input>` cria campos de entrada.
- `<textarea>` cria campo de texto multilinha.
- `<select>` e `<option>` criam listas de seleção.
- `<button>` cria botões de ação.

---

### Exemplos

#### Lista não ordenada

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

#### Menu de navegação

```html
<nav>
  <ul>
    <li><a href="#inicio">Início</a></li>
    <li><a href="#sobre">Sobre</a></li>
    <li><a href="#contato">Contato</a></li>
  </ul>
</nav>
```

#### Imagem com descrição

```html
<img src="foto.jpg" alt="Foto do campus do IFRN ao pôr do sol">
```

#### Formulário simples

```html
<form action="/inscrever" method="post">
  <label for="nome">Nome</label>
  <input type="text" id="nome" name="nome" required>

  <label for="email">E-mail</label>
  <input type="email" id="email" name="email" required>

  <button type="submit">Enviar</button>
</form>
```

#### Tabela simples

```html
<table>
  <caption>Disciplinas do curso</caption>
  <thead>
    <tr>
      <th>Disciplina</th>
      <th>Carga horária</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Autoria Web</td>
      <td>60h</td>
    </tr>
  </tbody>
</table>
```

---

### Boas práticas

- Prefira tags semânticas em vez de excesso de `<div>`.
- Mantenha uma hierarquia coerente de títulos.
- Use `alt` em todas as imagens.
- Associe corretamente `label` e `input`.
- Use `<table>` apenas para dados tabulares.
- Combine HTML semântico com CSS para layout, em vez de usar tabelas para posicionamento.

---

### Recursos adicionais

- [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
- [W3C - HTML](https://www.w3.org/TR/html52/)

---

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>