# Nota do CFO (leia primeiro)

**Como ler a tabela abaixo:** a ferramenta escreve "$" e "a day". Aqui, **$ = R$** e **"a day" = por mês** (usei 1 "dia" por mês, porque a unidade é um mandato fechado, não uma venda diária). Quase todos os números de entrada são **estimativas minhas**, marcadas em `founder/cfo-sources.md`. Troque pelos seus.

- **A margem:** cada mandato fechado (captação média estimada de R$ 3 mi, honorário de 2% = R$ 60 mil) deixa **R$ 41 mil (68%)** depois de impostos, comissão de indicação e custos da operação. No plano de 2 mandatos por mês, a margem de lucro é **54%**. O ponto de equilíbrio é **0,43 mandato por mês** (R$ 17.700 de custo fixo ÷ R$ 41.000), ou seja, um mandato a cada 2,3 meses paga a estrutura.
- **A linha a observar: quantos mandatos fecham, e quando.** O painel de compradores teve 4% de compra com a oferta antiga e 0% com a nova, por falta de prova. Se o ritmo for metade do plano, o lucro do ano 1 cai de R$ 238.600 para **R$ 13.100** e o dinheiro inicial não volta no ano 1 (`--volume 0.5`). Se o primeiro mandato só fechar no mês 6, o resultado é o mesmo: R$ 13.100 e **R$ 103.500 de caixa** necessário.
- **A segunda linha: o tamanho médio da captação.** Com captação média de R$ 1,5 mi (honorário de R$ 30 mil), o ano 1 dá **prejuízo de R$ 91.400** e o equilíbrio sobe para cerca de 1 mandato por mês (`--price 30000`). Por isso vale ter um honorário mínimo por operação.
- **Caixa:** no plano, você precisa de **R$ 68.100** antes do negócio se pagar (R$ 15 mil de abertura + 3 meses sem receita). No cenário lento, **R$ 103.500**. A entrada de R$ 7.500 ajuda pouco no caixa, porque é descontada do sucesso e devolvida se não houver proposta.

## Três formas de melhorar (testadas na ferramenta)

| Mudança | O que muda | Lucro do ano 1 | Caixa necessário |
|---|---|---:|---:|
| Base | — | R$ 238.600 | R$ 68.100 |
| Pró-labore de R$ 6 mil (em vez de R$ 12 mil) até o primeiro mandato | custo fixo cai para R$ 11.700 | R$ 310.600 | **R$ 50.100** |
| Honorário mínimo que eleve a média para R$ 66 mil por mandato | preço +10% | R$ 304.600 | R$ 68.100 |
| Comissão de indicação de 5% (em vez de 10%) | contribuição sobe para R$ 44 mil (73%) | R$ 271.600 | R$ 68.100 |

## Condições do conselho sobre dinheiro (`founder/board.md`)

- [x] Modelo de cobrança validado no caixa: com honorário híbrido, a conta fecha **se** fecharem cerca de 1 mandato a cada 2 meses com captação média de R$ 3 mi.
- [ ] Quanto tempo a operação aguenta até a primeira taxa de sucesso: R$ 68 mil cobrem 3 meses sem receita; R$ 103,5 mil cobrem 5. **Ainda não comprovado:** depende do ciclo real de venda.
- [ ] Quantos mandatos por ano pagam a conta: **cerca de 5,2 por ano** (0,43 por mês) só para empatar. O plano supõe 11 no ano 1, e nada no painel ainda sustenta esse número.
- [ ] Garantia pagável: o custo líquido é baixo (a entrada devolvida já tinha sido recebida). O risco real são as horas de trabalho em mandatos que não fecham, que estimei em R$ 1.500 cada.

Receita sem impostos já descontados no preço: os impostos sobre serviço (estimados em 15%) entram como custo por mandato. Isto não é aconselhamento financeiro, contábil ou jurídico: um contador deve confirmar o regime tributário (Simples, Lucro Presumido), o pró-labore e os contratos antes de mexer em dinheiro.

---

# Unit economics: Proposta Firme de Crédito: assessoria de dívida para empresas de R$ 5-50 mi (nome a definir)

Every number below comes from the input file. Nothing is looked up or guessed.

## One mandato fechado

| line | per mandato fechado |
| --- | ---: |
| Price | $60,000.00 |
| Impostos sobre serviço (estimativa 15%, confirmar regime com contador) | -$9,000.00 |
| Comissão de indicação ao contador parceiro (estimativa 10%) | -$6,000.00 |
| Certidões, advogado, viagens e dados por operação (estimativa) | -$3,000.00 |
| Custo dos mandatos que não fecham, rateado (0,67 por mandato fechado x R$ 1.500) | -$1,000.00 |
| **Contribution** (what each mandato fechado leaves to pay the fixed costs) | **$41,000.00** (68%) |

## The margin that matters

Fixed costs: $17,700 a month (Pró-labore do fundador (estimativa, a definir) $12,000, Contador $1,200, Software, CRM e consultas de crédito $1,500, Coworking e salas de reunião $1,000, Marketing e eventos com contadores e associações $2,000).

- **Break-even: 1 mandato fechados a day.** Below that you lose money every month.
- **Profit margin at your plan** (2 a day): **54%** of every sale, after every cost.
- Capacity: 3 a day.

## Year 1, month by month

| month | mandato fechados a day | revenue | profit | cumulative (after $15,000 startup) |
| ---: | ---: | ---: | ---: | ---: |
| 1 | 0 | $0 | -$17,700 | -$32,700 |
| 2 | 0 | $0 | -$17,700 | -$50,400 |
| 3 | 0 | $0 | -$17,700 | -$68,100 |
| 4 | 0 | $30,000 | $2,800 | -$65,300 |
| 5 | 0 | $30,000 | $2,800 | -$62,500 |
| 6 | 1 | $60,000 | $23,300 | -$39,200 |
| 7 | 1 | $60,000 | $23,300 | -$15,900 |
| 8 | 1 | $60,000 | $23,300 | $7,400 |
| 9 | 2 | $90,000 | $43,800 | $51,200 |
| 10 | 2 | $90,000 | $43,800 | $95,000 |
| 11 | 2 | $120,000 | $64,300 | $159,300 |
| 12 | 2 | $120,000 | $64,300 | $223,600 |

- **Year 1 operating profit: $238,600** on $660,000 of revenue.
- After the $15,000 startup spend: $223,600.
- Startup money earned back: month 8.
- Cash you need before it pays for itself: **$68,100**.

## What if

| scenario | margin at plan | break-even a day | year 1 profit |
| --- | ---: | ---: | ---: |
| Base plan | 54% | 1 | $238,600 |
| Price -10% | 48% | 1 | $172,600 |
| Volume -20% | 50% | 1 | $148,400 |
| Unit costs +15% | 49% | 1 | $207,250 |

No red flags in these numbers. They are only as good as the inputs: check every cost against a real quote.
