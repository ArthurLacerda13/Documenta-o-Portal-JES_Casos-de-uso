# Caso de Uso: UC05 - Manter Modalidades

**Objetivo:** Permitir que o Moderador realize o cadastro de modalidades esportivas.
**Requisitos:** [RF005]
**Atores:** Moderador
**Condição de entrada:** O ator acessa 'Gestão de Modalidades'.

## Fluxo Principal
1. O ator define Nome, Categoria, Tipo e limites de atletas (mínimo/máximo).
2. O sistema salva a modalidade.

## Fluxos de Exceção
- **[Exceção - Limites Inválidos]:** O sistema valida se o mínimo é menor que o máximo.
