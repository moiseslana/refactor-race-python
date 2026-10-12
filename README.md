# REFactor Race Python

## Equipe (Só eu mesmo kkkkk)
- Integrante 1: [Moises_Lameo_Lana]
- RA: 325140886


## Descrição
Projeto de refatoração de um sistema Python de processamento de pedidos. O objetivo é melhorar a organização, a legibilidade e a manutenibilidade sem alterar as regras de negócio existentes.

## Diagnóstico inicial
- A função `process_order` concentrava várias responsabilidades.
- Existia cálculo duplicado do subtotal.
- Havia condicionais aninhadas para descontos e frete.
- O código usava valores fixos diretamente nas regras.
- A identificação de produtos repetidos usava loops aninhados.

## Code smells encontrados
- Função extensa com muitas responsabilidades.
- Código duplicado.
- Condicionais complexas.
- Números e textos fixos espalhados pelo código.
- Busca de produtos repetidos com muitos loops.
- Impressão e armazenamento de resultados dentro da função principal.

## Refatorações realizadas
- Remoção do cálculo duplicado do subtotal.
- Simplificação das condições de desconto.
- Uso de `min()` para limitar o desconto máximo.
- Simplificação das condições de frete.
- Reorganização da identificação de produtos repetidos.

## Testes adicionados
Descrever os novos cenários implementados e registrar o resultado final da execução do pytest.

## Métricas antes e depois
Os resultados comparativos estão registrados no arquivo `METRICS.md`.

## Decisões técnicas
Foi utilizada a suíte pytest para verificar o comportamento do sistema. As ferramentas pytest-cov, Radon e Ruff foram utilizadas para analisar cobertura, complexidade, manutenibilidade e qualidade estática.

## Uso de inteligência artificial
Ferramenta utilizada: ChatGPT.

Finalidade: apoio para compreender os erros, planejar refatorações, interpretar métricas e revisar a documentação.

Exemplo de sugestão recebida: simplificar condicionais e remover o cálculo duplicado do subtotal.

Validação: as alterações foram revisadas e testadas com pytest. As métricas foram obtidas por meio da execução local das ferramentas.

## Melhorias futuras
- Dividir `process_order` em funções menores.
- Ampliar os testes para cenários de cupons, estados, frete e limites de desconto.
- Avaliar a separação entre cálculo, impressão e armazenamento de pedidos.
