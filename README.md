# Algoritmos de Ordenação

## Sobre
Este repositório contém um programa em C++ que implementa e compara diferentes algoritmos de ordenação. O objetivo é avaliar a eficiência dos seguintes métodos:

- **Seleção** (Selection Sort)
- **Inserção** (Insertion Sort)
- **Merge Sort**

O programa recebe um conjunto de números inteiros da entrada padrão, aplica um dos algoritmos de ordenação e mede o tempo de execução.

## Compilação
Para compilar o programa, utilize o seguinte comando:

```sh
g++ -Wall -o teste_ordenacao teste_ordenacao.cpp ordenacao.cpp
```

## Execução
O programa pode ser executado da seguinte forma:

```sh
./teste_ordenacao
```

Por padrão, a ordenação utilizada é a **seleção**. Para escolher um algoritmo diferente, utilize uma das opções abaixo:

```sh
./teste_ordenacao -s   # Selection Sort
./teste_ordenacao -i   # Insertion Sort
./teste_ordenacao -m   # Merge Sort
```

Para visualizar o manual do programa:

```sh
./teste_ordenacao -h
```

## Testes com Arquivos
Os testes podem ser realizados utilizando arquivos de entrada e saída:

```sh
./teste_ordenacao < entrada.txt > saida.txt
```

Exemplo de uso com diferentes algoritmos:

```sh
./teste_ordenacao -s < e1.txt > s1.txt   # Selection Sort
./teste_ordenacao -i < e1.txt > s1.txt   # Insertion Sort
./teste_ordenacao -m < e1.txt > s1.txt   # Merge Sort
```

## Estrutura do Código

- `teste_ordenacao.cpp`: Arquivo principal que gerencia a entrada e a execução do algoritmo escolhido.
- `ordenacao.hpp`: Cabeçalho com as assinaturas das funções de ordenação.
- `ordenacao.cpp`: Implementação dos algoritmos de ordenação.

## Considerações
O tempo de execução de cada algoritmo é exibido na saída de erro, permitindo a comparação entre os métodos de ordenação.

Este projeto foi desenvolvido como parte de uma atividade acadêmica.

