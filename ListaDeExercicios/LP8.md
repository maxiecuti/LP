```mermaid

flowchart TD
  inicio(( Início )) --> entrada[/Ler número N/]
  entrada --> init[Definir fatorial = 1]
  init --> initI[Definir i = 1]

  initI --> decisao{i <= N?}
  decisao -- Sim --> calculo[fatorial = fatorial * i]
  calculo --> incremento[i = i + 1]
  incremento --> decisao

  decisao -- Não --> resultado[/Resultado fatorial/]
  resultado --> fim(( Fim ))
