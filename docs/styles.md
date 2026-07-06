# styles.css

Este arquivo contém todo o CSS do projeto Museu Memórias. Ele define a aparência das páginas, o layout responsivo, as imagens de fundo e os componentes visuais.

## 1. Configuração global e variáveis

O CSS começa com um reset e variáveis de tema que são usadas em todo o site.

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --bg-header: #0e161d;
  --bg-timeline: #0d1e29;
  --bg-parchment: #e6dfcc;
  --bg-card: #ded5bf;
  --burgundy: #451119;
  --gold: #c3a267;
  --text-dark: #231f1a;
  --text-muted: #665d4e;
  --text-light: #f5f2eb;
  --site-max-width: 1440px;
  --site-padding: clamp(16px, 4vw, 80px);
}
```

## 2. Cabeçalho

O header usa `.main-header`, `.header-inner`, `.logo` e `.nav-menu` para criar a navegação principal.

```css
.main-header {
  background-color: var(--bg-header);
  padding: 24px 0;
  border-bottom: 2px solid var(--gold);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.25);
}

.nav-menu a {
  color: #929ba5;
  text-decoration: none;
  letter-spacing: 2px;
}

.nav-menu a.active,
.nav-menu a:hover {
  color: var(--gold);
  border-bottom: 1px solid var(--gold);
}
```

## 3. Hero Banners

As páginas usam `.hero-home`, `.hero-section` e `.hero-exposicao` para banners com imagens de fundo.

```css
.hero-home {
  height: 75vh;
  background-image: url('https://images.unsplash.com/photo-1706331004467-572aed0d1429?auto=format&fit=crop&q=80&w=1600');
}

.hero-exposicao {
  height: 360px;
  background-image: url('https://images.unsplash.com/photo-1697813586289-77bfd6b056a9?auto=format&fit=crop&q=80&w=1600');
}

.hero-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, rgba(14, 22, 29, 0.98) 30%, rgba(14, 22, 29, 0.75) 100%);
}
```

## 4. Layout e abas

- `.main-container`: centraliza o conteúdo.
- `.tabs-container`: container das abas de navegação.
- `.content-layout`: grid que separa conteúdo principal e sidebar.

```css
.main-container {
  max-width: var(--site-max-width);
  margin: 0 auto;
  padding: 50px var(--site-padding);
}

.tabs-container {
  display: flex;
  gap: 6px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.1);
}

.content-layout {
  display: grid;
  grid-template-columns: 3.2fr 1.3fr;
  gap: 60px;
}
```

## 5. Galerias e placeholders

A grade `.gallery-grid` exibe cards, e `.img-wrapper` aplica imagens de fundo aos lugares visuais.

```css
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(220px, 100%), 1fr));
  gap: 30px;
}

.img-wrapper {
  aspect-ratio: 16 / 10;
  background-color: #cbc0a5;
  background-size: cover;
  background-position: center;
  filter: sepia(0.6) contrast(0.95) brightness(0.9);
}

.placeholder-1 {
  background-image: url('https://images.unsplash.com/photo-1639412852143-fc3bf3fd7234?auto=format&fit=crop&q=80&w=900');
}

.oral-img-antonio {
  background-image: url('https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&q=80&w=900');
}
```

## 6. Componentes exclusivos de exposição

A página de exposição usa `.horizontal-gallery`, `.timeline-banner` e `.testimonial-section`.

```css
.horizontal-gallery {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.timeline-banner {
  background-color: var(--bg-timeline);
  border: 1px solid var(--gold);
  padding: 24px;
  color: white;
}

.testimonial-section {
  display: flex;
  gap: 24px;
  background: rgba(0, 0, 0, 0.02);
  border-left: 4px solid var(--burgundy);
}
```

## 7. Sidebar e formulário

- `.sidebar-box`, `.menu-box`, `.form-box`: caixas laterais.
- `.museum-form`, `.form-group`, `.form-row`: Formulário de agendamento.

```css
.sidebar-box {
  border: 1px solid #3a3226;
  background-color: var(--bg-card);
}

.museum-form input,
.museum-form textarea {
  border: 1px solid #5c523f;
  padding: 11px 14px;
}
```

## 8. Botões e ações

Os botões usam as classes `.btn-view`, `.btn-submit`, `.btn-solid`, `.btn-outline-gold`, `.btn-burgundy`.

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

## 9. Rodapé

- `.main-footer`, `.footer-inner`, `.footer-grid` e `.footer-col` organizam o final das páginas.

```css
.main-footer {
  background-color: var(--burgundy);
  color: rgba(255, 255, 255, 0.75);
  padding: 60px 0;
  border-top: 4px solid var(--gold);
}
```

## 10. Responsividade

As media queries ajustam o layout em telas menores para garantir boa leitura:
- colunas viram blocos
- o menu passa a centralizar
- o banner reduz a altura
- os cards ficam em uma coluna única

```css
@media (max-width: 850px) {
  .content-layout { grid-template-columns: 1fr; }
  .horizontal-gallery { grid-template-columns: repeat(2, 1fr); }
}
```

## Conclusão

O `styles.css` é o coração visual do site. Ele permite que todas as páginas HTML compartilhem cores, tipografia, efeitos de imagem e responsividade.
