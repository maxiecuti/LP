```mermaid

flowchart TD
  inicio(( Início )) --> entrada[\Ler idade inserida\]
  entrada --> calcular{Idade ≥ 16?}

  calcular -- Sim --> maior[Você pode votar🎊]
  calcular -- Não --> menor[Você não pode votar🤷‍♂️]
  
  maior --> Fim[Fim]
  menor --> Fim[Fim]