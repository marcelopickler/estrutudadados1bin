## 1 Problema
### Quais sao as duas caracterısticas mais comuns para analisar algoritmos?

##### Tempo e consumo de memória.
## 2 Problema
### Por que a medida de tempo em segundos nao representa qualificadamente o tempo de execucao de um algoritmo?

##### Não é medida em tempo o software já que deve possuir certa independência entre a tecnología; o software e o hardware.
## 3 Problema
### A medida de tempo de um algoritmo é realizada através de qual informacao?
### O que pode afetá-la?

##### A medição do tempo em representação a qualidade e estabilidade do software é feita mediante os passos do algoritmo que precisa  para finalizar a sua execução. Pode afetá-la pelo ambiente do hardware em que ela é executada e o tamanho da entrada.
## 4 Problema
### Na análise de algoritmos, qual é o valor da base da funcao logarítmica e exponencial? Por que é escolhido este valor?

##### A base da função logarítmica e exponencial é 2. A base 2 tem uma importância muito considerada na informática dada a codificação  binária que utiliza.O algoritmo binário tem uma frequência de aparição grande no análise de algoritmos. Na funcao logarítmica é  usada para descompor o número até chegar a uma base binária; no caso da funcao exponencial, um algoritmo que utiliza-lo é ligeramente melhor que uma operacao com n operacoes aninhadas
## 5 Problema
### O que é complexidade de tempo?

##### É uma função que representa o número máximo de passos de um algoritmo.
## 6 Problema
### Dado dois algoritmos A e B com as complexidades de tempo respectivamente f1 e f2, qual é o melhor algoritmo? O que indica qual é o melhor algoritmo?

##### Considerando A e B dois algoritmos totalmentes diferentes, é selecionado o melhor aquele que é executado com menores números de passos à finalização da execução e aquele que tem uma menor complexidade de tempo.
## 7 Problema
### Em uma funcao de complexidade, o que representa o termo n?

##### Em uma função de complexidade o termo “n” é considerado como o comprimento da entrada.
## 8 Problema
### Quais sao as operacoes primitivas de um algoritmo?

##### As operações primitivas de um algoritmo são:

     Atribuição de valores a variáveis;
     Chamadas de métodos;
     Operações aritméticas;
     Comparação de dois números;
     Acesso a um arranjo;
     Seguimento de uma referência para um objeto;
     Retorno de um método.

## 9 Problema
### Qual é o valor de uma operacao primitiva de um algoritmo?

##### Para cada valor de uma operação primitiva de um algoritmo é atribuído o valor 1.
## 10 Problema
### Desenvolva o pseudocódigo do algoritmo SOMA, que realiza a soma de dois números inteiros recebidos por parâmetro e tem como saída a resultado da operacao. Identifique a sua funcao de complexidade de tempo.

##### 1 - res <- a + b
##### 2 - retorna res;

##### f(n) = c1 . 1 + c2 . 1 f(n) = 1 + 1 f(n) = 2
## 11 Problema
### Desenvolva o pseudocódigo do algoritmo SOMA VETOR, que realiza a soma de todos os elementos de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo.

##### 1 - aux <- 0;
##### 2 - N <- comprimento V;
##### 3 - para i <- 1 até N:
##### 4 -     soma <- aux+ V[i];
##### 5 -     i <- i + 1;
##### 6 - retorna soma;

##### O número de vezes no "for" assume o valor de n : f(n) = c1 . 1 + c2 . 1 + c3 . n + c4 . n + c5 . n + c6 . 1 f(n) = 1 + 1 + n + n + n + 1 f(n) = 3n + 3
## 12 Problema
### Desenvolva o pseudocódigo do algoritmo CONTA EM IMPARES, que realiza a contagem de números ímpares de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua fun¸c˜ao de complexidade de tempo.

##### 1 - cont <- 0;
##### 2 - N < comprimento V;
##### 3 - para i <- 1 até N:
##### 4 - se V[i]%2 != 0:
##### 5 - cont <- cont + 1
##### 7 - i <- i + 1
##### 8 - retorna cont;

##### Acontece a mesma coisa que no problema anterior com o "for" e no condicional "if" ou "se" também assume o valor de n. f(n) = c1 . 1 + c2 . 1 + c3 . n + c4 . n + c5 . n + c6 . n + c7 . 1 f(n) = 1 + 1 + n + n + n + n + 1 f(n) = 4n + 3
## 13 Problema
### Desenvolva o pseudocódigo do algoritmo SOMA MATRIZ, que realiza a soma de todos os elementos de uma matriz. O algoritmo recebe a matriz M e tem como saída o resultado. Identifique a sua função de complexidade de tempo.

