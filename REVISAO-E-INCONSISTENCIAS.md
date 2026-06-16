# REVISÃO COMPLETA — BARÕES DO ASFALTO
## Relatório de inconsistências e melhorias

> Gerado em 12/06/2026 após leitura integral dos documentos do sistema.
> Severidade: 🔴 Crítico (quebra o jogo na mesa) | 🟡 Importante (confunde, mas contornável) | 🟢 Polimento

---

## ✅ STATUS DE CORREÇÃO (aplicado em 15/06/2026)

As correções de inconsistência foram **aplicadas diretamente nos documentos**. Resumo do que mudou:

| Item | Status | O que foi feito |
|------|--------|-----------------|
| **1. Dois sistemas de dados** | ✅ Resolvido | 5.1, 6.1, 6.2 e 7.1 convertidos para o **pool de d6**. Combate virou teste contestado; gravidade = margem + bônus de arma; detecção de lavagem virou 1d6. |
| **2. Perícias fantasma** | ✅ Resolvido | Esquiva→Instinto+Fuga · Atletismo→Fuga · Briga→Combate Corpo a Corpo · Primeiros Socorros→Medicina de Rua · "Crimes"→Ocultação · Percepção→Instinto puro · Persuasão→Negociação. Nota explicativa adicionada em 1.2. |
| **3. Conteúdo faltando** | ✅ Resolvido | Tabela de eventos econômicos 1d20 criada em 4.1. **Escritos:** 8.2 (banco de ~32 NPCs), 9.1 (Guia de Condução), 9.2 (Campanhas e Arcos), 10.1 (10 missões iniciais) e 10.2 (10 missões avançadas). Vendetta definida no 9.1. |
| **4. Lavagem 4.1 × 7.1** | ✅ Resolvido | 4.1 alinhado à tabela canônica do 7.1 (taxas 10-28%); 1.1 atualizado. |
| **5. Heat/Pressão conflitantes** | ✅ Resolvido | Tabela única de Heat (teto +5) em 6.1; Pressão alinhada à escala do 1.1 com regra de Colapso. |
| **6. Fichas/arquétipos fora das regras** | ✅ Resolvido | Exemplos do 1.2 corrigidos para 15 pts; Articulador Instinto 1; Atravessador sem "Operação" como perícia; Contatos 5 do Informante documentado como exceção; Fundo Eleitoral classificado. |
| **7. Numeração do 4.2** | ✅ Resolvido | 16 pontos renumerados de forma única (#01-#16); análise duplicada e header vazio removidos; ficha do #04 (que estava escondida sob "Análise") recuperada. |
| **8. Lixo de geração** | ✅ Resolvido | Rodapé de conversa de IA removido do fim do 3.1; grau "Crítico" de favor citado no 1.1. |

> As menções a "2d10" / "d100" que ainda aparecem **neste arquivo** e nos arquivos do `claude-design-kit/` são intencionais — explicam a conversão. Nenhum documento de regra do jogo usa mais o sistema antigo.

---

## 1. 🔴 DOIS SISTEMAS DE DADOS DIFERENTES CONVIVEM NO LIVRO

**Este é o problema mais grave do projeto.** Metade dos documentos usa um sistema, metade usa outro:

| Sistema | Documentos | Como funciona |
|---|---|---|
| **Pool de d6** (o canônico) | 1.1 Regras, 1.2 Atributos, 2.1 Arquétipos, 2.2 Ficha, 4.1 Economia | Atributo (1-5) + Perícia (0-5) dados; 5-6 = sucesso; 6 explode; dificuldade = 1 a 5 sucessos |
| **2d10 + bônus** (incompatível) | 5.1 Favores, 6.1 Combate, 6.2 Segurança, 7.1 Lavagem | 2d10 + Atributo + Perícia vs dificuldade 10-22; o 7.1 ainda usa **1d100** para detecção |

Evidências:
- 6.1: "INICIATIVA: 2d10 + Instinto + Sangue Frio", dificuldades 10-22, exemplos com **Instinto 6 e Lábia 6** (a escala oficial vai só até 5) e "Capital de Rua 8" dando +2 fixo.
- 5.1: "Rolagem: 2d10 + LÁBIA + CONTATOS... Dificuldade 16".
- 6.2: teste de lealdade "2d10 + Lealdade vs dificuldade 16".
- 7.1: "Teste: LÁBIA + Persuasão, Dificuldade: 10-18" e rolagens de 1d100 para detecção.

**Correção sugerida:** converter tudo para o pool de d6 com esta régua:
- Dificuldade 10-12 → 2 sucessos | 13-15 → 3 | 16-18 → 4 | 19+ → 5
- "2d10 + X vs 2d10 + Y" → teste contestado de pools (regra já existe no 1.1)
- d100 de detecção → rolar 1d6 ao lavar: 1 = complicação (1-2 se acima de 80% da capacidade)

---

## 2. 🔴 PERÍCIAS QUE NÃO EXISTEM NA LISTA OFICIAL

A lista oficial (1.2) tem 22 perícias. Vários documentos testam perícias inexistentes:

| Perícia fantasma | Onde aparece | Equivalente oficial |
|---|---|---|
| Esquiva | 6.1 (defesa em combate) | criar regra: defesa = Instinto + Fuga |
| Atletismo | 6.1 (fuga a pé) | Fuga |
| Briga | 6.1 (corpo a corpo) | Combate Corpo a Corpo |
| Primeiros Socorros | 6.1 (estancar hemorragia) | Medicina de Rua |
| "Crimes" | 6.1 (limpar cena) | Ocultação |
| Percepção | 1.1 e 6.1 (vários exemplos "Instinto + Percepção") | não existe — criar a perícia OU padronizar teste puro de Instinto |
| Manipulação | 1.2 (exemplo da Lábia) | Mentira ou Negociação |
| Persuasão | 7.1 (recrutar laranja) | Negociação |

**Decisão necessária:** ou cria-se "Percepção" como 23ª perícia (é usada demais nos exemplos), ou se padroniza tudo para Leitura de Intenções / teste puro de Instinto.

---

## 3. 🔴 CONTEÚDO FALTANDO (prometido e não entregue)

1. **`8.2 NPCs Recorrentes.md` está VAZIO (0 KB)** — o README promete banco de 30-50 NPCs.
2. **`9.1 Guia de Condução.md` está VAZIO (0 KB)** — o Livro do Mestre não existe.
3. **Categoria 9.2 (Campanhas e Arcos) não existe** — nem o arquivo foi criado.
4. **Categoria 10 inteira (Missões Iniciais e Avançadas) não existe** — as 20 missões prometidas.
5. **4.1, seção 7 "Eventos Econômicos":** o título está cortado no meio da frase ("Role 1d20 no início de cada mês") e **a tabela de 15-20 eventos não existe**. (O 8.1 tem uma tabela 1d20 de eventos de facção, mas não cobre economia.)
6. **"Mecânica de vendetta"** é citada no 1.1 ("Mortes geram vingança — mecânica de vendetta") mas nunca é definida em lugar nenhum.

> O kit de design (pasta `claude-design-kit/`) já preenche parte disso: criei a tabela de eventos econômicos 1d20 e o conteúdo do Livro Rápido do Mestre.

---

## 4. 🔴 ECONOMIA DA LAVAGEM: 4.1 E 7.1 SE CONTRADIZEM

Os mesmos tipos de empresa têm números diferentes nos dois documentos:

| Empresa | 4.1 (taxa / capacidade / custo mensal) | 7.1 (taxa / capacidade / custo mensal) |
|---|---|---|
| Lava-jato/pequeno comércio | 35% / 30-50k / 4k | 28% / 15-40k / 4,5k |
| Construtora pequena | 30% / 100-200k / 10k | 18% / 150-400k / 18k |
| Importadora | 25% / 300-600k / 20k | 15% / 300k-1M / 25k |
| Offshore | 20% / ilimitada / 40k+ (invest. 500k-1M) | 10-12% / 500k-5M / 15k (invest. 300-500k) |

Outras divergências:
- **Limite de uso de dinheiro sujo:** 4.1 diz R$ 10.000; 7.1 diz que acima de R$ 2.000 já há risco.
- **Laranjas:** 4.1 cobra R$ 1.500-3.000/mês; 7.1 escalona de R$ 200 a R$ 5.000+ por perfil.
- 1.1 resume lavagem como "perde 20-40%", compatível com 4.1 mas não com 7.1 (que chega a 10%).

**Sugestão:** adotar a tabela do **7.1 como canônica** (é mais granular e mais bem desenhada — taxa cai conforme sofisticação sobe, o que cria progressão de jogo) e atualizar 4.1 e 1.1 para referenciá-la.

---

## 5. 🟡 HEAT E PRESSÃO COM ESCALAS CONFLITANTES

**Heat de combate:**
- 1.1 (tabela): tiroteio +1 a +3; matar policial +3 a +5.
- 1.1 (filosofia): "combate dá +2 a +4 automaticamente".
- 6.1: tiroteio em rua +4; com fuzil +6; matar policial **+10**; figura pública **+15** — estoura a escala, que é 0-10.

**Sugestão de tabela única (cabe na escala 0-10):** briga sem arma +1 · tiroteio discreto +1 · tiroteio público +2 · fuzil/rajada +3 · morte de civil +3 · morte de policial +4 · figura pública +5.

**Pressão (efeitos):**
- 1.1: 3-4 Tenso (-1 Sangue Frio) / 5-6 (-1 SF e Instinto) / 7-8 (-2 testes mentais) / 9-10 (-3 tudo).
- 6.1: 3-5 (-1 SF) / 6-8 (-2 SF, -1 tudo) / 9-10 (-3 SF, -2 tudo).
Escolher uma (recomendo a do 1.1, que tem a regra de Colapso associada).

---

## 6. 🟡 FICHAS DE EXEMPLO E ARQUÉTIPOS VIOLAM AS PRÓPRIAS REGRAS

Regra de criação: 15 pontos de atributo (mín. 1, máx. 4) e 20 de perícia (máx. 3).

| Personagem | Problema |
|---|---|
| 1.2, Exemplo 2 "Operador de Elite" | atributos somam **17** (2+2+4+4+2+3) |
| 1.2, Exemplo 3 "Articulador" | atributos somam **17** (3+4+2+2+4+2) |
| 2.1, Articulador do Morro | **Instinto 0** (mínimo é 1) |
| 2.1, Informante Profissional | **Contatos 5** (máximo inicial é 4) — se for exceção da vantagem, documentar |
| 2.1, Atravessador | lista "**Operação: 2**" entre as perícias — Operação é atributo |

Outros pontos de criação:
- Regra diz contatos iniciais = Contatos × 3, mas todos os arquétipos entregam 5 fixos (Político tem Contatos 4 → deveria ter 12). Esclarecer que os 5 são os "principais" e o jogador define o resto.
- Herdeiro começa com Heat 3; a criação diz Heat 0-2 (documentar como exceção da desvantagem).
- README e 00 prometem **8 arquétipos; existem 9** (o Herdeiro Relutante foi adicionado — bom conteúdo, só atualizar os índices).

---

## 7. 🟡 BAGUNÇA ESTRUTURAL NO 4.2 (Fichas de Pontos)

- Numeração duplicada/conflitante: `#1 Barraca do Seu Milton`, `#2 Bar do Neguinho`, depois recomeça `#02 Barraca da Central`, `#03 Salão Glamour`...
- **Não existe ponto #04**; o "Ponto Táxi" aparece sem número no meio do arquivo e o cabeçalho `#11 PONTO TAXI` (linha ~2753) está **vazio**.
- A seção "ANÁLISE COMPARATIVA DOS 15 PONTOS" aparece **duas vezes** (linhas ~1620 e ~2757).
- Na prática há 16 fichas para "15 pontos". Renumerar de 01 a 16 e manter uma única análise comparativa.

---

## 8. 🟢 LIXO DE GERAÇÃO E POLIMENTO

- **3.1 (Mapa):** o final do arquivo tem sobra de conversa de IA ("## Concluído... Pronto! Concluí as 3 regiões finais...") dizendo que Baixada e Complexos foram "pulados" — **mas as 10 regiões existem no arquivo**. Apagar esse rodapé.
- **Graduação de resultado (1.1):** sucesso parcial = dificuldade -1, sucesso total = dificuldade, crítico = dificuldade +2. O caso "dificuldade +1" ficou sem nome (na prática é sucesso total; explicitar).
- **Falha crítica** ("0 sucessos + metade dos dados em 1") fica quase impossível com pools grandes (8+ dados). Alternativa mais elegante: "0 sucessos e mais 1s do que qualquer outro número".
- **Colapso (Pressão 10):** 2/3 dos resultados removem o personagem do jogo permanentemente. Sugestão: dar uma rota de retorno (ex.: fuga = volta após 1 arco, com complicações).
- **Favores:** 1.1 dá +1/+2/+3 dados por favor pequeno/médio/grande; 5.1 adiciona o grau "Crítico" e os pontos de débito (1/3/6/10). Compatíveis, mas o 1.1 precisa citar o grau Crítico e os pontos de débito.
- **Tipos de segurança:** 4.1 usa Básico/Armado/Ex-PM/Elite/Chefe; 6.2 usa Básico/Experiente/Ex-policial/Capanga/Elite. Unificar nomenclatura e preços.
- **"Fundo Eleitoral" do Político** (R$ 100k "pode usar pra qualquer coisa") não se encaixa nas 3 categorias de dinheiro. Classificar (sugestão: dinheiro sujo com lavagem "grátis" limitada a usos de campanha).

---

## 9. MELHORIAS RECOMENDADAS (visão de design de jogo)

1. **Eleger o pool de d6 como sistema único** e converter 5.1/6.1/6.2/7.1 (régua de conversão na seção 1). O conteúdo desses documentos é ótimo — só a matemática está errada.
2. **Criar um "Livro Básico" consolidado** de ~40 páginas como fonte canônica (o material atual é referência de mesa, não leitura sequencial). O kit de impressão já força essa consolidação.
3. **Fase Econômica em passos numerados** (coletar renda → pagar proteção → pagar equipe → decidir lavagem → investir → rolar evento 1d20). Hoje está descrita em prosa; na mesa vira confusão.
4. **Definir a vendetta:** sugestão — toda morte gera um marcador de vendetta com a facção/família da vítima; o mestre rola 1d6 por sessão: 1 = a vingança age.
5. **Escrever os documentos vazios** (8.2, 9.1) e a Categoria 10 — sem missões prontas, a primeira sessão exige muito do mestre.
6. **Balancear o App/Plataforma online** (4.2: ROI de 1,2 mês e lucro de R$ 100k/mês) — domina qualquer estratégia. Sugestão: exigir Tecnologia 3+, Exposição 8+ fixa e eventos de bloqueio judicial recorrentes.

---

## O QUE JÁ ESTÁ MUITO BOM (manter)

- A identidade do jogo: economia como motor, violência cara, favores como moeda social — coeso e original.
- 3.1 (Geografia): as 10 regiões com NPCs, custos e oportunidades são o coração do jogo e estão prontas para virar tabuleiro.
- 2.1 (Arquétipos): os 9 arquétipos com ganchos que convergem para a mesma premissa (sociedade dos 3 bicheiros) — excelente desenho de campanha.
- 5.1 (Favores): os 9 "banqueiros de favores" e os pontos de débito são a melhor mecânica social do sistema.
- 4.2: os 16 pontos prontos com análise comparativa dão início de campanha imediato.
