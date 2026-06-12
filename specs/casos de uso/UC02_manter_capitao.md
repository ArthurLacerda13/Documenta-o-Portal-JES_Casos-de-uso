# Caso de Uso: UC02 - Manter Capitão

**Objetivo:** Permitir que o Moderador promova um atleta ao cargo de Capitão.
**Requisitos:** [RF002]
**Atores:** Moderador
**Condição de entrada:** O ator acessa a lista de atletas cadastrados.

## Fluxo Principal
1. O ator busca e seleciona um atleta na lista geral.
2. O ator solicita a alteração do cargo para "Capitão".
3. O sistema valida se o atleta está apto para a promoção.
4. O sistema confirma a alteração e atualiza as permissões.

## Fluxos de Exceção
- **[Exceção - Atleta já é Capitão]:** O sistema informa que o cargo já está atribuído.
