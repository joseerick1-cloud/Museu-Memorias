# objetos.html

Este arquivo documenta a página de objetos do acervo. Ele descreve o HTML e as classes CSS usadas para exibir itens físicos com contexto histórico.

## Estrutura HTML

- `<header class="main-header">` com navegação do museu.
- `<section class="hero-section">` com o título da seção.
- `<div class="tabs-container">` para alternar entre categorias do acervo.
- `<section class="gallery-grid">` para exibir os objetos em cards.
- `<aside class="sidebar">` para destacar uma coleção relacionada.
- `<footer class="main-footer">` com informações de visita.

## Código principal

```html
<section class="gallery-grid">
  <div class="grid-item">
    <div class="img-wrapper placeholder-3"></div>
    <h3>Máquina de Costura</h3>
    <span class="meta">Objeto doméstico, c. 1930</span>
    <span class="credit">Doação de Maria Antunes</span>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-7"></div>
    <h3>Relógio de Bolso</h3>
    <span class="meta">Objeto pessoal, c. 1915</span>
    <span class="credit">Coleção Família Vieira</span>
  </div>
  <div class="grid-item">
    <div class="img-wrapper placeholder-4"></div>
    <h3>Balança de Mercado</h3>
    <span class="meta">Comércio local, c. 1940</span>
    <span class="credit">Acervo Caminhos da Feira</span>
  </div>
</section>
```

## Classes CSS usadas

- `.hero-section`: banner com imagem de fundo que padroniza todas as páginas internas.
- `.tabs-container`: barra de abas com links para as outras páginas.
- `.gallery-grid`: grade adaptável que organiza os objetos.
- `.grid-item`: cada bloque de objeto.
- `.img-wrapper`: placeholder de imagem com efeito antigo.
- `.placeholder-3`, `.placeholder-7`, `.placeholder-4`, `.placeholder-1`, `.placeholder-5`, `.placeholder-6`: cada classe define uma imagem de fundo diferente.
- `.meta` e `.credit`: exibem o tipo, ano e origem do objeto.
- `.featured-card`, `.featured-header`, `.featured-body`: card lateral de coleção em destaque.
- `.btn-view`: botão de chamada para ação.

## Relação com `styles.css`

A página de objetos se baseia em `styles.css` para aplicar o layout da grade, o estilo dos cards e o filtro sépia das imagens. A sidebar usa as mesmas classes de destaque das outras páginas do acervo.
