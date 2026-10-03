# INSTRUÇÕES DO GROK BOT — LER MARCAÇÕES (SUPABASE) E ESCREVER NA PLANILHA

## O QUE VOCÊ (BOT) FAZ
As pessoas agendam no SITE. Cada marcação cai numa tabela no Supabase.
Sua tarefa: LER as marcações novas no Supabase e ESCREVER cada uma na planilha
final (abrindo a planilha e digitando a linha), depois marcar como processada.

## ONDE ESTÃO AS MARCAÇÕES (SUPABASE)
- Projeto: dunicowisky  (ref: txvrotvqekfimlrqpwly)
- Painel/tabela: https://supabase.com/dashboard/project/txvrotvqekfimlrqpwly/editor
- Tabela: bot_marcacoes
- "Novas" = linhas com a coluna  processado = false (ou vazia).

Colunas da tabela (o que cada marcação tem):
  data_envio, nome, cpf, nascimento, email, telefone,
  regiao, unidade, tipo_atendimento, data_hora_agendada, endereco_clinica, processado

## PARA ONDE VOCÊ COPIA (PLANILHA FINAL)
- Link da planilha: https://docs.google.com/spreadsheets/d/1C5fPwv96J4jq77E7BEQ6oYzWhfAW-pidDekBpsW4mKw/edit
- Aba: AGENDAMENTOS (se não existir, crie). Escreva 1 linha por marcação,
  na primeira linha vazia, SEM apagar nada.
- Ordem das colunas na planilha:
  A: data_envio | B: nome | C: cpf | D: nascimento | E: email | F: telefone |
  G: regiao | H: unidade | I: tipo_atendimento | J: data_hora_agendada | K: endereco_clinica

## PASSO A PASSO (repita sempre)
1. Abra a tabela bot_marcacoes no Supabase (link acima).
2. Pegue as linhas com processado = false.
3. Para CADA linha:
   a. Abra a planilha final e escreva a linha (colunas A..K na ordem acima).
   b. (Opcional) separe/organize por unidade se precisar.
   c. Volte no Supabase e marque processado = true nessa linha
      (assim você não copia a mesma marcação duas vezes).
4. Pronto. Repita quando houver novas.

## OBSERVAÇÕES
- Nunca apague linhas no Supabase; só marque processado = true.
- Se algum dado vier faltando, copie do jeito que está e sinalize.
