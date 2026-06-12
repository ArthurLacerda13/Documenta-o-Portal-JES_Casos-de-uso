# Especificação de Caso de Uso: Manter Partidas [RF007]

**Ator Principal:** Moderador
**Prioridade:** Essencial
**Complexidade:** Alta

## Descrição
O sistema deve permitir ao Moderador realizar o gerenciamento e cadastro de Partidas do campeonato.

## Dados Necessários
- Modalidade ([RF005])
- Equipes/Atléticas que se enfrentarão ([RF004]/[RF006])
- Data e Horário
- Local
- Fase da competição
- Status da partida

## Regras de Negócio Vinculadas
- **[RN005] - Criação de Súmula:** Quando uma partida for criada, o sistema deve gerar automaticamente uma súmula personalizada para aquela respectiva modalidade.

## Fluxo Principal
1. O Moderador define os detalhes da partida (Equipes, Local, Data).
2. O sistema verifica a disponibilidade do local/horário (opcional).
3. Ao salvar a partida, o sistema aciona a **[RN005]** e gera a súmula digital.
4. A partida fica disponível para visualização pública e edição de resultados posterior.
