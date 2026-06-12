# Caso de Uso: UC03 - Manter Moderador

**Objetivo:** Permitir que o Admin realize o cadastro de novos Moderadores.
**Requisitos:** [RF003]
**Atores:** Admin
**Condição de entrada:** O ator acessa 'Área Administrativa' e seleciona 'Novo Moderador'.

## Fluxo Principal
1. O ator preenche Matrícula, Nome Completo, E-mail Institucional e Senha.
2. O sistema valida a unicidade da matrícula e o domínio do e-mail.
3. O sistema salva o novo usuário com Nível 2 de permissão.

## Fluxos de Exceção
- **[Exceção - E-mail Inválido]:** O sistema impede o cadastro se o e-mail não for institucional.
