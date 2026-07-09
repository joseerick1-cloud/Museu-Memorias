# Museu Memórias

Site estático educativo recriado do zero para apresentar um museu fictício de memória local.

## Páginas

- `index.html` — entrada para GitHub Pages, redirecionando para `inicio.html`.
- `inicio.html` — apresentação do museu, destaques e atalhos principais.
- `exposicao.html` — exposição "Caminhos da Memória", peças selecionadas e tabela de programação.
- `visita.html` — informações de visitação e formulário completo de agendamento/contribuição.
- `styles.css` — folha autoral com tokens, layout responsivo e estados de interação.

## Arquitetura da informação

1. Início
   - Identidade do museu
   - Imagem histórica creditada
   - Resumo do projeto
   - Destaques do acervo
2. Exposição
   - Texto curatorial
   - Galeria de peças selecionadas
   - Links internos por seção
   - Tabela semântica de programação
3. Visita
   - Orientações para grupos
   - Horários
   - Formulário com validações nativas

## Wireframes textuais

### Mobile

```text
[Header / menu Bootstrap]
[Hero: título + botões]
[Imagem com legenda]
[Texto principal]
[Painel lateral abaixo]
[Cards em uma coluna]
[Footer]
```

### Desktop

```text
[Header horizontal]
[Hero: texto | imagem]
[Conteúdo principal | aside]
[Cards em grid]
[Tabela responsiva]
[Footer em três colunas]
```

## Guia visual

- Cores principais:
  - `--color-primary: #8f2f3f`
  - `--color-green: #2f6b57`
  - `--color-paper: #f7f3ea`
  - `--color-ink: #1f2933`
- Tipografia:
  - Títulos: Georgia, com aparência institucional.
  - Texto: system-ui, priorizando legibilidade.
- Espaçamentos:
  - Escala definida em variáveis `--space-1` até `--space-6`.
- Componentes:
  - Cards com borda discreta.
  - Botões Bootstrap customizados por CSS.
  - Painéis laterais com `aside`.

## Requisitos atendidos

- Três páginas HTML interligadas: `inicio.html`, `exposicao.html` e `visita.html`.
- Estrutura HTML5 completa com `header`, `nav`, `main`, `section`, `article`, `aside` e `footer`.
- Títulos em ordem lógica, listas, links internos, links externos e navegação por teclado.
- Imagens com `alt`, `width`, `height`, crédito/licença e uso de `figure`/`figcaption`.
- Uso de `loading="lazy"` nas imagens de conteúdo.
- Estratégia responsiva com `picture`, `source`, `srcset` e `sizes` equivalentes via mídia.
- Tabela semântica em `exposicao.html` com `caption`, `thead`, `tbody`, `th` e `scope`.
- Formulário em `visita.html` com `label`, `fieldset`, `legend`, `required`, `autocomplete`, tipos adequados e validações nativas.
- CSS autoral com cascata, herança, especificidade, combinadores, box model, display, cores, fundos, bordas, tipografia e unidades relativas.
- Flexbox nos grupos de botões e escolhas do formulário.
- CSS Grid em grids de cards, áreas de conteúdo e rodapé.
- Abordagem mobile-first, viewport configurado, imagens fluidas e media queries em `42rem`, `62rem` e `78rem`.
- Pseudoclasses `:hover`, `:focus-visible`, `:checked`, `:valid` e `:invalid`.
- Pseudoelementos `::before`, `::after` e `::marker`.
- Transições discretas em links e botões.
- Design tokens em `:root`.

## Uso do Bootstrap

Bootstrap foi usado em parte relevante da interface:

- Navbar responsiva com botão expansível.
- Classes de container, botões e tabela responsiva.
- Script `bootstrap.bundle.min.js` para o menu mobile.

Permaneceu autoral:

- Paleta, tokens, tipografia, cards, hero, grids, formulário, estados visuais e responsividade fina.

Motivo: Bootstrap resolve padrões comuns de navegação e componentes acessíveis, enquanto o CSS autoral demonstra domínio dos requisitos da disciplina e cria uma identidade visual própria.

## Imagens e créditos

As imagens são carregadas de Wikimedia Commons via `Special:FilePath` e indicadas como domínio público nos créditos junto ao conteúdo.

- `Brazil 16thc map.jpg` — Wikimedia Commons, domínio público.
- `DpedroI-brasil-full.jpg` — Wikimedia Commons, domínio público.
- `Pedro Américo - Independência ou Morte - Google Art Project.jpg` — Wikimedia Commons, domínio público.

## Testes recomendados

- Abrir `inicio.html`, `exposicao.html` e `visita.html` no navegador.
- Testar larguras mobile, tablet e desktop no DevTools.
- Navegar usando apenas teclado: `Tab`, `Shift + Tab` e `Enter`.
- Conferir validações do formulário enviando campos vazios ou inválidos.
- Verificar se textos não estouram os cards e se a tabela rola em telas pequenas.

## Publicação

Para publicar no GitHub Pages:

1. Enviar os commits para `main`.
2. No GitHub, abrir Settings > Pages.
3. Selecionar Deploy from a branch.
4. Escolher branch `main` e pasta `/root`.

O projeto já possui `index.html`, então o GitHub Pages encontrará a página inicial automaticamente.
