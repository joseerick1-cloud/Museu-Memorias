# documentos.html

Este arquivo documenta a página de documentos históricos. Ele explica o HTML e as classes CSS usadas para organizar registros escritos e visuais.

## Estrutura HTML

- `<header class="main-header">` mantém o padrão de navegação do site.
- `<section class="hero-section">` exibe o título da página com banner temático.
- `<div class="tabs-container">` mostra o filtro ativo de documentos.
- `<section class="gallery-grid">` agrupa os documentos em cards de visualização.
- `<aside class="sidebar">` traz coleção em destaque e chamada à ação.
- `<footer class="main-footer">` informa horário, endereço e apoio.

## Código principal

```html
<section class="gallery-grid">
  <div class="grid-item">
    <div class="img-wrapper placeholder-4"></div>
    <h3>Carta de Imigrante</h3>
    <span class="meta">Correspondência, 1908</span>
    <span class="credit">Coleção Família Bianchi</span>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-2"></div>
    <h3>Programa de Festa Cívica</h3>
    <span class="meta">Impresso, 1946</span>
    <span class="credit">Arquivo Municipal</span>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-bridge"></div>
    <h3>Projeto da Ponte Velha</h3>
    <span class="meta">Planta técnica, 1932</span>
    <span class="credit">Fundo Obras Públicas</span>
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
      <div class="featured-img placeholder-4"></div>
      <h3>Cartas e registros públicos</h3>
      <p>Documentos pessoais, mapas, projetos e impressos que preservam decisões, trajetos e lembranças da cidade.</p>
      <a href="documentos.html" class="btn-view">Ver coleção <span class="arrow">→</span></a>
    </div>
  </div>
</aside>
```

## Classes CSS usadas

- `.hero-section`: banner de topo com imagem de fundo.
- `.tabs-container` e `.tab-btn.active`: criam a navegação de categoria.
- `.gallery-grid`: grade responsiva de cards.
- `.grid-item`: cada documento é apresentado em um cartão.
- `.img-wrapper`: placeholder visual que recebe imagem de fundo.
- `.placeholder-4`, `.placeholder-2`, `.placeholder-bridge`, `.placeholder-1`, `.placeholder-6`, `.expo-img-2`: classes de imagem específicas.
- `.meta` e `.credit`: legendas de data e origem.
- `.featured-card`, `.featured-header`, `.featured-body`: card lateral de destaque.
- `.btn-view`: botão de ação para ver a coleção.

## Relação com `styles.css`

Essa página utiliza os mesmos estilos de acervo para manter consistência visual. O CSS aplica texturas, filtros sépia e comportamento responsivo sem inserir imagens na marcação HTML.
