# Especificação de Caso de Uso: Manter Atléticas [RF004]

**Ator Principal:** Moderador
**Prioridade:** Essencial
**Complexidade:** Média

## Descrição
O sistema deve permitir ao Moderador realizar o cadastro e a manutenção das Atléticas participantes do JES.

## Dados Necessários
- Nome da atlética
- Cursos envolvidos
- Capitão (vinculação)
- Instituto
- Campi

## Regras de Negócio Vinculadas
- **[RN003] - Validação de Nome da Atlética:** O nome das atléticas deve ser único no sistema, possuindo no mínimo 3 e no máximo 255 caracteres.

## Fluxo Principal
1. O Moderador acessa o menu de "Manter Atléticas".
2. O sistema exibe as atléticas cadastradas.
3. O Moderador solicita o cadastro de uma nova atlética.
4. O Moderador insere o nome, seleciona os cursos, vincula o capitão responsável e define instituto/campi.
5. O sistema valida o nome conforme a **[RN003]**.
6. O sistema confirma o salvamento.

## Fluxo de Exceção
- **[FE01] Nome Duplicado ou Inválido:** Se o nome não atender à **[RN003]**, o sistema solicita correção.
