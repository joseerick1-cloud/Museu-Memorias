# Museu Memórias

Guia técnico do projeto completo. Este documento explica todos os arquivos do site e descreve o papel principal de cada elemento do CSS.

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

## 3. Descrição de cada arquivo HTML

### `inicio.html`
- Header com logo e menu de navegação
- Banner principal com imagem de fundo e texto de abertura
- Seções de destaque para atrair o visitante ao museu
- Funciona como a página de entrada do projeto

### `exposicao.html`
- Banner com imagem temática da exposição
- Texto introdutório sobre a mostra
- Galeria horizontal de itens relacionados
- Linha do tempo com eventos históricos
- Depoimento em destaque e sidebar com formulário
- Mostra a parte narrativa e informativa do museu

### `acervo.html`
- Lista de abas para filtrar tipos de conteúdo
- Grade de itens do acervo com imagem e título
- Sidebar com coleção em destaque
- Serve como catálogo geral do museu

### `fotografias.html`
- Layout similar ao acervo, mas focado em imagens
- Mostra registros visuais e históricos
- Destaca o valor das fotografias para contar memória

### `objetos.html`
- Página de objetos do acervo
- Itens históricos como máquinas, relógios e utensílios
- Mostra o valor do acervo material, não apenas visual

### `documentos.html`
- Página dedicada a documentos históricos
- Exibe cartas, listas e registros antigos
- Reforça a importância da documentação na memória coletiva

### `historia-oral.html`
- Página de depoimentos e entrevistas
- Inclui relatos pessoais e memórias orais
- Apresenta voz e experiência humana como elemento central

## 4. Explicação do `styles.css`

### 4.1. Variáveis e configuração global

O início do arquivo define variáveis para cores, fontes e espaçamento.

Exemplo:
```css
:root {
  --bg-header: #0e161d;
  --bg-parchment: #e6dfcc;
  --gold: #c3a267;
  --text-dark: #231f1a;
  --site-max-width: 1440px;
}
```

Também há regras de reset para remover margens e definir `box-sizing: border-box`.

### 4.2. Cabeçalho (`header`)

Classes principais:
- `.main-header` — define o fundo escuro e o bordo inferior dourado
- `.header-inner` — organiza logo, menu e ícone em linha
- `.logo` — estilo da marca do museu
- `.nav-menu` — links de navegação com hover e estado ativo

Essas regras criam a identidade institucional do site.

### 4.3. Hero sections e banners

Classes principais:
- `.hero-section`, `.hero-home`, `.hero-exposicao`
- `.hero-overlay`
- `.hero-content`, `.hero-content-expo`

Função:
- define imagens de fundo
- controla altura e posição
- aplica sobreposição escura para legibilidade
- formata títulos e texto principal

### 4.4. Layout de páginas

Classes principais:
- `.main-container` — centraliza o conteúdo e aplica espaçamento
- `.content-layout` — organiza conteúdo principal e sidebar em grade
- `.tabs-container`, `.tab-btn` — navegação interna para acervo/história

Essa área define como as páginas separam conteúdo e suporte lateral.

### 4.5. Grades, galerias e itens

Classes principais:
- `.gallery-grid`, `.gallery-item`, `.grid-item`
- `.img-wrapper`, `.mini-img`
- classes de imagem específicas: `.placeholder-1`, `.expo-img-1`, `.oral-img-luzia`, `.oral-img-antonio`

Função:
- cria cartões de imagem com título
- aplica estilo de fotografia histórica
- garante responsividade e alinhamento

Exemplo:
```css
.img-wrapper {
  aspect-ratio: 16 / 10;
  background-size: cover;
  filter: sepia(0.6) contrast(0.95);
}
```

### 4.6. Componentes especiais

Classes principais:
- `.featured-card` — card de destaque na sidebar
- `.timeline-banner`, `.timeline-node` — linha do tempo
- `.testimonial-section` — bloco de depoimento
- `.sidebar-box` — caixas laterais de informação e formulário

Esses blocos adicionam conteúdo extra e tornam o site mais completo.

### 4.7. Botões e interações

Classes principais:
- `.btn-view`, `.btn-solid`, `.btn-outline`, `.btn-solid-small`
- `.tab-btn.active`

Essas regras definem cores, bordas e transições para ações visuais.

### 4.8. Rodapé

Classes principais:
- `.main-footer`
- `.footer-grid`
- `.footer-col`
- `.support-col`

Função:
- organiza informações de horário, endereço e valores
- finaliza a página com estilo institucional

## 5. Como apresentar no GitHub

### 5.1. O que mostrar primeiro

- abra o `README.md`
- explique o propósito do site
- mostre a estrutura de arquivos

### 5.2. Como explicar o HTML

- cada arquivo HTML é uma página do museu
- use títulos e listas para descrever conteúdo
- mostre que `historia-oral.html` tem depoimentos e `acervo.html` tem catálogo

### 5.3. Como explicar o CSS

- descreva as variáveis como a base de cores e fontes
- explique o header como identidade institucional
- mostre as hero sections como a parte visual principal
- fale da grade e dos cards como organização de acervo

### 5.4. Exemplo rápido no GitHub

Explique assim:

> "O `styles.css` controla a identidade visual. Por exemplo, `.hero-exposicao` define a imagem de capa da exposição, e `.gallery-grid` organiza os itens do acervo em cartões." 

### 5.5. Finalização

Diga que o projeto combina:
- conteúdo histórico
- design visual consistente
- navegação clara
- apresentação pensada para web

## 6. Arquivos principais e suas funções

- `inicio.html`: entrada do projeto
- `exposicao.html`: apresentação do tema da mostra
- `acervo.html`: catálogo geral do acervo
- `fotografias.html`: coleção de imagens
- `objetos.html`: itens físicos do museu
- `documentos.html`: documentos históricos
- `historia-oral.html`: relatos orais e entrevistas
- `styles.css`: aparência, layout e efeitos visuais

## 7. Dica para a apresentação

Mostre o `README.md` primeiro e depois abra uma página HTML para exemplificar.
Assim você prova que o projeto é organizado e que o código tem intenção clara.


