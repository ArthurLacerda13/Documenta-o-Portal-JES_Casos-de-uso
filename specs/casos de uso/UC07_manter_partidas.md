# Caso de Uso: UC07 - Manter Partidas

**Objetivo:** Permitir que o Moderador realize o gerenciamento de Partidas.
**Requisitos:** [RF007]
**Atores:** Moderador
**Condição de entrada:** O ator acessa 'Calendário de Partidas'.

## Fluxo Principal
1. O ator define Modalidade, Equipes, Data, Horário e Local.
2. O sistema salva a partida e gera a súmula automática conforme [RN005].

## Fluxos de Exceção
- **[RN005 - Criação de Súmula]:** O sistema notifica se houver erro na geração automática da súmula.
