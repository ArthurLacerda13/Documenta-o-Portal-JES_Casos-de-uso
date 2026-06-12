# Diagrama Geral de Casos de Uso - Portal JES

Este diagrama representa a visão geral do sistema, utilizando herança de atores para otimizar os relacionamentos conforme o modelo.

```mermaid
useCaseDiagram
    actor "Usuário Logado" as UL
    actor Capitão as C
    actor Moderador as M
    actor Admin as A
    actor Visitante as V

    %% Generalização/Herança
    C --|> UL
    M --|> C
    A --|> M

    package "Portal JES" {
        usecase UC01 as "Manter Atletas [RF001]"
        usecase UC02 as "Manter Capitão [RF002]"
        usecase UC03 as "Manter Moderador [RF003]"
        usecase UC04 as "Manter Atléticas [RF004]"
        usecase UC05 as "Manter Modalidades [RF005]"
        usecase UC06 as "Manter Equipes [RF006]"
        usecase UC07 as "Manter Partidas [RF007]"
        usecase UC08 as "Carregamento de Dados [RF008]"
        usecase UC10 as "Primeiro Acesso [RF010]"
        usecase UC11 as "Acesso às Estatísticas [RF011]"
    }

    UL --> UC10
    C --> UC01
    C --> UC06
    M --> UC02
    M --> UC04
    M --> UC05
    M --> UC07
    M --> UC08
    A --> UC03
    V --> UC11

    %% Relacionamentos <<include>>
    UC06 ..> UC01 : <<include>>
    UC06 ..> UC05 : <<include>>
    UC07 ..> UC04 : <<include>>
    UC07 ..> UC06 : <<include>>
```
