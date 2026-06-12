# Especificação de Caso de Uso: Manter Atletas [RF001]

**Ator Principal:** Capitão
**Prioridade:** Essencial
**Complexidade:** Média

## Descrição
O sistema deve permitir que o Capitão realize o cadastro e a manutenção (inclusão, alteração, exclusão e consulta) dos atletas de sua atlética.

## Dados Necessários
- Nome do atleta
- Matrícula
- Foto
- Sexo

## Regras de Negócio Vinculadas
- **[RN001] - Validação de Matrícula:** As matrículas devem conter apenas números, possuir de 6 a 10 dígitos e ser únicas no sistema.
- **[RN002] - Validação de Data de Nascimento:** As datas de nascimento não podem ser futuras e a idade deve estar estritamente entre 14 e 100 anos.

## Fluxo Principal
1. O Capitão acessa a funcionalidade de "Manter Atletas" no Dashboard do Capitão.
2. O sistema exibe a lista de atletas já cadastrados.
3. O Capitão solicita a inclusão de um novo atleta.
4. O Capitão insere os dados necessários (Nome, Matrícula, Foto, Sexo, Data de Nascimento).
5. O sistema valida os dados conforme as regras **[RN001]** e **[RN002]**.
6. O sistema confirma o salvamento do registro.
7. O sistema retorna à lista de atletas atualizada.

## Fluxo de Exceção
- **[FE01] Matrícula Inválida:** Se a matrícula não seguir o padrão da **[RN001]**, o sistema exibe mensagem de erro e solicita correção.
- **[FE02] Idade fora do limite:** Se a idade calculada não estiver entre 14 e 100 anos (**[RN002]**), o sistema impede o cadastro e informa o erro.
