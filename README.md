# IFRN - Campus Macau
# Curso Técnico Integrado em Informática
# AUTORIA WEB
# Prof. Guilherme Leal Santos

## 30/04 - Introdução a HTML

### Introdução

As principais tags HTML se dividem em grupos que estruturam o documento (html, head, body), organizam o conteúdo (títulos, parágrafos, listas, links, imagens) e dão significado semântico ao layout (header, nav, main, section, article, aside, footer, etc.).

Um elemento HTML é formado, em geral, por uma tag de abertura, conteúdo e tag de fechamento, podendo ter atributos para configurar detalhes (por exemplo, <p class="destaque">Texto</p>).

Os elementos indicam um texto, imagens e outros conteúdos para que o navegador saiba “o que é o quê” (título, parágrafo, link, imagem, seção etc.).

### Estrutura básica do documento

<!DOCTYPE html> não é uma tag, é uma instrução que informa ao navegador que o documento segue o padrão HTML5 e deve ser renderizado no modo padrão.

<html> é o elemento raiz: tudo que faz parte da página (head e body) fica dentro dele, e o atributo lang indica o idioma, ajudando leitores de tela e motores de busca.

<head> contém metadados: título, codificação (<meta charset>), descrição, links para CSS, scripts, ícones, entre outros, que normalmente não aparecem diretamente na tela.

<title> define o texto da aba/janela do navegador e é importante para SEO (Search Engine Optimization) e usabilidade (“em que página estou?”).

<meta> insere metadados diversos, como charset, viewport para responsividade e descrições para mecanismos de busca.

<body> contém todo o conteúdo visível e interativo da página: textos, imagens, links, formulários, menus, etc.

### Títulos e parágrafos

HTML usa elementos específicos para organizar o texto em títulos e parágrafos, criando hierarquia de conteúdo.

<h1> … <h6>: representam níveis de título, sendo <h1> o título principal da página, <h2> subtítulos, e assim por diante até <h6>.

<p>: representa um parágrafo de texto; cada parágrafo deve ser envolvido por um <p> separado em vez de usar quebras de linha aleatórias.

<br>: insere apenas uma quebra de linha dentro de um parágrafo; deve ser usado com moderação, pois não cria nova unidade semântica como um <p>.

Boas práticas: usar apenas um <h1> por página e seguir a hierarquia (h1 → h2 → h3) ajuda na organização lógica, acessibilidade e SEO.

### Ênfase, destaque e texto inline

Para dar significado à ênfase e destaque, existem tags específicas:

<strong>: indica que o conteúdo é de grande importância; por padrão é renderizado em negrito e é reconhecido pelos leitores de tela como ênfase forte.

<em>: indica ênfase (“entonação” na leitura); por padrão é itálico, mas o ponto central é o significado, não o estilo.

<span>: contêiner genérico inline, usado para aplicar estilos ou atributos a trechos pequenos de texto quando não houver uma tag semântica mais adequada.

Boas práticas: usar <strong> e <em> quando for realmente importante para o sentido da frase, e <span> apenas como último recurso, evitando perda de semântica.

### Listas

Listas são essenciais para agrupar itens relacionados de forma organizada.

<ul> (unordered list): lista não ordenada, geralmente exibida com marcadores (bolinhas) para itens sem ordem específica (por exemplo, “hobbies”, “links úteis”).

<ol> (ordered list): lista ordenada, numerada, usada quando a ordem importa (passos de um procedimento, ranking, etc.).

<li> (list item): cada item individual de uma <ul> ou <ol> deve estar dentro de um <li>.

Exemplo:

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

### Links e navegação

Links conectam páginas e recursos na Web.

<a> (anchor): cria um hiperlink por meio do atributo href, que pode apontar para outra página, seção da mesma página, e-mail, arquivo ou recurso externo.

O texto entre <a> e </a> é o que o usuário vê e clica, devendo descrever claramente o destino (evitar apenas “clique aqui”).

<nav>: agrupa blocos de links de navegação importantes, como menus principais, barras laterais de navegação ou rodapés com links globais.

Exemplo típico de menu:

