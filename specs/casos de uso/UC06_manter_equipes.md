# Caso de Uso: UC06 - Manter Equipes

**Objetivo:** Permitir que o Capitão realize o cadastro das equipes de sua atlética.
**Requisitos:** [RF006]
**Atores:** Capitão
**Condição de entrada:** O ator seleciona 'Minhas Equipes' no Dashboard.

## Fluxo Principal
1. O ator seleciona a Modalidade.
2. O ator seleciona os Atletas.
3. O sistema valida os atletas e limites conforme [RN004].
4. O sistema confirma a inscrição.

## Fluxos de Exceção
- **[RN004 - Validação de Equipe]:** Valida se atletas são da mesma atlética e não estão duplicados na mesma modalidade.
