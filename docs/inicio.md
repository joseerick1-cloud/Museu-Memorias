# inicio.html

Este arquivo é a página inicial de `Museu Memórias`. Ele combina HTML semântico e classes CSS para criar a primeira impressão visual do site.

## Estrutura HTML

- `<header class="main-header">` contém a marca e a navegação principal.
- `<section class="hero-home">` é o banner principal da home, com imagem de fundo carregada pelo CSS.
- `<main class="main-container">` organiza o conteúdo em duas seções: a exposição em cartaz e o atalho para o acervo.
- `<footer class="main-footer">` exibe informações de horário, endereço, preço e apoio.

## Código principal

```html
<header class="main-header">
  <div class="header-inner">
    <div class="logo"><a href="inicio.html">Museu Memórias</a></div>
    <nav class="nav-menu">
      <a href="index.html" class="active">INÍCIO</a>
      <a href="acervo.html">ACERVO</a>
      <a href="historia-oral.html">HISTÓRIA ORAL</a>
      <a href="#">VISITE</a>
      <a href="#">SOBRE</a>
      <a href="#">CONTATO</a>
    </nav>
    <div class="header-icon">...</div>
  </div>
</header>
```

```html
<section class="hero-home">
  <div class="hero-overlay"></div>
  <div class="hero-content-home">
    <p class="pre-title">BEM-VINDO AO</p>
    <h1>Museu Memórias</h1>
    <p class="hero-desc">Preservando o passado para iluminar o futuro da nossa cidade.</p>
    <div class="hero-buttons">
      <a href="#exposicoes" class="btn-solid">Ver Exposições</a>
      <a href="acervo.html" class="btn-outline-gold">Explorar Acervo</a>
    </div>
  </div>
</section>
```

```html
<section class="acervo-shortcut">
  <div class="shortcut-content">
    <h2>O Acervo Digital</h2>
    <p>Milhares de fotografias, documentos e objetos catalogados para pesquisa e apreciação pública.</p>
    <a href="acervo.html" class="btn-burgundy">Acesse a Coleção Completa</a>
  </div>
</section>
```

## Classes CSS usadas

- `.main-header`: cabeçalho escuro com borda dourada, alinhamento flexível e menu de navegação.
- `.hero-home`: define a imagem de fundo, altura e centraliza o conteúdo.
- `.hero-overlay`: camada escura sobre a imagem do banner para boa legibilidade.
- `.hero-content-home`: posiciona o texto e aplica tipografia clara.
- `.pre-title`, `.hero-desc`, `.hero-buttons`: adicionam estilo ao texto e aos botões.
- `.btn-solid`, `.btn-outline-gold`, `.btn-burgundy`: criam botões com visual diferenciado.
- `.acervo-shortcut`: painel escuro de acesso rápido ao acervo.
- `.main-footer`, `.footer-grid`, `.footer-col`: estruturam as informações do rodapé em colunas.

## Relação com `styles.css`

O arquivo CSS define as imagens de fundo, a paleta de cores, o espaçamento e o layout responsivo dessa página. A home depende de estilos globais para o texto e do `hero-home` para imprimir a imagem e o estilo inicial do site.
