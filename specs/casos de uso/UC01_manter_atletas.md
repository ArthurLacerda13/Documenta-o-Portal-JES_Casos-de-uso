# Caso de Uso: UC01 - Manter Atletas

**Objetivo:** Permitir que o Capitão realize o cadastro e a manutenção (inclusão, alteração, exclusão e consulta) dos atletas de sua atlética.
**Requisitos:** [RF001]
**Atores:** Capitão
**Condição de entrada:** O ator seleciona 'Manter Atletas' no Dashboard do Capitão.

## Fluxo Principal
1. O ator acessa a página de Manutenção de Atletas.
2. O sistema exibe a lista de atletas já cadastrados.
3. O ator solicita a inclusão de um novo atleta.
4. O ator insere Nome, Matrícula, Foto, Sexo e Data de Nascimento.
5. O sistema valida os dados conforme [RN001] e [RN002].
6. O sistema confirma o salvamento do registro.
7. O sistema retorna à lista de atletas atualizada.

## Fluxos de Exceção
- **[RN001 - Validação de Matrícula]:** Se a matrícula não contiver apenas números (6 a 10 dígitos) ou já existir, o sistema exibe erro.
- **[RN002 - Validação de Data de Nascimento]:** Se a idade não estiver entre 14 e 100 anos, o sistema impede o cadastro.
