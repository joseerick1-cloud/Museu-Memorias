# Museu Memórias

Guia técnico do projeto completo. Este documento explica cada arquivo do site, mostra trechos de código reais e descreve o papel principal dos elementos HTML e CSS.

## 1. Objetivo do projeto

O site apresenta um museu digital com páginas que exploram:
- início
- exposição em cartaz
- acervo
- fotografias
- objetos
- documentos
- história oral

A intenção é simular um site institucional com design histórico, navegação clara e conteúdo de memória.

## 2. Estrutura de arquivos

- `inicio.html` — página inicial do museu
- `exposicao.html` — página da exposição principal
- `acervo.html` — página geral do acervo
- `fotografias.html` — página com apenas fotografias
- `objetos.html` — página com objetos do acervo
- `documentos.html` — página com documentos históricos
- `historia-oral.html` — página de depoimentos e entrevistas
- `styles.css` — arquivo de estilo que controla todo o layout e visual
- `README.md` — documentação do projeto para apresentação

## 3. Explicação de cada arquivo HTML

### `inicio.html`

A home apresenta o museu, o banner principal e um atalho direto para o acervo.

Trecho principal:
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

Por que importa:
- é a entrada do site
- apresenta identidade visual
- direciona o visitante para as demais páginas

### `exposicao.html`

A página da exposição combina texto, galeria e depoimentos para contar a história principal.

Trecho principal:
```html
<section class="hero-exposicao">
  <div class="hero-overlay"></div>
  <div class="hero-content-expo">
    <h1>Caminhos da Feira</h1>
    <div class="decorator"><span>♦</span> <hr> <span>♦</span></div>
    <p class="hero-expo-desc">Uma exposição sobre os trajetos que conectaram pessoas, mercadorias e histórias...</p>
  </div>
</section>
```

Galeria de exemplo:
```html
<div class="horizontal-gallery">
  <div class="gallery-item">
    <div class="mini-img expo-img-1"></div>
    <h4>Feira Livre no Largo da Matriz</h4>
    <p class="meta">c. 1895 • Fotografia</p>
    <p class="credit">Acervo: Coleção José Ferreira</p>
  </div>
</div>
```

Depoimento:
```html
<div class="testimonial-section">
  <span class="large-quote">“</span>
  <div class="testimonial-card">
    <div class="author-photo"></div>
    <div class="testimonial-text">
      <p>"Minha mãe vinha ainda de madrugada..."</p>
      <span class="author-info">DONA LUZIA, 82 ANOS<br><em>Entrevista em 24/03/2019</em></span>
    </div>
  </div>
</div>
```

Por que importa:
- mostra o conteúdo narrativo principal
- usa layout misto de texto e imagem
- inclui linha do tempo e formulário

### `acervo.html`

A página do acervo organiza itens históricos em uma grade e mostra uma coleção em destaque.

Trecho principal:
```html
<div class="tabs-container">
  <a href="acervo.html" class="tab-btn active">Todos</a>
  <a href="fotografias.html" class="tab-btn">Fotografias</a>
  <a href="objetos.html" class="tab-btn">Objetos</a>
  <a href="documentos.html" class="tab-btn">Documentos</a>
  <a href="historia-oral.html" class="tab-btn">História oral</a>
</div>
```

Card de acervo:
```html
<div class="grid-item">
  <div class="img-wrapper placeholder-1"></div>
  <h3>Estação Ferroviária</h3>
</div>
```

Sidebar de destaque:
```html
<div class="featured-card">
  <div class="featured-header">
    <span>Coleção em destaque</span>
    <div class="card-decorator"></div>
  </div>
  <div class="featured-body">
    <div class="featured-img placeholder-featured"></div>
    <h3>Pontes que uniram histórias</h3>
    <p>Registros fotográficos e documentos sobre as pontes...</p>
    <a href="#" class="btn-view">Ver item <span class="arrow">→</span></a>
  </div>
</div>
```

Por que importa:
- serve como catálogo geral
- mostra navegação por categorias
- utiliza cards visuais de acervo

### `fotografias.html`

A página de fotografias enfatiza registros visuais e metadados.

Trecho principal:
```html
<div class="grid-item">
  <div class="img-wrapper placeholder-1"></div>
  <h3>Estação Ferroviária</h3>
  <span class="meta">Fotografia, 1928</span>
  <span class="credit">Coleção Família Andrade</span>
</div>
```

Por que importa:
- separa as fotografias do acervo geral
- mostra texto de data e crédito
- usa a mesma grade de cards para manter consistência

### `objetos.html`

A página de objetos apresenta peças físicas do Museu.

Trecho principal:
```html
<div class="grid-item">
  <div class="img-wrapper placeholder-3"></div>
  <h3>Máquina de Costura</h3>
  <span class="meta">Objeto doméstico, c. 1930</span>
  <span class="credit">Doação de Maria Antunes</span>
</div>
```

