# exposicao.html

Este arquivo é a página da exposição "Caminhos da Feira". Ele combina narrativa histórica, galeria visual, linha do tempo, depoimentos e um formulário de agendamento.

## Estrutura HTML

- `<header class="main-header">`: topo com navegação e marcação de página ativa.
- `<section class="hero-exposicao">`: banner com título e descrição da exposição.
- `<main class="main-container content-layout">`: divide o conteúdo principal e a sidebar.
- `<section class="expo-main-content">`: contém introdução, galeria, linha do tempo e depoimento.
- `<aside class="sidebar">`: apresenta informações extras e um formulário de contato.
- `<footer class="main-footer">`: rodapé institucional.

## Código principal

```html
<section class="hero-exposicao">
  <div class="hero-overlay"></div>
  <div class="hero-content-expo">
    <h1>Caminhos da Feira</h1>
    <div class="decorator"><span>♦</span> <hr> <span>♦</span></div>
    <p class="hero-expo-desc">Uma exposição sobre os trajetos que conectaram pessoas, mercadorias e histórias. Das primeiras feiras livres às grandes transformações urbanas, descubra as histórias que fizeram nossa cidade pulsar.</p>
  </div>
</section>
```

```html
<div class="horizontal-gallery">
  <div class="gallery-item">
    <div class="mini-img expo-img-1"></div>
    <h4>Feira Livre no Largo da Matriz</h4>
    <p class="meta">c. 1895 • Fotografia</p>
    <p class="credit">Acervo: Coleção José Ferreira</p>
  </div>
  <div class="gallery-item">
    <div class="mini-img expo-img-2"></div>
    <h4>Lista de vendedores da feira</h4>
    <p class="meta">1908 • Documento</p>
    <p class="credit">Acervo: Arquivo Municipal</p>
  </div>
</div>
```

```html
<div class="timeline-banner">
  <div class="timeline-title">Linha do tempo</div>
  <div class="timeline-scroll">
    <div class="timeline-node">
      <span class="year">1850</span>
      <span class="desc">Primeiras feiras livres registradas</span>
    </div>
    <div class="timeline-node">
      <span class="year">2020</span>
      <span class="desc">Memória que inspira o futuro</span>
    </div>
  </div>
</div>
```

```html
<div class="testimonial-section">
  <span class="large-quote">“</span>
  <div class="testimonial-card">
    <div class="author-photo"></div>
    <div class="testimonial-text">
      <p>"Minha mãe vinha ainda de madrugada. Montava a banca, arrumava tudo com capricho e dizia que a feira era a escola da vida..."</p>
      <span class="author-info">DONA LUZIA, 82 ANOS<br><em>Entrevista em 24/03/2019</em></span>
    </div>
  </div>
</div>
```

```html
<aside class="sidebar">
  <div class="sidebar-box menu-box">
    <div class="box-header">Sobre a exposição</div>
    <div class="box-body">...</div>
  </div>
  <div class="sidebar-box form-box">
    <div class="box-header">Agende uma visita guiada</div>
    <form class="museum-form">...</form>
  </div>
</aside>
```

## Classes CSS usadas

- `.hero-exposicao`: aplica imagem de fundo, altura e posicionamento do banner.
- `.hero-overlay`: escurece a imagem para manter o texto legível.
- `.hero-content-expo`: posiciona o título e a descrição sobre o banner.
- `.horizontal-gallery`: exibe quatro itens em uma grade de galeria horizontal.
- `.mini-img`: cria o bloco de miniaturas com estilo de foto antiga.
- `.expo-img-1`, `.expo-img-2`, `.expo-img-3`, `.expo-img-4`: definem as imagens de cada item da galeria.
- `.timeline-banner`: bloco escuro que organiza eventos históricos.
- `.timeline-node`, `.year`, `.desc`: formata cada evento da linha do tempo.
- `.testimonial-section`, `.testimonial-card`, `.large-quote`, `.author-photo`: criam o bloco de depoimento.
- `.sidebar-box`, `.box-header`, `.box-body`: formatam os blocos laterais.
- `.museum-form`, `.form-group`, `.form-row`, `.btn-submit`: estruturam o formulário de agendamento.

## Relação com `styles.css`

A página de exposição depende de estilos exclusivos de `styles.css` para a experiência visual:
- imagens de fundo aplicadas por classes de background
- layout em grade e responsividade
- tipografia clássica e efeitos de hover
- estilos de botão e formulário.
