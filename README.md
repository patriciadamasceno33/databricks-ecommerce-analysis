# Analise-de-Dados-de-E-commerce-com-Databricks
Este projeto tem como objetivo analisar dados reais de um e-commerce brasileiro, construindo um pipeline completo de dados e gerando insights estratégicos para o negócio.

A solução foi desenvolvida utilizando Databricks, com foco em organização de dados em camadas (Bronze, Silver e Gold) e análises voltadas para tomada de decisão.

O Objetivo foi
Construir um pipeline de dados estruturado
Realizar tratamento e padronização dos dados
Integrar múltiplas tabelas relacionais
Gerar análises de faturamento e comportamento de clientes
Demonstrar habilidades práticas como analista de dados


Tecnologias utilizadas:
Python (PySpark),
SQL,
Databricks e
Modelo de dados em camadas (Medallion Architecture).


Arquitetura de Dados - 
O projeto segue a arquitetura em três camadas:

Bronze:
Dados brutos carregados diretamente dos arquivos CSV
Sem tratamento ou transformação

Silver:
Dados limpos e tratados
Remoção de duplicidades
Padronização de colunas
Filtragem de dados relevantes (ex: pedidos entregues)

Gold:
Dados consolidados para análise
Integração entre pedidos, pagamentos e itens
Preparação para geração de insights


Modelagem dos Dados - 
Relacionamentos principais:

Clientes ↔ Pedidos → customer_id

Pedidos ↔ Itens → order_id

Pedidos ↔ Pagamentos → order_id


Análises Realizadas:
Faturamento ao longo do tempo;
Análise do crescimento mensal do faturamento, identificando tendências de expansão do negócio.

<img width="1009" height="289" alt="evolucao_faturamento_mensal" src="https://github.com/user-attachments/assets/6b5b7ee2-8471-4952-b2aa-1de131c24bc6" />


Top clientes:
Identificação dos clientes com maior volume de compras.

<img width="501" height="335" alt="image" src="https://github.com/user-attachments/assets/7e99fe2a-90b9-43f6-bdf0-55f49d06b522" />


Produtos mais vendidos:
Análise de volume de vendas por produto.


<img width="501" height="336" alt="image" src="https://github.com/user-attachments/assets/48cfe671-30b9-4b51-ae87-7ef3c49ee657" />


Principais Insights:
Houve crescimento consistente do faturamento ao longo de 2017, indicando expansão da operação.
Os primeiros meses apresentam baixa volumetria, sugerindo fase inicial do negócio.
A receita está concentrada em uma parcela menor de clientes, indicando comportamento compatível com o princípio de Pareto.
Alguns produtos apresentam alto volume de vendas, mas não necessariamente alto faturamento.


Desafios enfrentados:
Ajuste de joins para evitar duplicação de valores,
Tratamento de dados inconsistentes e
Garantia de integridade nas agregações financeiras


Possíveis melhorias:

Criação de dashboards interativos (Power BI),
Análise de retenção de clientes,
Cálculo de métricas como LTV (Lifetime Value) e
Segmentação de clientes


Caso queira trocar ideias ou discutir o projeto:

LinkedIn: https://www.linkedin.com/in/patricia-damasceno-2492266b/

Considerações finais:
Este projeto demonstra a construção de um pipeline de dados completo, desde a ingestão até a geração de insights, simulando um cenário real de atuação como analista de dados.
