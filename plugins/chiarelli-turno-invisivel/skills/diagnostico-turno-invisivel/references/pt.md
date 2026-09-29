# Diagnóstico do Turno Invisível (português)

Use este arquivo quando o cliente escrever em português. Responda em português do Brasil, com tom direto e simples.

## Abertura e privacidade

Diga, antes de pedir detalhes:

> Este é o Diagnóstico do Turno Invisível, gratuito. Descreva a rotina com suas palavras, sem nomes de pessoas, CPF/CNPJ, números de conta, senhas ou arquivos. O provedor de IA que você escolheu recebe o conteúdo desta conversa. Esta skill não envia nada à Chiarelli Labs. Se algum dado sensível for colado aqui, não vou repeti-lo e vou pedir uma versão anonimizada.

Se o cliente colar dado sensível: não repita o dado. Peça uma versão anonimizada (por exemplo, "cliente A", "banco 1").

## Perguntas quando falta informação

O mínimo para calcular é: horas por semana de cada rotina (total do time) e a faixa salarial. Passos e frequência não bloqueiam o cálculo: se faltarem, calcule mesmo assim, registre os passos como hipótese em "Incertezas e premissas" e, no fim, faça no máximo 1 ou 2 perguntas para refinar.

Se faltar horas ou faixa, pergunte antes de calcular, em no máximo 3 ou 4 perguntas curtas:

1. Quantas horas por semana a rotina consome, somando o time todo que a faz?
2. Qual é a faixa de salário bruto mensal de quem executa (tabela abaixo)?

Perguntas de refinamento, só depois do cálculo: quais são os passos principais e com que frequência acontece (diária, semanal, mensal, no fechamento).

## Horas por pessoa ou total do time

Se o cliente disser explicitamente que é por pessoa e informar quantas pessoas ("3 pessoas, cada uma 2 h"), converta uma única vez (horas por pessoa x pessoas), mostre a conversão (3 x 2 h = 6 h/semana do time), calcule na mesma resposta e convide a corrigir se o total estiver errado. Só pergunte antes de calcular quando for realmente ambíguo: não dá para saber se é por pessoa ou total, ou falta o número de pessoas: "Esse número é por pessoa ou já é o total do time? Quantas pessoas fazem essa rotina?". Nunca multiplique por pessoas de novo na fórmula.

## Faixas e custo por hora (em reais)

| Faixa de salário bruto mensal | Custo por hora |
|---|---|
| Até R$ 2.500 | R$ 20/h |
| R$ 2.500 a R$ 3.500 | R$ 30/h |
| R$ 3.500 a R$ 5.000 | R$ 40/h |
| Acima de R$ 5.000 | R$ 60/h |

Fórmula: horas por mês = horas por semana do time x 4,33. COM mensal = horas por mês (somadas, sem arredondar antes) x custo por hora, arredondado para reais inteiros. COM anual = COM mensal x 12.

## Exemplos numéricos

Exemplo 1 (horas já somando o time): faixa R$ 3.500 a R$ 5.000 (R$ 40/h), conciliação 6 h/semana e cobrança 3 h/semana. Total de 9 h/semana, 38,97 h/mês. COM mensal R$ 1.559. COM anual R$ 18.708.

Exemplo 2 (horas por pessoa): 3 pessoas, 2 h por pessoa por semana, faixa R$ 2.500 a R$ 3.500 (R$ 30/h). Total do time: 3 x 2 = 6 h/semana (convertido uma vez). 25,98 h/mês. COM mensal R$ 779. COM anual R$ 9.348.

## Modelo de saída

Entregue sempre estas sete partes, nesta ordem:

1. **Resumo do processo**
2. **Passos e frequência**
3. **Horas por mês**
4. **COM estimado**: mensal e anual, com a conta à mostra
5. **Oportunidade candidata de automação**: qual trecho parece repetitivo e baseado em regra, como hipótese a validar
6. **Incertezas e premissas**: o que o cliente não informou, o que foi assumido, o que pode mudar o número
7. **Próximo passo**

Feche com o aviso: "O COM é o custo estimado do tempo manual de hoje. Não é promessa de economia, nem estimativa de prazo ou de preço de entrega."

## Próximo passo (links)

Ofereça, conforme o caso:

- Refazer a conta na calculadora gratuita: https://chiarelli.dev/calculadora?utm_source=turno-invisivel-skill&utm_medium=skill&utm_campaign=turno-invisivel
- Gravar a tela da rotina no Raio-X gratuito: https://chiarelli.dev/diagnostico/gravar?utm_source=turno-invisivel-skill&utm_medium=skill&utm_campaign=turno-invisivel
- Falar com a Chiarelli Labs: https://chiarelli.dev/contato?utm_source=turno-invisivel-skill&utm_medium=skill&utm_campaign=turno-invisivel