<nav>
  <ul>
    <li><a href="#inicio">Início</a></li>
    <li><a href="#sobre">Sobre</a></li>
    <li><a href="#contato">Contato</a></li>
  </ul>
</nav>

### Imagens e mídia

Imagens, áudio e vídeo enriquecem a página, e também têm tags próprias.

<img>: insere imagens; usa o atributo obrigatório src (caminho da imagem) e o atributo alt, que descreve a imagem para quem não pode vê-la (leitores de tela, conexão lenta, erro de carregamento).

<audio> e <video>: elementos semânticos para incorporar áudio e vídeo com controles nativos (controls), podendo ter múltiplas fontes (<source>) para formatos diferentes.

Exemplo:

<img src="foto.jpg" alt="Foto do campus do IFRN ao pôr do sol">

### Estrutura semântica de página (layout)

HTML5 trouxe elementos semânticos que substituem muitos usos genéricos de <div> para estruturar o layout.

<header>: cabeçalho da página ou de uma seção; costuma conter logo, título, navegação principal.

<main>: delimita o conteúdo principal da página, único por documento, facilitando navegação por leitores de tela.

<section>: seção temática do documento, geralmente com um título próprio (por exemplo, “Sobre”, “Serviços”, “Contato”).

<article>: bloco de conteúdo independente e reutilizável (post de blog, notícia, card de produto, comentário), que faz sentido fora do contexto imediato.

<aside>: conteúdo complementar ou relacionado, como barras laterais, boxes de “leia também”, anúncios.

<footer>: rodapé da página ou de uma seção, com informações de autoria, direitos, links secundários, contatos, etc.

<div>: contêiner genérico em bloco, sem significado semântico próprio, útil para agrupamento quando nenhum dos elementos semânticos se aplica.

Esses elementos ajudam buscadores e tecnologias assistivas a entenderem a função de cada parte da página, melhorando acessibilidade e SEO.

### Tabelas: <table>, <tr>, <th>, <td>, <thead>, <tbody>, <caption>

Tabelas são usadas para dados tabulares (não para layout).

<table>: contêiner principal da tabela.

<tr> (table row): linha da tabela.

<th> (table header): célula de cabeçalho, geralmente em negrito e centralizada, descreve a coluna ou linha.

<td> (table data): célula de dados comum.

<thead> e <tbody>: agrupam cabeçalho e corpo da tabela, respectivamente, melhorando estrutura e acessibilidade.

<caption>: legenda da tabela, descrevendo sucintamente seu conteúdo.

Exemplo:

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

### Formulários: <form>, <label>, <input>, <textarea>, <select>, <button>

Formulários coletam dados do usuário, e são fundamentais em sistemas Web.

<form>: contêiner do formulário; usa atributos como action (para onde enviar) e method (GET/POST).

<label>: rótulo de campo; associado a um controle pelo atributo for (ligado ao id do input), melhorando acessibilidade e usabilidade.

<input>: campo de entrada genérico com tipos diversos (text, email, password, checkbox, radio, number, etc.), definidos pelo atributo type.

<textarea>: campo de texto multilinha para mensagens mais longas.

<select> e <option>: listas suspensas (combobox) para seleção de uma ou mais opções.

<button>: botão clicável, usado para enviar o formulário (type="submit") ou para ações gerais (type="button").

Exemplo:

```html
<form action="/inscrever" method="post">
  <label for="nome">Nome</label>
  <input type="text" id="nome" name="nome" required>

  <label for="email">E-mail</label>
  <input type="email" id="email" name="email" required>

  <button type="submit">Enviar</button>
</form>
```

### Boas práticas com as principais tags

* Preferir tags semânticas (header, nav, main, section, article, aside, footer) em vez de excesso de <div> melhora acessibilidade, manutenção e SEO.

* Manter uma hierarquia coerente de títulos (h1 único, seguido de h2, h3 etc.) ajuda leitores de tela e organização do conteúdo.

* Sempre usar alt em <img> e <label> corretamente associados a campos de formulário aumenta muito a acessibilidade da página.

* Usar <table> apenas para dados tabulares; para layout, combinar HTML semântico com CSS (Flexbox, Grid), evitando gambiarras visuais.

