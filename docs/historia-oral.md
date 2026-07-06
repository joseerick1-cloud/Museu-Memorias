# historia-oral.html

Este arquivo documenta a página de história oral. Ele explica o HTML e as classes CSS usadas para apresentar depoimentos e memórias pessoais.

## Estrutura HTML

- `<header class="main-header">` mantém a navegação do site.
- `<section class="hero-section">` cria o banner de topo com título.
- `<div class="tabs-container">` mostra a aba ativa de História oral.
- `<section class="gallery-grid">` organiza depoimentos em cards.
- `<aside class="sidebar">` destaca uma coleção de vozes.
- `<footer class="main-footer">` fecha a página com informações institucionais.

## Código principal

```html
<div class="grid-item">
  <div class="img-wrapper oral-img-luzia"></div>
  <h3>Dona Luzia</h3>
  <span class="meta">Entrevista, 24/03/2019</span>
  <span class="credit">Memórias da Feira Central</span>
</div>
<div class="grid-item">
  <div class="img-wrapper oral-img-antonio"></div>
  <h3>Seu Antônio</h3>
  <span class="meta">Entrevista, 12/08/2018</span>
  <span class="credit">Relatos do Bairro Operário</span>
</div>
```

```html
<div class="grid-item">
  <div class="img-wrapper expo-img-3"></div>
  <h3>Feirantes do Mercado</h3>
  <span class="meta">Entrevistas coletivas, 2020</span>
  <span class="credit">Acervo Caminhos da Feira</span>
</div>
```

## Classes CSS usadas

- `.hero-section`: banner superior com imagem de fundo padrão.
- `.tabs-container`: navegação de abas.
- `.gallery-grid`: grade de depoimentos.
- `.img-wrapper`: placeholder visual para imagens de depoimento.
- `.oral-img-luzia`, `.oral-img-antonio`: imagens de fundo específicas para entrevistas.
- `.expo-img-3`: imagem relacionada ao conteúdo da exposição.
- `.meta` e `.credit`: legendas de data e crédito.
- `.featured-card`, `.featured-header`, `.featured-body`: card de destaque lateral.

## Relação com `styles.css`

A página de história oral usa os mesmos estilos de grade e placeholders das outras páginas, com classes de imagem especializadas para os depoimentos. O CSS mantém a tipografia, cores e responsividade de forma consistente.
