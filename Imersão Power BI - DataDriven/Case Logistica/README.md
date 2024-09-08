
# Dashboard de Logística

## Roteiro da Atividade

- Este relatório teve como objetivo principal, a análise da malha logística. 

## Indicadores

- Custo do frete;
- Performance de transportes;
- Tipos de veículos mais utilizados;
- OTD ( on time Delivery);
- Malha logística.


## Medidas
O dashboard FINANCEICO contém as seguintes medidas. 

### % OTD (On Time Delivery)
            % OTD = DIVIDE([Qtd no Prazo],[Total de Viagens])

### Meta 
            Meta = 0.80

### Qtdo no prazo

           Qtd no Prazo = 
    CALCULATE([Total de Viagens],'Histórico de Transporte'[Status Transporte]= "Dentro do Prazo")

### Total de viagens 

        Total de Viagens = COUNTROWS('Histórico de Transporte')

## Tecnologias

- Power BI

## Instalação

Para acessar o dashboard, basta abrir o arquivo .pbix usando o Power BI

## Uso

O uso do dashboard é intuitivo e fácil de entender. Cada visualização é interativa e permite filtrar dados e visualizar informações de diferentes maneiras. Basta selecionar a visualização desejada e começar a explorar os dados.

## Visualização do Dashboard

![dash logística](https://github.com/user-attachments/assets/659c0ab1-0591-4ed5-98e4-1be9b52bc1c8)
