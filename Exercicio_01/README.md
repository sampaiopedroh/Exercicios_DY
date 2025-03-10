# Tarefa de Programação Dinâmica - Checkpoint 1

**Nome:** Pedro Henrique Ribeiro Sampaio
**RA:** 555613

**Data de Entrega:** 11 de março de 2025

## Descrição do Projeto

Este projeto aborda os conceitos de ordenação e estruturas de dados em Python, conforme especificado na tarefa de Programação Dinâmica - Checkpoint 1.  O projeto implementa dois algoritmos de ordenação, Merge Sort e Quick Sort (apenas Merge Sort foi implementado neste caso, devido a melhor didática para a tarefa), para classificar:

1. **Pontos 2D pela distância de Manhattan:** Uma lista de pontos 2D representados como tuplas (x, y) é classificada com base em sua distância de Manhattan a partir da origem (0, 0).
2. **Palavras por ordem personalizada:** Uma lista de palavras é classificada de acordo com um dicionário fornecido que mapeia cada caractere para um número de prioridade.

Além da implementação dos algoritmos de ordenação, o projeto também utiliza compreensão de lista para filtragem e reestruturação de dados e demonstra o armazenamento de dados usando tuplas e dicionários.  O desempenho dos algoritmos de ordenação (Merge Sort) é avaliado medindo o tempo de execução e o uso de memória.

## Explicar hipóteses e considerações para a sua solução.
A solução implementada utiliza Merge Sort para a ordenação de pontos e palavras, devido à sua complexidade de tempo O(n log n) consistente, adequada para os cenários propostos. Considerou-se a distância de Manhattan como critério de ordenação para os pontos 2D, calculando a soma dos valores absolutos das coordenadas. Para a ordenação de palavras, utilizou-se um dicionário de prioridades, atribuindo um valor padrão 0 para caracteres não mapeados, garantindo que todos os caracteres fossem considerados na comparação. Adicionalmente, implementou-se uma função de comparação que trata palavras com prefixos iguais, mas comprimentos diferentes, assegurando a ordenação correta mesmo nesses casos. A medição de desempenho foi realizada utilizando o módulo time para o tempo de execução e sys.getsizeof() para o uso de memória, fornecendo uma comparação da eficiência do Merge Sort e Quick Sort em ambos os cenários. Para evitar a modificação dos dados originais durante os testes de desempenho, foram utilizadas cópias das listas de entrada.

## Instruções de Execução

1. **Clone o Repositório:** Clone este repositório para sua máquina local usando o seguinte comando:
   ```bash
   git clone [URL do seu repositório]
