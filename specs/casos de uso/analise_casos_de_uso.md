# Diagrama Geral de Casos de Uso - Portal JES

Este diagrama representa a visão geral dos casos de uso do sistema, relacionando os atores (Admin, Moderador, Capitão e Visitante) às funcionalidades principais.

```mermaid
useCaseDiagram
    actor Admin
    actor Moderador
    actor Capitão
    actor Visitante

    package "Portal JES" {
        usecase UC01 as "Manter Atletas [RF001]"
        usecase UC02 as "Manter Capitão [RF002]"
        usecase UC03 as "Manter Moderador [RF003]"
        usecase UC04 as "Manter Atléticas [RF004]"
        usecase UC05 as "Manter Modalidades [RF005]"
        usecase UC06 as "Manter Equipes [RF006]"
        usecase UC07 as "Manter Partidas [RF007]"
        usecase UC08 as "Carregamento de Dados (Planilha) [RF008]"
        usecase UC09 as "Otimização de Processos [RF009]"
        usecase UC10 as "Primeiro Acesso (Troca Senha) [RF010]"
        usecase UC11 as "Acesso às Estatísticas [RF011]"
    }

    Admin --> UC03
    Admin --> UC08
    Admin --> UC10

    Moderador --> UC02
    Moderador --> UC04
    Moderador --> UC05
    Moderador --> UC07
    Moderador --> UC08
    Moderador --> UC10

    Capitão --> UC01
    Capitão --> UC06
    Capitão --> UC10

    Visitante --> UC11
    
    %% Relacionamentos de dependência
    UC06 ..> UC01 : <<include>>
    UC06 ..> UC05 : <<include>>
    UC07 ..> UC04 : <<include>>
    UC07 ..> UC06 : <<include>>
```

## Resumo dos Atores
- **Admin (Nível 3):** Responsável pela gestão de moderadores e carga massiva de dados.
- **Moderador (Nível 2):** Responsável pela gestão de atletas (promoção a capitão), atléticas, modalidades e partidas.
- **Capitão (Nível 1):** Responsável por cadastrar atletas e montar as equipes de sua atlética.
- **Visitante:** Usuário anônimo que consome as estatísticas públicas.