Por que importa:
- exibe itens materiais do acervo
- usa imagens de fundo em cards
- mantém o estilo do inventário

### `documentos.html`

A página de documentos foca em registros escritos e projetos antigos.

Trecho principal:
```html
<div class="grid-item">
  <div class="img-wrapper placeholder-4"></div>
  <h3>Carta de Imigrante</h3>
  <span class="meta">Correspondência, 1908</span>
  <span class="credit">Coleção Família Bianchi</span>
</div>
```

Por que importa:
- destaca documentos históricos
- reforça a importância da preservação escrita
- usa o mesmo padrão visual da galeria

### `historia-oral.html`

A página de história oral mostra depoimentos com imagens de entrevistados.

Trecho principal:
```html
<div class="grid-item">
  <div class="img-wrapper oral-img-antonio"></div>
  <h3>Seu Antônio</h3>
  <span class="meta">Entrevista, 12/08/2018</span>
  <span class="credit">Relatos do Bairro Operário</span>
</div>
```

Por que importa:
- apresenta conteúdo pessoal e narrativo
- conecta o visitante a histórias reais
- usa imagens e metadados para contextualizar cada relato

## 4. Explicação do `styles.css`

O arquivo CSS define a aparência de todas as páginas do projeto.

### 4.1. Variáveis e configuração global

Exemplo:
```css
:root {
  --bg-header: #0e161d;
  --bg-parchment: #e6dfcc;
  --bg-card: #ded5bf;
  --burgundy: #451119;
  --gold: #c3a267;
}
```

Também há reset global e estilo base para `body`.

### 4.2. Header e navegação

Exemplo:
```css
.main-header {
  background-color: var(--bg-header);
  border-bottom: 2px solid var(--gold);
}

.nav-menu a.active,
.nav-menu a:hover {
  color: var(--gold);
  border-bottom: 1px solid var(--gold);
}
```

### 4.3. Hero banners

Exemplo de hero:
```css
.hero-home {
  height: 75vh;
  background-image: url('https://images.unsplash.com/photo-1706331004467-572aed0d1429?...');
}

.hero-exposicao {
  height: 360px;
  background-image: url('https://images.unsplash.com/photo-1697813586289-77bfd6b056a9?...');
}
```

### 4.4. Layout de página

Contêiner principal:
```css
.main-container {
  max-width: var(--site-max-width);
  margin: 0 auto;
  padding: 50px var(--site-padding);
}

.content-layout {
  display: grid;
  grid-template-columns: 3.2fr 1.3fr;
  gap: 60px;
}
```

### 4.5. Grades e imagens de acervo

Exemplo:
```css
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(220px, 100%), 1fr));
  gap: 30px;
}

.img-wrapper {
  border: 1px solid rgba(0,0,0,0.08);
  background-size: cover;
  filter: sepia(0.6) contrast(0.95) brightness(0.9);
}
```

Classes de imagem:
```css
.placeholder-1 { background-image: url('...'); }
.expo-img-1 { background-image: url('...'); }
.oral-img-antonio { background-image: url('...'); }
```

### 4.6. Componentes especiais

Linha do tempo:
```css
.timeline-banner {
  background-color: var(--bg-timeline);
  border: 1px solid var(--gold);
  padding: 24px;
  color: white;
}
```

Depoimento:
```css
.testimonial-section {
  display: flex;
  gap: 24px;
  border-left: 4px solid var(--burgundy);
}
```

### 4.7. Botões

Exemplo:
```css
.btn-solid,
.btn-submit,
.btn-burgundy {
  background-color: var(--burgundy);
  color: var(--text-light);
}

.btn-outline-gold {
  border: 1px solid var(--gold);
  color: var(--gold);
}
```

### 4.8. Responsividade

Regras principais:
- `.content-layout` vira uma coluna única em telas menores
- `.horizontal-gallery` reduz para 2 colunas
- `.nav-menu` centraliza em dispositivos pequenos

Trecho:
```css
@media (max-width: 850px) {
  .content-layout { grid-template-columns: 1fr; }
  .horizontal-gallery { grid-template-columns: repeat(2, 1fr); }
}
```

## 5. Como usar este README

- `inicio.html`: leia a seção de introdução
- `exposicao.html`: veja o uso de galeria e depoimento
- `acervo.html`: entenda como o catálogo é construído
- `fotografias.html`, `objetos.html`, `documentos.html`, `historia-oral.html`: cada página tem seu foco e mantém o mesmo padrão visual
- `styles.css`: veja as regras que criam a identidade, as imagens e o layout responsivo

## 6. Resumo final

Este projeto usa HTML semântico e CSS unificado para criar um site institucional. Cada página apresenta um aspecto diferente do museu, e o `styles.css` garante que todos os elementos se comportem de forma consistente e elegante.


Mostre o `README.md` primeiro e depois abra uma página HTML para exemplificar.
Assim você prova que o projeto é organizado e que o código tem intenção clara.


