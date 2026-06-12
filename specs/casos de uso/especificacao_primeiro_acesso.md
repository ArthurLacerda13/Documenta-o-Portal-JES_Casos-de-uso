# Especificação de Caso de Uso: Primeiro Acesso [RF010]

**Ator Principal:** Usuário (Capitão, Moderador, Admin)
**Prioridade:** Essencial
**Complexidade:** Média

## Descrição
O sistema deverá obrigar o usuário a alterar sua senha padrão no primeiro login efetuado por questões de segurança.

## Regras de Negócio Vinculadas
- **[RNF006] - Validação de Senha Forte:** Mínimo de 8 caracteres, 1 minúscula, 1 maiúscula, 1 número, sem blacklists.

## Fluxo Principal
1. O usuário realiza o login com a senha padrão.
2. O sistema detecta que é o primeiro acesso.
3. O sistema redireciona o usuário obrigatoriamente para a tela de troca de senha.
4. O usuário insere a nova senha, validada pela **[RNF006]**.
5. O sistema confirma a alteração e libera o acesso ao dashboard.
