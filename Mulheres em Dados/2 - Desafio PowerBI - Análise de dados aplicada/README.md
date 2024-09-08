
# Dashboard da Copa do Mundo Feminina

## Roteiro da Atividade

- Este relatório teve como objetivo principal, a análise dos dados da Copa do Mundo de Futebol Feminino. 

## Indicadores

- Total de público;
- Ano com maior média de público;
- Maior média de público;
- Países que já sediaram a copa;
- Evolução de público nas copas;
- Total de gols;
- Total de gols por país.


## Medidas
O dashboard FINANCEICO contém as seguintes medidas. 

### Maior média de público
       Maior média de publico = MAXX(Hosts,Hosts[Average Attendance])

### Ano com maior média de público
           Ano Com maior Media = CALCULATE(SELECTEDVALUE(Hosts[Year]), Hosts[Average Attendance]=MAXX(Hosts,Hosts[Average Attendance]))

### Paises que mais sediaram copas 
        Paises mais sediaram = CALCULATE(COUNT(Hosts[Country_ID]),USERELATIONSHIP(Hosts[Country_ID],DimCountry[Country_ID]))


## Tecnologias

- Power BI

## Instalação

Para acessar o dashboard, basta abrir o arquivo .pbix usando o Power BI

## Uso

O uso do dashboard é intuitivo e fácil de entender. Cada visualização é interativa e permite filtrar dados e visualizar informações de diferentes maneiras. Basta selecionar a visualização desejada e começar a explorar os dados.

## Visualização do Dashboard

![dasho copa feminina 1](https://github.com/user-attachments/assets/3269d39f-5b2c-44a1-925d-795b75f228ba)

![dasho copa feminina 2](https://github.com/user-attachments/assets/6c548393-d6d1-4648-880e-979dbea25643)

![dasho copa feminina 3](https://github.com/user-attachments/assets/376e7250-ec0b-4f01-a67c-04568a0e754f)

![dasho copa feminina 4](https://github.com/user-attachments/assets/4c085614-9a11-4d5f-b3c1-de2daa3a94a8)
