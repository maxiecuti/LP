```mermaid

flowchart TD
  inicio(( Início )) --> entradaNota[\ Digite sua nota \]
  entradaNota --> entradaFrequencia[\ Digite sua frequência em %\]

  entradaFrequencia --> validarNota{ Nota entre 0 e 100? }
  validarNota --> |Não| notaInvalida[/ Nota inválida /]
  notaInvalida --> fim([ Fim ])

  validarNota --> |Sim| validarFrequencia{ Frequência entre 0% e 100%?}
  validarFrequencia --> |Não| frequenciaInvalida[/ Frequencia inválida /]
  frequenciaInvalida --> fim

  validarFrequencia --> |Sim| verificarAprovacao{ Nota ≥ 50 e Frquência ≥ 75%? }
  verificarAprovacao --> |Sim| aprovado[/ Aprovado /]
  verificarAprovacao --> |Não| reprovado[/ Reprovado /]

  aprovado --> fim
  reprovado --> fim

