# Especificação de Caso de Uso: Manter Moderador [RF003]

**Ator Principal:** Admin
**Prioridade:** Essencial
**Complexidade:** Baixa

## Descrição
O sistema deve permitir ao Administrador (Admin) realizar o cadastro de novos Moderadores no sistema.

## Dados Necessários
- Matrícula
- Nome completo
- E-mail institucional
- Senha padrão
- Nível de permissão (Nível 2)

## Fluxo Principal
1. O Admin acessa a área de administração de usuários.
2. O Admin seleciona a opção "Cadastrar Moderador".
3. O Admin preenche os campos obrigatórios (Matrícula, Nome, E-mail, Senha).
4. O sistema valida se o e-mail é institucional e se a matrícula é única.
5. O sistema salva o novo Moderador com nível 2 de permissão.

## Fluxo de Exceção
- **[FE01] Usuário já existente:** Se a matrícula ou e-mail já estiverem em uso, o sistema impede o cadastro e notifica o Admin.
