# Implementação de tarefas

## Informações gerais

- Capítulo: [Implementação de tarefas](https://wiki.inf.ufpr.br/maziero/lib/exe/fetch.php?media=socm:socm-05.pdf)
- Disciplina: *sistemas operacionais*
- Livro: [Sistemas Operacionais: Conceitos e Mecanismos](https://wiki.inf.ufpr.br/maziero/doku.php?id=socm:start)

## Aluno

- nome: Luiz Fernando Gama Nery
- matrícula: 20232014040019

## Respostas dos exercícios

1.
O TCB (Task Control Block) é uma estrutura de dados usada em sistemas operacionais para armazenar as informações necessárias ao gerenciamento de uma tarefa. Ele contém dados como o identificador da tarefa, seu estado (ex.: pronta, executando), valores dos registradores do processador, áreas de memória em uso e recursos alocados, como arquivos abertos.

3.
A quantidade exata depende do comportamento dos forks() e do valor N, o que resulta em 2^N saídas de "X".

4.
Threads são fluxos de execução independentes que compartilham o mesmo espaço de memória dentro de um processo. São usadas para realizar múltiplas operações concorrentes em uma aplicação, aumentando a eficiência e permitindo a execução paralela de tarefas relacionadas.

5.
Vantagens: Menor custo para criação, troca de contexto mais rápida e uso mais eficiente de memória.
Desvantagens: Menor robustez e segurança, pois um erro em uma thread pode comprometer todo o processo.

6.
Algoritmos sequenciais sem possibilidade de paralelismo, como o cálculo de uma sequência Fibonacci iterativa.
Leitura de um arquivo pequeno onde o tempo de I/O é irrelevante e não há necessidade de processamento paralelo.

7.
(a) N:1
(b) N
(c) 1:1
(d) N:1
(e) N
(f) N:1
(g) 1:1
(h) N:1
(i) 1:1
(j) N