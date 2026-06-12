# Caso de Uso: UC08 - Carregamento de Dados por Planilha

**Objetivo:** Permitir a importação em lote de dados de partidas via planilha.
**Requisitos:** [RF008]
**Atores:** Admin, Moderador
**Condição de entrada:** O ator seleciona 'Importar Planilha'.

## Fluxo Principal
1. O ator faz o upload do arquivo.
2. O sistema valida os registros conforme [RN006].
3. O sistema processa a importação dos dados válidos.

## Fluxos de Exceção
- **[RN006 - Validação de Planilha]:** Se houver erros de padrão, o sistema lista as linhas inválidas.