##### 1 - soma <- 0;
##### 2 - N <- comprimento M;
##### 3 - para i <- até N:
##### 4 - para j <- 1 até N:
##### 5 - soma <- soma + M[i][j]
##### 6 - j <- j + 1
##### 7 - i <- i + 1
##### 8 - retorna soma;

##### f(n) = 1 + 1 + n + n * n + n * n + n * n + n + 1 f(n) = 3n² + 2n + 3
## 14 Problema
### Desenvolva o pseudocódigo do algoritmo BUSCA MATRIZ, que identifica posição x e y de um elemento em uma matriz. O algoritmo recebe a matriz M e o valor V e tem como saída a posição x e y . Identifique a sua função de complexidade de tempo.

##### 1 - N <- comprimento M;
##### 2 - para i <- 1 até N:
##### 3 -     para j <- 1 até N:
##### 4 -     se M[i][j] = V:
##### 5 -         retorna M[i][j];
##### 6 -         j <- j + 1;
##### 7 -         i <- i + 1;
##### 8 - retorna M;

##### f(n) = 1 + n + n² + n² + n² + n² + n + 1 f(n) = 4n² + 2n + 2
## 15 Problema
### O que é análise assintótica? Qual é o seu objetivo?

##### A análise assintótica é uma aproximação do tempo de execução para entradas de dados grandes; seu objetivo é descrever o comportamento de limites.
## 16 Problema
### Qual é o processo da análise assintótica? Crie um exemplo.

<img src="C:\Users\marce\Desktop" alt="Fluxo" />

    No primeiro caso define a variável f(n)
    Identificar o componente de maior ordem.
    6n³
    Ignorar os coeficientes.
    n³

## 17 Problema
### O que é a notação assintótica?

##### A notação assintótica ou notação Big-Oh é utilizada para descrever o relacionamento de f(n) = O(n³)
## 18 Problema
### O que é a notação O-Grande ou Big-Oh?

##### A notação Big-Oh diz que uma função é menor que ou igual a outra função g(n).
## 19 Problema
### Qual é a definicao formal da notacao O-Grande?

##### Formalmente é definido a notação do Big-Oh como: R+ onde ele é o conjunto dos números reais negativos.
## 20 Problema
### Crie um gráfico explicando a notacao O-grande. Utilize f(n) = 2n + 4. Qual é um valor possível para n0?

<img src="http://cdn.osxdaily.com/wp-content/uploads/2013/07/dancing-banana.gif" alt="Banana" /> 

##### O valor para n0 é n=5 || f(x)=14. O valor representado no gráfico é a barra laranja.
## 21 Problema
### O que é a notacao o-pequeno ou Little-Oh?

##### É uma notação a qual diz que uma função é menor que a outra.
## 22 Problema
### Qual é a definicao formal da notacao o-pequeno?

##### Definição formal: f (n) = o (g (n)) significa que para todo c> 0 existe algum k> 0 tal que 0 ≤ f (n) <cg (n) para todo n ≥ k. O valor de k não deve depender de n, mas pode depender de c. Onde R+ é o conjunto dos reais não negativos.
## 23 Problema
### Crie um gráfico explicando a notacao o-pequeno.

##### image Notação do Little-Oh diz que uma função é menor que a outra função g(n). Ou seja, f é dominada por g assintoticamente. A diferença entre Big-Oh e Little-Oh é análoga àquela entre ≤ e <.
## 24 Problema
### Passe a notacao O-grande e o-pequeno as funcoes abaixo:

    A F(n) = n + 1
    B F(n) = 8
    C F(n) = 2n
    2 − 1
    D F(n) = nlogn
    E F(n) = 3n! + 2n
    F F(n) = 3n
    3 + 2n
    2 + 4n + 6
    G F(n) = 5n + 11
    H F(n) = 3logn

<img src="http://cdn.osxdaily.com/wp-content/uploads/2013/07/dancing-banana.gif" alt="Banana" />

## 25 Problema
### Identifique o O-Grande dos algoritmos desenvolvidos nos Problemas 10 até 14.

#### Problema 10 f(n)=2 Big-O = 1

#### Problema 11 f(n) = 3n+3 Big-O = n

#### Problema 12 f(n) = 4n+3 Big-O = n

#### Problema 13 f(n) = 3n² + 2n + 3 Big-O = n²

#### Problema 14 f(n) = 4n² + 2n + 2 Big-O = n²
