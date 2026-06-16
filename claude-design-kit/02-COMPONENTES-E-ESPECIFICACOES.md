# COMPONENTES DO KIT FÍSICO — ESPECIFICAÇÕES DE IMPRESSÃO

Para uma mesa de **1 mestre + 3-5 jogadores**. Tudo dimensionado para impressora doméstica A4 (com opção de gráfica nos itens marcados ★).

| # | Componente | Formato físico | Quantidade | Papel sugerido | Conteúdo em |
|---|---|---|---|---|---|
| 1 | Ficha de Personagem | A4 frente/verso (2 folhas = 4 páginas) | 1 por jogador + reservas | Sulfite 90g (preencher a lápis) | `conteudo/ficha-personagem.md` |
| 2 | Tabuleiro do Rio ★ | A2 (420×594mm) fatiado em 4×A4 com marcas de junção e sangria 3mm | 1 | Couché 170g ou A2 em gráfica | `conteudo/tabuleiro-mapa.md` |
| 3 | Escudo do Mestre | 4 painéis A4 paisagem (colar em papelão/pasta) | 1 | Couché 150g | `conteudo/escudo-do-mestre.md` |
| 4 | Livro Rápido do Mestre | Booklet A5 (A4 dobrado, 12-16 págs, imposição para grampo canoa) | 1 | Sulfite 90g | `conteudo/escudo-do-mestre.md` |
| 5 | Baralho de Favores | 40 cartas poker 63,5×88,9mm, 9 por A4, frente e verso | 40 | Couché 250g ★ ou sulfite + sleeve | `conteudo/cartas-favor.md` |
| 6 | Cartas de Ponto de Bicho | Tarot 70×120mm, 4 por A4 | 16 prontas + 4 em branco | Couché 250g | `conteudo/fichas-ponto.md` |
| 7 | Cartas de Arquétipo | A5 (2 por A4), frente/verso | 9 | Couché 200g | `conteudo/arquetipos.md` |
| 8 | Dinheiro do jogo | Notas 130×60mm, 9 por A4 | ~15 folhas | Sulfite 75g (verde p/ limpo, pode imprimir em papel reciclado p/ sujo) | `conteudo/marcadores-e-tokens.md` |
| 9 | Réguas de métricas | Tiras 210×40mm, 5 por A4 (usar clipe de papel como cursor) | 4 tiras por jogador | Couché 200g | `conteudo/marcadores-e-tokens.md` |
| 10 | Tokens de território | Círculos Ø25mm com os 25 bichos, 35 por A4 | 2 folhas por jogador (1 bicho escolhido) | Couché 250g + furador 25mm | `conteudo/marcadores-e-tokens.md` |
| 11 | Referência Rápida do Jogador | A5 frente/verso | 1 por jogador | Couché 200g (plastificar) | `conteudo/regras-essenciais.md` |
| 12 | Pôster dos 25 Bichos | A3 (ou 2×A4) | 1 | Couché 170g | `conteudo/animais-do-bicho.md` |
| 13 | Cartas de Evento Mensal | Poker 63,5×88,9mm | 20 econômicas + 9 de facção | Couché 250g | `conteudo/escudo-do-mestre.md` (tabelas viram cartas) |
| 14 | Ficha de Favores da Sociedade | A4 (registro compartilhado de dívidas do grupo) | 5 cópias | Sulfite 90g | `conteudo/cartas-favor.md` (seção final) |

## Regras técnicas para o Claude Design

- Cada componente = um arquivo HTML independente com CSS `@page { size: ...; margin: ... }` e medidas em **mm**
- Cartas e tabuleiro: **sangria de 3mm** + marcas de corte; linhas de corte tracejadas finas cinza 30%
- Frente e verso de cartas em páginas alternadas **espelhadas** (para impressão duplex pela borda longa)
- Fundos escuros apenas em: versos de carta, painéis do escudo, dinheiro. Fichas preenchíveis = fundo creme claro com campos em linha pontilhada
- Corpo de texto mínimo 7pt em cartas, 9pt em fichas
- Testar contraste: tudo precisa continuar legível impresso em preto-e-branco (impressora sem cor)

## Itens NÃO imprimíveis (lista de compras do jogador)

- ~12 dados d6 por jogador (pools chegam a 10+) — ideal: 1 cor por jogador
- Clipes de papel (cursores das réguas)
- Lápis e borracha
- Opcional: sleeves para as cartas, cubos coloridos de madeira para marcar pontos no tabuleiro
