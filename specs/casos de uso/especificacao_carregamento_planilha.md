# Especificação de Caso de Uso: Carregamento de Dados por Planilha [RF008]

**Ator Principal:** Admin ou Moderador
**Prioridade:** Importante
**Complexidade:** Alta

## Descrição
O sistema deve permitir o envio de planilhas para a população em lote dos dados das partidas, agilizando o processo manual.

## Regras de Negócio Vinculadas
- **[RN006] - Validação de Planilha:** O sistema deve validar o arquivo, checando padrões de registros, tipos de esportes e aplicando algoritmos para barrar erros de preenchimento.

## Fluxo Principal
1. O usuário faz o upload de um arquivo (.xlsx ou .csv).
2. O sistema processa o arquivo e valida as informações conforme a **[RN006]**.
3. O sistema exibe um resumo dos dados importados e eventuais erros.
4. O usuário confirma a importação dos dados válidos.
