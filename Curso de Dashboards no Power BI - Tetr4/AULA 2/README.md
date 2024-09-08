
# Dashboard de Logística 

## Roteiro da Atividade

- Neste relatório consta o resumo das encomendas entregues pela empresa nos anos de 2021 e 2022.

## Indicadores

- O valor total da receita líquida de fretes em cada ano;
- O custo total das encomendas em cada ano;
- A quantidade de pedidos entregues em cada ano;
- A quantidade de pedidos que foram entregues atrasados em cada ano;
- A quantidade de devoluções em cada ano;
- A evolução da quantidade de pedidos por mês dentro de cada ano;
- A quantidade de pedidos atrasados e no prazo por cada tipo de veículo;
- A porcentagem de entregas que foram feitas atrasadas e no prazo;
- A quantidade de pedidos por estado;
- Os principais motivos de devolução;
- A variação percentual da receita líquida de fretes, custo de encomendas, quantidade de pedidos, entregas atrasadas e devoluções de 2022 em relação a 2021.


## Medidas
O dashboard de LOGÍSTICA contém as seguintes medidas.

### 🧮 Receita líquida de fretes:
        ReceitaFretes = SUM(Pedidos[Valor do Frete])

### 🧮 Quantidade de pedidos:
        QtdPedidos = COUNTROWS(Pedidos)

### 🧮 Custo das entregas:
        Custo = SUM(Pedidos[Custo de Entrega])

### 🧮 Variação da Receita:
        %Receita =
        var Receita = [ReceitaFretes] 
        var ReceitaLY = CALCULATE([ReceitaFretes],
        SAMEPERIODLASTYEAR(Pedidos[Data Pedido].[Date])
        RETURN 
        DIVIDE(Receita - ReceitaLY,ReceitaLY,0)

### 🧮 Variação da quantidade de pedidos:
        %Pedidos = 
        var Pedido = [QtdPedidos]
        var PedidoLY = CALCULATE([QtdPedidos], 
        SAMEPERIODLASTYEAR(Pedidos[Data Pedido].[Date])
        RETURN 
        DIVIDE(Pedido - PedidoLY,PedidoLY,0)

### 🧮 Variação do custo de entrega:
        %Custo =
        var Custo = [Custo]
        var CustoLY = CALCULATE([Custo],
        SAMEPERIODLASTYEAR(Pedidos[Data Pedido].[Date])
        RETURN
        DIVIDE(Custo - CustoLY,CustoLY,0)

## Tecnologias

- Power BI

## Instalação

Para acessar o dashboard, basta abrir o arquivo .pbix usando o Power BI

## Uso

O uso do dashboard é intuitivo e fácil de entender. Cada visualização é interativa e permite filtrar dados e visualizar informações de diferentes maneiras. Basta selecionar a visualização desejada e começar a explorar os dados.

## Visualização do Dashboard

![dash logistica](https://github.com/user-attachments/assets/db70513e-7a68-47a5-ba3f-c4f89229a620)
