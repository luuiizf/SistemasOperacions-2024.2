# Conceito de tarefas

## Informações gerais

- Capítulo: [Conceito de tarefas](https://wiki.inf.ufpr.br/maziero/lib/exe/fetch.php?media=socm:socm-04.pdf)
- Disciplina: *sistemas operacionais*
- Livro: [Sistemas Operacionais: Conceitos e Mecanismos](https://wiki.inf.ufpr.br/maziero/doku.php?id=socm:start)

## Aluno

- nome: Luiz Fernando Gama Nery
- matrícula: 20232014040019

## Respostas dos exercícios

1.
É a técnica que permite que várias tarefas compartilhem o processador de forma interativa, atribuindo "fatias" de tempo a cada uma. Isso garante que várias tarefas possam ser atendidas ao mesmo tempo, essencial para manter o sistema eficiente e responsivo.

2.
O tempo de quantum é ajustado para equilibrar responsividade e eficiência. Um quantum curto aumenta a responsividade, enquanto um quantum longo reduz as trocas de contexto. A escolha depende da prioridade e do tipo de tarefas em execução.

3.
Transição faltante (t6): 
S (Suspensa) → P (Pronta): Ocorre quando o evento ou o recurso que a tarefa aguardava fica disponível, permitindo que a tarefa retorne ao estado de pronta para execução.

Significado dos estados e transições:
N (Nova): Tarefa sendo criada, carregando código e dados necessários para execução.
P (Pronta): Tarefa apta a executar, aguardando disponibilidade do processador.
E (Executando): Tarefa em execução ativa no processador.
S (Suspensa): Tarefa em espera, aguardando um recurso ou evento externo.
T (Terminada): Tarefa concluída ou abortada.
t1 (Nova → Pronta): Tarefa carregada e pronta para iniciar.
t2 (Pronta → Executando): Tarefa selecionada pelo escalonador para execução.
t3 (Executando → Pronta): O quantum de tempo da tarefa se esgota.
t4 (Executando → Suspensa): Tarefa requer um recurso indisponível.
t5 (Executando → Terminada): Tarefa conclui sua execução.
t6 (Suspensa → Pronta): O recurso aguardado pela tarefa está disponível.

4.
E → P (Executando → Pronta): Possível. O quantum da tarefa termina, retornando-a ao estado de pronta.
E → S (Executando → Suspensa): Possível. A tarefa necessita de um recurso externo (ex: leitura de disco).
S → E (Suspensa → Executando): Não é possível diretamente; a tarefa deve passar pelo estado "Pronta" antes de retornar ao processador.
P → N (Pronta → Nova): Não é possível. Tarefas prontas já foram carregadas e preparadas para execução.
S → T (Suspensa → Terminada): Possível em caso de erro fatal enquanto a tarefa aguarda um recurso.
E → T (Executando → Terminada): Possível. A tarefa conclui ou é encerrada por erro.
N → S (Nova → Suspensa): Não é possível. Tarefas novas precisam ser carregadas e passar pelo estado de "Pronta" antes de serem suspensas.
P → S (Pronta → Suspensa): Possível se a tarefa aguarda uma condição antes de executar.

5.
O código da tarefa está sendo carregado. - (N) Nova
A tarefas são ordenadas por prioridades. - (P) Pronta
A tarefa sai deste estado ao solicitar uma operação de entrada/saída. - (E) Executando
Os recursos usados pela tarefa são devolvidos ao sistema. - (T) Terminada
A tarefa vai a este estado ao terminar seu quantum. - (P) Pronta
A tarefa só precisa do processador para poder executar. - (P) Pronta
O acesso a um semáforo em uso pode levar a tarefa a este estado. - (S) Suspensa
A tarefa pode criar novas tarefas. - (E) Executando
Há uma tarefa neste estado para cada processador do sistema. - (E) Executando
A tarefa aguarda a ocorrência de um evento externo. - (S) Suspensa