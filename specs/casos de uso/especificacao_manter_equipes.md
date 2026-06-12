# Especificação de Caso de Uso: Manter Equipes [RF006]

**Ator Principal:** Capitão
**Prioridade:** Essencial
**Complexidade:** Alta

## Descrição
O sistema deve permitir ao Capitão realizar o cadastro das equipes de sua atlética para as diferentes modalidades.

## Dados Necessários
- Modalidade (conforme [RF005])
- Atletas selecionados (conforme [RF001])

## Regras de Negócio Vinculadas
- **[RN004] - Validação de Time/Equipe:** 
    - Nome único por atlética/modalidade.
    - Número de atletas deve respeitar os limites da modalidade ([RF005]).
    - Todos os atletas devem pertencer à mesma atlética.
    - Nenhum atleta pode estar duplicado em times da mesma modalidade.

## Fluxo Principal
1. O Capitão seleciona a modalidade desejada.
2. O Capitão seleciona os atletas de sua atlética para compor a equipe.
3. O sistema valida se os atletas pertencem à atlética do capitão.
4. O sistema valida se o número de atletas está dentro do min/max da modalidade (**[RN004]**).
5. O sistema verifica se algum atleta já está inscrito em outra equipe da mesma modalidade (**[RN004]**).
6. O sistema confirma a inscrição da equipe.
