# Nota do CFO (leia primeiro)

**Atualizada em 15/10/2026** depois do `/founder-ops`: software e consultas caíram de R$ 1.500 para R$ 600/mês (preços públicos em `founder/ops.md`) e entrou o custo dos diagnósticos grátis que não viram mandato (R$ 900 por mandato fechado).

**Como ler a tabela abaixo:** a ferramenta escreve "$" e "a day". Aqui, **$ = R$** e **"a day" = por mês** (1 "dia" por mês, porque a unidade é um mandato fechado). Quase todos os números de entrada são **estimativas**, marcadas em `founder/cfo-sources.md`.

- **A margem:** cada mandato fechado (captação média estimada de R$ 3 mi, honorário de 2% = R$ 60 mil) deixa **R$ 40.100 (67%)**. No plano de 2 mandatos por mês, a margem de lucro é **53%**. O ponto de equilíbrio é **0,42 mandato por mês** (R$ 16.800 ÷ R$ 40.100), cerca de 5 por ano.
- **A linha a observar: quantos mandatos fecham, e quando.** Com metade do ritmo, o lucro do ano 1 cai de R$ 239.500 para **R$ 18.950** (`--volume 0.5`). Se o primeiro mandato só fechar no mês 6: R$ 18.950 e **R$ 99.000 de caixa** necessário.
- **A segunda linha: o tamanho médio da captação.** Com R$ 1,5 mi de média (honorário de R$ 30 mil), o ano 1 dá **prejuízo de R$ 90.500** (`--price 30000`). Daí o mínimo de R$ 40 mil por operação em `founder/pricing.md`.
- **Caixa:** no plano, **R$ 65.400** antes de se pagar; no cenário lento, R$ 99.000.

## Três formas de melhorar (testadas na ferramenta)

| Mudança | O que muda | Lucro do ano 1 | Caixa necessário |
|---|---|---:|---:|
| Base | — | R$ 239.500 | R$ 65.400 |
| Pró-labore de R$ 6 mil até o primeiro mandato | custo fixo cai para R$ 10.800 | R$ 311.500 | **R$ 47.400** |
| Honorário mínimo que eleve a média para R$ 66 mil | preço +10% | R$ 305.500 | R$ 65.400 |
| Comissão de indicação de 5% (em vez de 10%) | contribuição sobe para R$ 43.100 (72%) | R$ 272.500 | R$ 65.400 |

## Condições do conselho sobre dinheiro (`founder/board.md`)

- [x] Modelo de cobrança fecha no papel **se** fecharem cerca de 5 mandatos por ano com captação média de R$ 3 mi.
- [ ] Tempo que a operação aguenta até a primeira taxa de sucesso: depende do ciclo real de venda (`founder/launch.md`).
- [ ] Captação média real: medir nos primeiros diagnósticos.

Os impostos sobre serviço (estimados em 15%) entram como custo por mandato. Isto não é aconselhamento financeiro, contábil ou jurídico: um contador deve confirmar o regime tributário, o pró-labore e os contratos antes de mexer em dinheiro.

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
| Diagnósticos grátis que não viram mandato (3 por mandato x R$ 300 em consultas e deslocamento) | -$900.00 |
| **Contribution** (what each mandato fechado leaves to pay the fixed costs) | **$40,100.00** (67%) |

## The margin that matters

Fixed costs: $16,800 a month (Pró-labore do fundador (estimativa, a definir) $12,000, Contador $1,200, Software e consultas (Google Workspace, Clicksign, CRM, Serasa; ver founder/ops.md) $600, Coworking e salas de reunião $1,000, Marketing e eventos com contadores e associações $2,000).

- **Break-even: 1 mandato fechados a day.** Below that you lose money every month.
- **Profit margin at your plan** (2 a day): **53%** of every sale, after every cost.
- Capacity: 3 a day.

## Year 1, month by month

| month | mandato fechados a day | revenue | profit | cumulative (after $15,000 startup) |
| ---: | ---: | ---: | ---: | ---: |
| 1 | 0 | $0 | -$16,800 | -$31,800 |
| 2 | 0 | $0 | -$16,800 | -$48,600 |
| 3 | 0 | $0 | -$16,800 | -$65,400 |
| 4 | 0 | $30,000 | $3,250 | -$62,150 |
| 5 | 0 | $30,000 | $3,250 | -$58,900 |
| 6 | 1 | $60,000 | $23,300 | -$35,600 |
| 7 | 1 | $60,000 | $23,300 | -$12,300 |
| 8 | 1 | $60,000 | $23,300 | $11,000 |
| 9 | 2 | $90,000 | $43,350 | $54,350 |
| 10 | 2 | $90,000 | $43,350 | $97,700 |
| 11 | 2 | $120,000 | $63,400 | $161,100 |
| 12 | 2 | $120,000 | $63,400 | $224,500 |

- **Year 1 operating profit: $239,500** on $660,000 of revenue.
- After the $15,000 startup spend: $224,500.
- Startup money earned back: month 8.
- Cash you need before it pays for itself: **$65,400**.

## What if

| scenario | margin at plan | break-even a day | year 1 profit |
| --- | ---: | ---: | ---: |
| Base plan | 53% | 1 | $239,500 |
| Price -10% | 48% | 1 | $173,500 |
| Volume -20% | 49% | 1 | $151,280 |
| Unit costs +15% | 48% | 1 | $206,665 |

No red flags in these numbers. They are only as good as the inputs: check every cost against a real quote.
