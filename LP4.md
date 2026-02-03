```mermaid

flowchart TD
  inicio(( Início )) --> entrada[\ Digite o numero \]
  entrada --> positivoNegativo{ O Número é negativo ou positivo? }

  positivoNegativo --> |Positivo| numeroPositivo[/ Número ≥ 0 /]
  numeroPositivo --> fim([ Fim ])

  positivoNegativo --> |Negativo| numeroNegativo[/ Número ≤ 0 /]
  numeroNegativo --> fim([ Fim ])

