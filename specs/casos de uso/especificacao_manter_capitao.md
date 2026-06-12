# Especificação de Caso de Uso: Manter Capitão [RF002]

**Ator Principal:** Moderador
**Prioridade:** Importante
**Complexidade:** Baixa

## Descrição
O sistema deve permitir ao Moderador alterar o cargo de um atleta (previamente cadastrado no sistema via [RF001]) para o cargo de Capitão.

## Fluxo Principal
1. O Moderador acessa a funcionalidade de gerenciamento de usuários/atletas.
2. O Moderador busca e seleciona um atleta cadastrado.
3. O Moderador solicita a alteração do cargo do atleta selecionado para "Capitão".
4. O sistema valida se o atleta já não possui outro cargo administrativo conflitante.
5. O sistema confirma a alteração e atualiza as permissões de acesso do novo Capitão.

## Fluxo de Exceção
- **[FE01] Atleta não encontrado:** Se a busca não retornar resultados, o sistema informa que o atleta precisa ser cadastrado primeiro.
