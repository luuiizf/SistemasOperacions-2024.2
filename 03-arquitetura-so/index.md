# Arquiteturas de Sistemas Operacionais

## Informações gerais

- Capítulo: [Arquitetura de SO](https://wiki.inf.ufpr.br/maziero/lib/exe/fetch.php?media=socm:socm-03.pdf)
- Disciplina: *sistemas operacionais*
- Livro: [Sistemas Operacionais: Conceitos e Mecanismos](https://wiki.inf.ufpr.br/maziero/doku.php?id=socm:start)

## Aluno

- nome: Luiz Fernando Gama Nery
- matrícula: 20232014040019

## Respostas dos exercícios

1.
Arquitetura	| Benefícios | Deficiências
------------------------------------------
Monolítica |	Alta performance devido à execução direta no núcleo; eficiente na comunicação entre componentes. |	Difícil manutenção e adição de novos recursos; menos segura, pois falhas podem afetar todo o sistema.
------------------------------------------
Micronúcleo |	Maior segurança e confiabilidade; fácil de manter e adaptar. |	Menor performance devido à comunicação entre processos no espaço do usuário; mais complexa.
------------------------------------------
Híbrida	| Combina vantagens do monolítico e micronúcleo, como flexibilidade e performance balanceada. |	Pode aumentar a complexidade e o custo de implementação; compromisso entre performance e segurança.

2.
O núcleo do Linux é considerado monolítico, pois a maioria dos seus serviços e funcionalidades está incorporada diretamente no kernel, o que permite maior eficiência e performance. No entanto, ele possui algumas características de micronúcleo, como módulos carregáveis, que podem ser adicionados ou removidos dinamicamente, proporcionando uma certa modularidade e flexibilidade.

3.
(a) Incorreta. Uma máquina virtual de sistema não é construída para suportar apenas uma aplicação específica em uma linguagem específica, como Java. Máquinas virtuais de sistema, como o Hypervisor, suportam múltiplos sistemas operacionais e não são limitadas a uma única linguagem de programação.

(b) Correta. Um hypervisor convidado realmente executa sobre um sistema operacional hospedeiro.

(c) Incorreta. Em um sistema operacional micronúcleo, os componentes são executados fora do núcleo, em espaço de usuário, e se comunicam via troca de mensagens. No entanto, a afirmação sugere que os módulos executam dentro do núcleo, o que é uma característica de sistemas monolíticos.

(d) Incorreta. Núcleos monolíticos são robustos e podem ser eficientes, mas são mais difíceis de manter devido à sua estrutura integrada, onde falhas em um módulo podem comprometer todo o sistema.

(e) Correta. Em sistemas operacionais de micronúcleo, as chamadas de sistema são geralmente implementadas através de troca de mensagens, pois os componentes principais operam no espaço do usuário e se comunicam com o núcleo através de mensagens.
