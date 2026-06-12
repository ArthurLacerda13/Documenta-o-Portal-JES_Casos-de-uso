# Caso de Uso: UC04 - Manter Atléticas

**Objetivo:** Permitir que o Moderador realize o cadastro e manutenção das Atléticas.
**Requisitos:** [RF004]
**Atores:** Moderador
**Condição de entrada:** O ator acessa 'Gestão de Atléticas' no Dashboard.

## Fluxo Principal
1. O ator preenche Nome da Atlética, Cursos, Capitão, Instituto e Campi.
2. O sistema valida o nome conforme [RN003].
3. O sistema salva a nova Atlética.

## Fluxos de Exceção
- **[RN003 - Validação de Nome]:** O nome deve ser único e ter entre 3 e 255 caracteres.
