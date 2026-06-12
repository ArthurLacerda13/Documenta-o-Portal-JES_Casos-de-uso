# Caso de Uso: UC10 - Primeiro Acesso

**Objetivo:** Obrigar o usuário a alterar a senha padrão no primeiro login.
**Requisitos:** [RF010]
**Atores:** Usuário (Admin, Moderador ou Capitão)
**Condição de entrada:** O usuário realiza login pela primeira vez.

## Fluxo Principal
1. O sistema identifica o primeiro acesso.
2. O sistema redireciona para troca de senha.
3. O usuário insere nova senha seguindo [RNF006].
4. O sistema libera o acesso.

## Fluxos de Exceção
- **[RNF006 - Senha Forte]:** Se a senha não atender aos requisitos (8 chars, maiúscula, minúscula, número), o sistema exige correção.
