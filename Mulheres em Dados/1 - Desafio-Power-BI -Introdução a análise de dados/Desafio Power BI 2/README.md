
# Dashboard de Análise de dados 2022 (Visual 2)

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

![visão de faturamento](https://github.com/user-attachments/assets/0c420a40-50f1-412f-9862-3bc17b76f252)

![Resumo financeiro](https://github.com/user-attachments/assets/70f24bdd-f6e9-463f-8fa5-4a03ff8c03f6)

![Visão do cliente](https://github.com/user-attachments/assets/ea04e618-cc47-4b50-be1f-386a47c7e5a3)

![Resumo do cliente ](https://github.com/user-attachments/assets/452f89e6-eb4f-4542-878a-c5079bde88af)
