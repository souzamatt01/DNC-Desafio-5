# DNC-Desafio-5

Quinta prova da formação em Cientista de Dados pela Escola DNC

**Arquivo da Base de Dados utilizada se encontra dentro deste repositório com o nome : "dataset_DESAFIO5"**

**Contexto:** Uma empresa do ramo de e-commerce contratou você para levantar os indicadores de recência, frequência e ticket médio (RFM) dos seus clientes.

A saber RFM:

- R (Recency): Tempo que o cliente realizou a última compra (em dias)
- F (Frequency): Quantidade de compras realizadas pelo cliente
- M (Monetary): Valor do ticket médio gasto pelo cliente onde ticket médio = média do total gasto por pedido para cada cliente.


**Critérios de Avaliação:**
- **Leia o arquivo e inspecione os dados:** Utilize o describe para verificar a distribuição dos dados.
- **Verifique se há valores faltantes na identificação do cliente:** Certifique-se de verificar os valores nulos com o isna e utilize a função sum para a somar a quantidade de nulos e a função dropna para remover estes nulos.
- **Verifique se há produtos com preços unitários iguais ou inferior a 0:** Utilize filtros para: verificar se existem dados nulos ou menor que zero na coluna de preços.
- **Verifique se há produtos com quantidade igual ou inferior a 0:** Utilize filtros para verificar a existência de dados nulos ou menor que zero na coluna de quantidade.
- **Verifique se existem linhas duplicadas:** Utilize a função duplicated para verificar as linhas duplicadas, drope essas linhas e as remova.
- **Tipos de dados da coluna:** Corrija o tipo de dado do CustomerID (tipo esperado: int) e o tipo de dado da InvoiceDate (tipo esperado: datetime).
- **Tratando os outliers:** Remova os outliers extremos em que a quantidade do item na compra é superior a 10.000 e o preço unitário é maior que 5.000.
- **Crie uma coluna adicional:**  Utilize as colunas Quantity e UnitPrice para criar uma coluna adicional com o preço total da compra.
- **Última data:** Utilize a função max() para calcular e identificar a data da última compra no dataset.
- **Plotando gráficos:** Plote 5 gráficos, que contenham os seguintes dados: Top 10 países com maior valor em vendas; Top 10 produtos mais vendidos; Valor de venda total por mês; Valor de venda total por mês e por país (considere apenas os top 10).
- **Cálculo do RFM:** Agrupe os dados por cliente e pedido/compra (InvoiceNo) e obtenha a data e o preço total do pedido.
Com isso, agrupe novamente apenas por cliente e calcule o RFM, onde:

- R é a recência, diferença em dias da última compra do cliente e da última compra disponível no conjunto de dados, que calcularam previamente.
- F é a frequência, ou seja, a quantidade de compras feitas pelo cliente;
- M é o ticket médio, ou seja, a média das compras feitas pelo cliente.

  **Código comentado no Google Colab se encontra disponível dentro desse Repositório.**
