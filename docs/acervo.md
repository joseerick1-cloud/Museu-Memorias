# acervo.html

Este arquivo define a página geral do acervo do museu. Ele usa HTML semântico e classes CSS para criar um catálogo visual de itens históricos.

## Estrutura HTML

- `<header class="main-header">` apresenta a marca e a navegação.
- `<section class="hero-section">` exibe o banner superior da página de acervo.
- `<div class="tabs-container">` mostra os links para todas as categorias do acervo.
- `<div class="content-layout">` separa a grade principal da sidebar.
- `<section class="gallery-grid">` organiza os itens em uma grade responsiva.
- `<aside class="sidebar">` apresenta a coleção em destaque.
- `<footer class="main-footer">` finaliza a página.

## Código principal

```html
<section class="hero-section">
  <div class="hero-overlay"></div>
  <div class="hero-content">
    <h1>Explore o acervo</h1>
    <div class="decorator"><span>♦</span> <hr> <span>♦</span></div>
  </div>
</section>
```

```html
<div class="tabs-container">
  <a href="acervo.html" class="tab-btn active">Todos</a>
  <a href="fotografias.html" class="tab-btn">Fotografias</a>
  <a href="objetos.html" class="tab-btn">Objetos</a>
  <a href="documentos.html" class="tab-btn">Documentos</a>
  <a href="historia-oral.html" class="tab-btn">História oral</a>
</div>
```

```html
<section class="gallery-grid">
  <div class="grid-item">
    <div class="img-wrapper placeholder-1"></div>
    <h3>Estação Ferroviária</h3>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-2"></div>
    <h3>Desfile Cívico</h3>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-3"></div>
    <h3>Máquina de Costura</h3>
  </div>
</section>
```

```html
<aside class="sidebar">
  <div class="featured-card">
    <div class="featured-header">
      <span>Coleção em destaque</span>
      <div class="card-decorator"></div>
    </div>
    <div class="featured-body">
      <div class="featured-img placeholder-featured"></div>
      <h3>Pontes que uniram histórias</h3>
      <p>Registros fotográficos e documentos sobre as pontes que conectaram bairros...</p>
      <a href="#" class="btn-view">Ver item <span class="arrow">→</span></a>
    </div>
  </div>
</aside>
```

## Classes CSS usadas

- `.hero-section`: banner do acervo com imagem de fundo e altura fixa.
- `.tabs-container`: container flexível das abas de navegação.
- `.tab-btn`: botões que simulam guias de categoria.
- `.tab-btn.active`: estilo do guia ativo.
- `.content-layout`: grid de duas colunas para o conteúdo principal e a sidebar.
- `.gallery-grid`: grade responsiva que organiza cards.
- `.grid-item`: bloco de item do acervo.
- `.img-wrapper`: placeholder de imagem com efeito sépia.
- `.placeholder-1` a `.placeholder-7`: cada uma define uma imagem de fundo diferente.
- `.featured-card`, `.featured-header`, `.featured-body`: card de destaque lateral.
- `.featured-img`: placeholder grande do card lateral.

## Relação com `styles.css`

O HTML do acervo funciona com as regras de grade e placeholders de `styles.css`. Os itens históricos são apresentados sem `<img>`, usando classes de background no CSS para controlar imagem e estética.
