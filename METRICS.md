# Métricas — REFactor Race Python

## Objetivo

Comparar a qualidade do código antes e depois da refatoração.

## Comparação antes e depois

| Indicador                         |     Antes |    Depois |
| --------------------------------- | --------: | --------: |
| Testes aprovados                  |         4 |         6 |
| Quantidade de testes              |         4 |         6 |
| Cobertura de testes               |       83% |       85% |
| Complexidade de process_order     |    E (34) |    D (26) |
| Complexidade média                |  E (34,0) |  D (26,0) |
| Índice de manutenibilidade        | A (51,69) | A (58,20) |
| Problemas identificados pelo Ruff |         4 |         0 |

## Análise dos resultados

A quantidade de testes passou de 4 para 6, e todos os testes passaram na medição final. A cobertura aumentou de 83% para 85%.

A complexidade ciclomática de process_order caiu de 34 para 26, passando da classificação E para D. O índice de manutenibilidade aumentou de 51,69 para 58,20, mantendo a classificação A.

O Ruff apontou quatro problemas na análise inicial e não listou problemas na análise final.

## Conclusão

Os resultados indicam melhorias na complexidade, na manutenibilidade e na cobertura dos testes. Os testes automatizados foram utilizados para verificar se as mudanças mantiveram os comportamentos cobertos pela suíte.
