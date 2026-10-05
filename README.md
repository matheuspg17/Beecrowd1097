# Resolução exercício Beecrowd1097

## Descrição do problema
O programa não possui dados de entrada e deve apenas exibir uma sequência numérica predefinida. A variável `I` percorre os números ímpares de 1 até 9 (`1, 3, 5, 7, 9`). Para cada valor de `I`, a variável `J` deve assumir três valores decrescentes baseados na relação `(6 + I)` até `(4 + I)`.

## Como Funciona
1. O algoritmo utiliza dois laços de repetição `for` de forma aninhada.
2. O **laço externo** controla a variável `i`, iniciando em 1 e indo até 9 com incrementos de duas em duas unidades (`i += 2`) para filtrar apenas números ímpares.
3. O **laço interno** controla a variável `j`, cujos limites mudam dinamicamente a cada iteração do laço externo:
   - O valor inicial de `j` é definido por `6 + i`.
   - O laço decrementa de um em um (`j--`) até atingir o limite inferior definido por `4 + i`.
4. Dentro do bloco interno, a instrução `System.out.println` imprime o par corrente formatado como `I=x J=y`.