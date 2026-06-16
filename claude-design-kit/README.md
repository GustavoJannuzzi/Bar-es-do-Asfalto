# CLAUDE DESIGN KIT — BARÕES DO ASFALTO

Pasta autocontida para importar no **Claude Design** e gerar todo o material físico de impressão do RPG.

## Como usar

1. Importe esta pasta inteira no Claude Design
2. Cole o prompt que está em **`00-PROMPT-PARA-CLAUDE-DESIGN.md`**
3. Aprove componente a componente (a ordem de produção está no prompt)
4. Imprima seguindo as especificações de papel/formato do arquivo `02`

## Estrutura

```
claude-design-kit/
├── 00-PROMPT-PARA-CLAUDE-DESIGN.md   ← o prompt para colar
├── 01-DIRECAO-DE-ARTE.md             ← identidade visual (paleta, fontes, 25 bichos)
├── 02-COMPONENTES-E-ESPECIFICACOES.md← inventário + medidas de impressão
└── conteudo/
    ├── regras-essenciais.md          ← sistema canônico (pool d6) + cartão de referência
    ├── animais-do-bicho.md           ← tabela dos 25 bichos + pôster A3
    ├── tabuleiro-mapa.md             ← as 10 regiões, conexões e layout do tabuleiro A2
    ├── ficha-personagem.md           ← conteúdo da ficha A4 frente/verso (2 folhas)
    ├── arquetipos.md                 ← 9 cartas de arquétipo A5
    ├── cartas-favor.md               ← baralho de 40 favores + caderneta da sociedade
    ├── fichas-ponto.md               ← 16 cartas de ponto prontas + em branco
    ├── escudo-do-mestre.md           ← 4 painéis + livro rápido (inclui missão 1 pronta)
    └── marcadores-e-tokens.md        ← dinheiro, réguas de métricas, tokens
```

## Decisões canônicas embutidas no kit

- **Sistema único:** pool de d6 (documentos 5.1/6.1/6.2/7.1 do livro usam um sistema 2d10 antigo — o kit já traz a conversão; ver `REVISAO-E-INCONSISTENCIAS.md` na raiz do projeto)
- **Tabela de lavagem canônica:** a do doc 7.1 (taxas 10-28%)
- **Heat de combate:** tabela única reconciliada (máx. +5)
- O kit também preenche lacunas do livro: tabela de eventos econômicos 1d20, regra de vendetta e a primeira missão ("O Ponto de Madureira")
