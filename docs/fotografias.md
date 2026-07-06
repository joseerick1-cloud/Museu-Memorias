# fotografias.html

Este arquivo documenta a página de fotografias do acervo. Ele detalha o HTML e as classes CSS usadas para exibir imagens históricas.

## Estrutura HTML

- `<header class="main-header">` mantém a navegação consistente com o resto do site.
- `<section class="hero-section">` cria o banner de título da página.
- `<div class="tabs-container">` destaca a aba ativa de fotografias.
- `<section class="gallery-grid">` organiza as fotografias em cards.
- Cada `.grid-item` contém a imagem, o título, a data e a fonte.
- A sidebar usa `.featured-card` para promover uma coleção de destaque.

## Código principal

```html
<section class="gallery-grid">
  <div class="grid-item">
    <div class="img-wrapper placeholder-1"></div>
    <h3>Estação Ferroviária</h3>
    <span class="meta">Fotografia, 1928</span>
    <span class="credit">Coleção Família Andrade</span>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-2"></div>
    <h3>Desfile Cívico</h3>
    <span class="meta">Fotografia, 1946</span>
    <span class="credit">Arquivo Municipal</span>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-5"></div>
    <h3>Trabalhadores da Fábrica</h3>
    <span class="meta">Fotografia, 1954</span>
    <span class="credit">Doação de Helena Reis</span>
  </div>
</section>
```

## Classes CSS usadas

- `.hero-section`: banner de topo com imagem de fundo e texto central.
- `.hero-content`: título e decorador do hero.
- `.tabs-container`: linhas de navegação como botões de categoria.
- `.tab-btn.active`: indica que a aba de fotografias está selecionada.
- `.gallery-grid`: grade responsiva que acomoda múltiplos cartões.
- `.grid-item`: cada item representa uma fotografia do acervo.
- `.img-wrapper`: placeholder visual com filtro sépia.
- `.placeholder-1`, `.placeholder-2`, `.placeholder-5`, `.placeholder-6`, `.placeholder-bridge`, `.expo-img-1`: classes que aplicam imagens distintas.
- `.meta`, `.credit`: etiquetas de data e crédito para cada registro.
- `.featured-card`: card lateral com coleção em destaque.

## Relação com `styles.css`

O estilo da página de fotografias utiliza os padrões de grid e placeholders de `styles.css`, além de tipografia clara e efeitos de hover em `.grid-item h3`. A imagem não está em tags `<img>`; ela é aplicada no CSS com `background-image` nas classes de placeholder.
