# Testando Threads

Linha de execução (em inglês: thread), é uma forma de um processo dividir a si mesmo em duas ou mais tarefas que podem ser executadas concorrentemente. O suporte à thread é fornecido pelo próprio sistema operacional (SO), no caso da linha de execução ao nível do núcleo (em inglês: Kernel-Level Thread (KLT)), ou implementada através de uma biblioteca de uma determinada linguagem, no caso de uma User-Level Thread (ULT). 

Uma Thread é "um fluxo de controle sequencial isolado dentro de um programa". Como um programa sequencial qualquer, uma thread tem um começo, um fim, e uma seqüência de comandos. Entretanto, uma thread não é um programa, não roda sozinho, roda dentro de um programa. Threads permitem que um programa simples possa executar várias tarefas diferentes ao mesmo tempo, independentemente umas das outras. Uma thread sempre realiza determinada tarefa codificada em um método. Programas multi-threaded são programas que contém vários threads, executando tarefas distintas, ao mesmo tempo. 

Threads, sequências, linhas de execução, encadeamento não importa o nome, todas as aplicações são executadas em uma thread principal. Um programa C# quer do tipo Console, WPF ou Windows Forms inicia em uma única thread criada de forma automática pela CLR (Common Languagem Runtime) e pelo Sistema Operacional (a thread principal - main) e torna-se multithread pela criação de threads adicionais.

Por exemplo, vamos pensar em um jogo de vídeo game. Imagine um jogo possuindo uma única thread, tanto para o processamento de imagens quanto para o processamento de áudio. Seria possível? Sim, seria. Mas esse é o cenário ideal para garantir a performance? Não. O ideal seria criar threads para o processamento das rotinas de imagens e outra para rotinas de áudio.
