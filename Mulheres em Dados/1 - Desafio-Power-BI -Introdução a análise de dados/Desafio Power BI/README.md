
# Dashboard de Análise de dados 2022

## Roteiro da Atividade

- Este relatório teve como objetivo principal, a análise do Financeiro da empresa fictícia. 

## Indicadores

- Faturamento líquido;
- Faturamento Bruto;
- Total de vendas;
- Evolução de Faturamento líquido e bruto;
- Faturamento por Região;
- Faturamento por segmento.


## Medidas
O dashboard FINANCEICO contém as seguintes medidas. 

### Total de vendas 
       Total_vendas = SUMX(fVendas,fVendas[Valor Unitário])

### Total Faturamento sem desconto 
           Total_Faturado_semDesconto = [Total_unitário] * [Total_vendas]

### Indicador de Crescimento 
          Indicador_crescimento = SWITCH(TRUE(), 
    [Total_Líquido]>[Faturamento_Ano_Anterior],"🟢 Crescimento",
    [Total_Líquido]=[Faturamento_Ano_Anterior],"🟡 Manteve", 
    [Total_Líquido]<[Faturamento_Ano_Anterior],"🔴 Queda", 
    BLANK())

### Média de vendas 
        Média_vendas = AVERAGEX(fVendas,[Total_Líquido])

## Tecnologias

- Power BI

## Instalação

Para acessar o dashboard, basta abrir o arquivo .pbix usando o Power BI

## Uso

O uso do dashboard é intuitivo e fácil de entender. Cada visualização é interativa e permite filtrar dados e visualizar informações de diferentes maneiras. Basta selecionar a visualização desejada e começar a explorar os dados.

## Visualização do Dashboard

![Overview financeiro](https://github.com/user-attachments/assets/704676d7-6266-423b-b21b-be60f17332db)
![Resumo financeiro](https://github.com/user-attachments/assets/64a54435-6450-4d03-8b3c-0e7406f09beb)
![overview cliente](https://github.com/user-attachments/assets/1fd55e97-c337-4555-a73d-9be911b6a9d3)
![Resumo cliente ](https://github.com/user-attachments/assets/a42e02ae-444e-4546-9541-4e6cda75797c)
