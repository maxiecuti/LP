```mermaid

flowchart TD
  inicio(( Início )) --> entrada[\ Digite sua nota \]
  entrada --> validarNota{ Nota entre 0 e 100? }

  validarNota --> |Não| notaInvalida[/ Nota inválida /]
  notaInvalida --> fim([ Fim ])

  validarNota --> |Sim| verificarAprovacao{ Nota ≥ 50? }
  verificarAprovacao --> |Sim| aprovado[/ Aprovado /]
  verificarAprovacao --> |Não| reprovado[/ Reprovado /]

  aprovado --> fim
  reprovado --> fim
