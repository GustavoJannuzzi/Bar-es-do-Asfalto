# PROMPT PARA O CLAUDE DESIGN
## (copie e cole o texto abaixo da linha ao importar esta pasta)

---

Você vai criar o **kit físico completo de impressão** do RPG de mesa **"BARÕES DO ASFALTO"** — um jogo brasileiro sobre o jogo do bicho e o crime organizado no Rio de Janeiro contemporâneo. Tudo será impresso em casa/gráfica e jogado fisicamente na mesa: nada é digital.

Esta pasta é o seu codebase de referência. Leia nesta ordem antes de desenhar qualquer coisa:

1. `01-DIRECAO-DE-ARTE.md` — identidade visual obrigatória (paleta, tipografia, texturas, os 25 bichos como sistema de ícones)
2. `02-COMPONENTES-E-ESPECIFICACOES.md` — a lista de tudo que deve ser gerado, com formatos e medidas de impressão
3. A pasta `conteudo/` — o texto e os dados reais de cada componente (regras, regiões do tabuleiro, arquétipos, cartas, tabelas do mestre)

## O que você deve produzir

Gere cada componente como **página HTML/CSS pronta para impressão** (uma página ou conjunto de páginas por componente), seguindo rigorosamente:

- Dimensões físicas exatas definidas no arquivo 02 (use `@page` com tamanho e margens; medidas em `mm`; sangria de 3mm onde indicado)
- Tipografia e cores da direção de arte (carregue as fontes do Google Fonts indicadas)
- Densidade de tinta consciente: fundos escuros só onde indicado (escudo do mestre e cartas); fichas que serão preenchidas a lápis têm fundo claro
- Todo texto em **português do Brasil**, com a voz do jogo: seca, urbana, sem glorificar crime

## Ordem de produção (priorize assim)

1. **Ficha de Personagem** (A4 frente/verso) — `conteudo/ficha-personagem.md`
2. **Tabuleiro do Rio** (A2 montável em 4×A4 com marcas de corte/junção) — `conteudo/tabuleiro-mapa.md`
3. **Escudo do Mestre** (4 painéis A4 paisagem) + **Livro Rápido do Mestre** (booklet A5) — `conteudo/escudo-do-mestre.md`
4. **Baralho de Favores** (40 cartas poker 63,5×88,9mm, frente+verso) — `conteudo/cartas-favor.md`
5. **Cartas de Ponto de Bicho** (16 prontas + 4 em branco, tamanho tarot 70×120mm) — `conteudo/fichas-ponto.md`
6. **Cartas de Arquétipo** (9 cartas A5) — `conteudo/arquetipos.md`
7. **Dinheiro do jogo** (notas "limpo" e "sujo", 6 valores, 9 notas por A4) — `conteudo/marcadores-e-tokens.md`
8. **Trilhas e marcadores** (réguas de Heat/Pressão/Exposição/Capital de Rua com clipes, tokens dos 25 bichos) — `conteudo/marcadores-e-tokens.md`
9. **Cartão de Referência Rápida do jogador** (A5 frente/verso) — `conteudo/regras-essenciais.md`
10. **Pôster dos 25 Bichos** (A3) — `conteudo/animais-do-bicho.md`

## Regras inegociáveis

- O sistema de jogo impresso é **somente o pool de d6** descrito em `conteudo/regras-essenciais.md` (dificuldades de 1 a 5 sucessos). Ignore qualquer menção a 2d10, d100 ou dificuldades 10-22 — são resquícios de uma versão antiga.
- Os 25 bichos do jogo do bicho são o DNA visual do projeto: use-os como ícones, marca d'água, numeração e ornamento em TODOS os componentes (a tabela oficial com dezenas está em `conteudo/animais-do-bicho.md`).
- O tabuleiro não é um mapa geográfico fiel — é um **mapa estilizado de territórios** (estética de diagrama de metrô + xilogravura), com as 10 regiões, suas conexões e os dados de jogo de cada uma.
- Material do mestre tem estética de **dossiê confidencial de investigação** (carimbos, papel timbrado, tarjas); material do jogador tem estética de **pule de bicho vintage** (bilhete de aposta, serrilhas, numeração tipográfica).
- Nunca use símbolos reais de facções criminosas. Use os símbolos abstratos definidos na direção de arte.

Comece pela Ficha de Personagem e me mostre antes de seguir para os próximos componentes.
