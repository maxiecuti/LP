```mermaid

flowchart TD
  inicio(( Início )) --> entrada[\ Ler número A \]
  entrada --> entradaDois[\ Ler número B \]

  entradaDois --> calculo{A > B?}
  calculo -- Sim --> resultadoA[A é o maior]

  entradaDois --> calculoDois{B > A?}
  calculoDois -- Sim --> resultadoB[B é o maior]

  entradaDois --> resultadoC[Os números são iguais]

  resultadoA --> Fim[Fim]
  resultadoB --> Fim[Fim]
  resultadoC --> Fim[Fim]
