
# Dashboard de Pesquisa de Satisfação dos Colaboradores  - Empowerdata

## Roteiro da Atividade

- Este relatório teve como objetivo principal, realizar a análise exploratória dos dados e em seguida criar a Visualização do dados facilitando a tomada de decisão.  

## Indicadores

- Total de perguntas respondidas    ;
- Quantidade de cargos;
- Total de Funcionários;
- Range de idade; 
- Fonte de recrutamento;
- Quantidade de ffuncionários por ano;
- Comparativo de Satisfação.


## Medidas
O dashboard *Pesquisa de Satisfação* contém as seguintes medidas.

### Quantidades de Cargos 
```javascript
Qtde Cargos = DISTINCTCOUNT(bd_integrantes[Cargo])
```

### Quantidades de Funcionários 
```javascript
qtde de funcionarios = COUNTROWS(bd_integrantes)
```

### Quantidades de Perguntas
```javascript
qtde de Perguntas = COUNTROWS(Entrevistas)
```

## Ferramentas

- Power BI

## Compartilhamento

Para acessar o dashboard, basta abrir o arquivo no power BI Desktop.
 

## Uso

O uso do dashboard é intuitivo e fácil de entender. Cada visualização é interativa e permite filtrar dados e visualizar informações de diferentes maneiras. Basta selecionar a visualização desejada e começar a explorar os dados.

## Visualização do Dashboard

### 💻Desktop
![pesquisa de satisfação](https://github.com/user-attachments/assets/f814108e-c8e6-4899-b830-b942cf8deceb)