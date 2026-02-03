```mermaid

flowchart TD

  inicio(( Início )) --> entrada[\ Ler número A \]
  entrada --> entradaDois[\ Ler número B \]
  entradaDois --> entradaTres[\ Ler número C \]

  entradaTres --> comparacaoA{A >= B?}
  comparacaoA -- Sim --> comparacaoA2{A >= C?}
  comparacaoA2 -- Sim --> resultadoA[A é o maior]
  comparacaoA2 -- Não --> resultadoC[C é o maior]

  comparacaoA -- Não --> comparacaoB{B >= C?}
  comparacaoB -- Sim --> resultadoB[B é o maior]
  comparacaoB -- Não --> resultadoC[C é o maior]

  resultadoA --> Fim[Fim]
  resultadoB --> Fim[Fim]
  resultadoC --> Fim[Fim]
