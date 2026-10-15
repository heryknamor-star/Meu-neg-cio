# Oferta: Proposta Firme de Crédito

Base: `founder/panel/results.md` (100 compradores, pitch v1), `founder/board.md`, `founder/competitors.md`.
Ainda não existe `founder/numbers.json`: os custos abaixo são estimativas relativas (1 a 5), a confirmar com `/founder-cfo`.

## 1. Lista de problemas (nas palavras do comprador)

Antes de comprar
1. "Não conheço você nem nenhum cliente seu." (73 de 100 passaram por confiança)
2. "Já paguei consultoria adiantado e o crédito não saiu."
3. "Meu banco já me atende, para que um intermediário?"
4. "Não vou abrir meus números para um desconhecido."
5. "Não quero minha empresa rodando por 8 credores que não escolhi; o banco vai achar que estou desesperado."
6. "R$ 15 mil adiantado é dinheiro saindo de um caixa já curto."
7. "Apresentar a 8 credores não é crédito aprovado: a garantia não garante nada."
8. "Isso parece as ligações de 'crédito garantido'."
9. "Só contrato o que meu contador indicar."

Durante
10. "60 dias é muito; preciso de dinheiro em semanas."
11. "Meus números estão atrasados e desorganizados; não tenho tempo para isso."
12. "Vai tomar o tempo do meu controller/CFO."
13. "Não sei se vocês acessam mesmo bancos médios e FIDCs."

Depois / custo total
14. "2% em cima de um crédito que já é caro." (10 passaram por preço)
15. "Meu problema é juro alto, não falta de crédito."
16. "FIDC e fundo cobram mais que meu banco."
17. "Em captação grande, 2% vira R$ 300-400 mil."
18. "Vocês ganham comissão do credor? De que lado estão?"
19. "E se nenhuma proposta for melhor que a do meu banco?"

## 2. Soluções, pontuadas e cortadas

| # | Solução | Mata o problema | Valor (1-5) | Custo (1-5) | Fica? |
|---|---|---|---:|---:|---|
| A | Diagnóstico de crédito gratuito em 7 dias | 1, 3, 15, 19 | 4 | 2 | sim |
| B | NDA assinado antes de qualquer número | 4 | 4 | 1 | sim |
| C | Cliente aprova cada credor antes do envio | 5, 18 | 4 | 1 | sim |
| D | Entrada menor (R$ 7.500), 100% abatida do sucesso | 6, 14 | 4 | 2 | sim |
| E | Sucesso só se o cliente aceitar uma proposta; se não for melhor que a oferta escrita do banco, não aceita e não paga | 14, 15, 16, 19 | 5 | 2 | sim |
| F | Garantia: devolve a entrada se não houver proposta firme por escrito em 45 dias | 2, 7 | 4 | 3 | sim |
| G | Dossiê de crédito fica com o cliente mesmo sem fechar | 2, 11 | 3 | 1 | sim |
| H | Comparação do custo efetivo total das dívidas atuais | 15 | 3 | 2 | sim |
| I | Transparência: assessoria nova, primeira turma de 5 empresas em troca de autorização para relatar o caso | 1, 8 (honestidade) | 2 | 1 | sim |
| J | Sucesso escalonado (ex.: 1% acima de R$ 10 mi) | 17 | 3 | 3 | para o `/founder-pricing` |
| K | Entrada em conta-garantia (escrow) até a primeira proposta firme | 2, 6 | 4 | 2 | testar na v3 |
| L | Prazo expresso de 15 dias para quem está apagando incêndio | 10 | 4 | 4 | não por enquanto (depende de rede de credores comprovada) |
| M | Indicação via contador ou associação comercial | 1, 9 | 5 | 2 | é canal, vai para o `/founder-marketing` |

## 3. A oferta montada (pitch v2)

- **Núcleo:** uma proposta firme de crédito, por escrito, de banco médio, FIDC ou fundo, negociada por você.
- **Bônus:** diagnóstico gratuito (A), dossiê que fica com você (G), comparação do custo das dívidas atuais (H).
- **Garantia:** entrada de R$ 7.500 devolvida se não houver proposta firme em 45 dias (F). Sucesso só se você aceitar a proposta (E).
- **Escassez verdadeira:** 5 vagas na primeira turma, porque o fundador atende sozinho (I).
- **Nome:** Proposta Firme de Crédito.

Custo da garantia: depende da taxa de clientes sem proposta em 45 dias, que ainda não se conhece. Com 40% sem proposta, o custo esperado é R$ 3.000 por cliente mais as horas do dossiê. Rodar no `/founder-cfo` antes de prometer.

## 4. Equação de valor (antes → depois)

| Elemento | v1 | v2 | O que mexeu |
|---|---:|---:|---|
| Resultado dos sonhos | 6 | 7 | "proposta firme" no lugar de "apresentação"; comparação de custo (H) |
| Probabilidade percebida | 3 | 4 | garantia ligada a proposta firme (F), sucesso só se aceitar (E). Continua baixa: nenhum caso ou referência |
| Tempo até o resultado | 4 | 5 | 45 dias em vez de 60; diagnóstico em 7 dias (A) |
| Esforço e sacrifício | 4 | 6 | entrada menor e abatida (D), NDA e aprovação de credores (B, C), dossiê pronto (G) |

## 5. Re-teste (20 compradores, mesma semente, cartas diferentes porque o painel é menor)

| | v1 (100 compradores) | v2 (20 compradores) |
|---|---|---|
| Compram | 4 (4%) | 0 (0%) |
| Confiança | 73% | 85% |
| Preço | 10% | 10% |
| Prazo | 11% | 5% |
| Faixa de preço aceitável (entrada) | R$ 3.060 a R$ 19.913 | R$ 2.003 a R$ 14.947 |

**Nada melhorou.** As objeções de prazo e de garantia caíram, e ninguém mais reclamou de "pagar e não receber nada". Mas a confiança subiu de 73% para 85%. Dizer com honestidade que a assessoria é nova (I) deixou isso explícito, e nenhum termo do contrato substitui um caso real que o comprador possa conferir.

O sinal mais útil: **14 dos 20 aceitariam o diagnóstico gratuito**, mas não assinariam. O diagnóstico é a porta de entrada; a venda acontece depois, quando houver prova.

**Conclusão:** o problema não é a oferta nem o preço. É a falta de prova e de quem indique. Antes de mexer de novo na oferta:
1. Usar o histórico real do fundador, se existir (operações que conduziu em banco, IB ou empresa), com permissão e sem exagero. Foi a virada mais citada: "ver o histórico dos sócios num banco ou fundo".
2. Conseguir os 3 primeiros casos por indicação de contadores e associações comerciais, oferecendo o diagnóstico gratuito como entrada.
3. Para esses 3 primeiros, testar só sucesso (sem entrada) ou entrada em conta-garantia (K), e medir com clientes reais.

Regras: sem depoimentos inventados, sem escassez falsa. Garantias e promessas em contrato devem seguir o Código de Defesa do Consumidor e as regras aplicáveis; confirmar com um advogado (não é aconselhamento jurídico).
