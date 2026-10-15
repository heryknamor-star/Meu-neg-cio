# Preço: Proposta Firme de Crédito

Fontes: `founder/pricing-curve.md` (painel v1, 100 compradores), `founder/pricing-curve-v2.md` (painel v2, 20), `founder/competitors.md`, `founder/numbers.json` e a ferramenta do CFO.
Na saída das ferramentas, "$" = R$ e "a day" = por mês.

## O que os compradores disseram (simulados: servem para escolher o que testar, não são prova)

As perguntas de preço do painel valiam para a **entrada fixa**, não para a taxa de sucesso.

| Ponto | Painel v1 | Painel v2 |
|---|---:|---:|
| PMC (abaixo disso, "barato demais") | R$ 3.060 | R$ 2.003 |
| IPP (tantos acham barato quanto caro) | R$ 8.080 | R$ 5.093 |
| PME (acima disso, muitos não compram) | R$ 19.913 | R$ 14.947 |
| Mediana "começa a ficar caro" | R$ 12.000 | R$ 12.000 |

Sobre a taxa de sucesso não há curva, só objeções: 10 de 100 passaram por preço, quase sempre pelos 2%, não pela entrada.

## O que os concorrentes cobram (`founder/competitors.md`)

Quase nada é público. Referências que existem:
- Venda de empresa acima de R$ 180 mi: 3% de sucesso, considerado prática de mercado pelo TJSC.
- Referência internacional (não brasileira): 1% a 5% de sucesso, mais mensalidade.
- Consultorias de crédito de varejo: cerca de R$ 5.600 em 12 parcelas, com reclamações de "paguei e o crédito não saiu".
- Plataformas de crédito (Finplace e similares): grátis para quem toma o crédito.

Ou seja: 2% está dentro do que se vê em assessoria, mas o comprador compara com o próprio banco e com plataformas que não cobram nada dele.

## O que o negócio precisa (ferramenta do CFO)

| Honorário médio por mandato | Contribuição | Margem no plano | Lucro do ano 1 | Caixa necessário |
|---:|---:|---:|---:|---:|
| R$ 45.000 (1,5% de R$ 3 mi) | R$ 26.000 (58%) | 38% | R$ 73.600 | R$ 77.500 |
| **R$ 60.000 (2% de R$ 3 mi)** | **R$ 41.000 (68%)** | **54%** | **R$ 238.600** | **R$ 68.100** |
| R$ 66.000 (com mínimo puxando a média) | R$ 47.000 (71%) | 58% | R$ 304.600 | R$ 68.100 |
| R$ 75.000 | R$ 56.000 (75%) | 63% | R$ 403.600 | R$ 68.100 |

Em 1,5% o negócio ainda dá lucro no plano, mas fica frágil se o ritmo atrasar.

## 1. O preço

- **Entrada: R$ 7.500**, abatida do sucesso e devolvida se não houver proposta firme em 45 dias. Fica perto do IPP do painel v1 (R$ 8.080), acima do IPP do v2 (R$ 5.093) e bem abaixo do PME dos dois.
- **Sucesso: 2% até R$ 10 mi captados e 1% sobre o que passar de R$ 10 mi**, pago só se o cliente aceitar a proposta. A faixa acima de R$ 10 mi responde à objeção mais concreta do painel: "2% sobre R$ 15-20 mi são R$ 300-400 mil".
- **Mínimo de R$ 40.000 por operação fechada.** Com captação de R$ 1,5 mi, 2% dariam R$ 30 mil e o ano 1 viraria prejuízo de R$ 91.400 (`--price 30000`, ver `founder/cfo.md`). O mínimo protege a margem nas operações pequenas e deve aparecer no diagnóstico gratuito, antes da assinatura.
- No caso médio (R$ 3 mi), o honorário continua R$ 60 mil: `founder/numbers.json` não muda.

## 2. A escada

| Degrau | O que é | Preço | Por que subir |
|---|---|---|---|
| 1. Diagnóstico de crédito | Em 7 dias: quanto crédito a empresa consegue, de quem e a que custo estimado, com NDA | Grátis | 14 de 20 no painel v2 aceitariam. É a porta de entrada |
| 2. Dossiê para o seu banco | Números, certidões e material de crédito prontos para o cliente levar ao próprio banco e negociar sozinho | R$ 7.500 fixo | Serve ao perfil "fiel ao banco" (22% do painel, 0% de compra), que disse que usaria o diagnóstico para negociar com o banco |
| 3. Proposta Firme de Crédito | Tudo do degrau 2, mais a negociação com bancos médios, FIDCs e fundos e a garantia de 45 dias | R$ 7.500 de entrada + sucesso | Se o banco não resolver, os R$ 7.500 do dossiê viram a entrada do degrau 3. Ninguém paga duas vezes |

## 3. Oferta de lançamento

**Primeira turma, 5 empresas: entrada zero, só sucesso.** Termina quando 5 mandatos forem assinados ou em 31/03/2027, o que vier primeiro. A troca é a autorização para relatar o caso (sem nomes, se o cliente preferir).

Custo, pela lógica do CFO: a entrada já é abatida do sucesso e devolvida se não houver proposta. Retirá-la só custa nos casos em que há proposta e o cliente recusa, e no caixa dos primeiros meses. Os R$ 68.100 de caixa necessário não mudam, porque o plano não contava com entradas.

Isso responde a primeira virada mais pedida no painel ("zero adiantado") sem virar desconto permanente: a escassez é real (o fundador atende sozinho) e a data é fixa.

## 4. O que testar com compradores reais

1. **Entrada R$ 5.000 contra R$ 7.500**, depois da primeira turma. Alternar a proposta enviada a cada diagnóstico concluído e medir a taxa de assinatura.
2. **Sucesso 2% contra 1,5% com mínimo de R$ 40 mil.** Mesma alternância. Com poucos clientes, isso é uma leitura, não uma estatística: decida pela tendência dos primeiros 10.
3. **Degrau 2 sozinho:** quantos diagnósticos viram dossiê para o próprio banco, e quantos dossiês sobem para o degrau 3.

## 5. Objeções de preço, nas palavras do painel (para o marketing responder)

1. "Se captar R$ 5 milhões, são R$ 100 mil de honorário só de sucesso." (P098)
2. "Pagar R$ 15 mil adiantado mais 2% do captado come justamente a economia de taxa que eu iria buscar." (P098) / "2% do captado come boa parte da economia de taxa que eu conseguiria sozinha." (P013)
3. "2% sobre uma captação de R$ 15-20 mi para a fábrica são R$ 300-400 mil a mais num crédito que já está caro com essa Selic." (P004, painel v2)

Resposta que a oferta já dá: sucesso só se a proposta for aceita e melhor que a do banco; 1% acima de R$ 10 mi; comparação do custo efetivo total no diagnóstico, mostrando a economia em reais antes de qualquer assinatura.

Estas são falas de compradores simulados. Não use como depoimento.
