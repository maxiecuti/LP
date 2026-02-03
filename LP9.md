```mermaid

flowchart TD
  inicio(( Início )) --> entrada[/Ler número N/]
  entrada --> decisao{N % 2 == 0?}
  decisao -- Sim --> resultadoPar[Número é par]
  decisao -- Não --> resultadoImpar[Número é ímpar]

  resultadoPar --> fim(( Fim ))
  resultadoImpar --> fim
