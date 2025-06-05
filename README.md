# Challenge Alura - Data Science
![image](https://github.com/user-attachments/assets/59a9b23d-4522-439e-be93-5896c641087a)

# Descrição do Projeto
O projeto visa a ajudar o Senhor João a decidir qual loja da sua rede Alura Store vender para iniciar um novo empreendimento, por meio de análise de dados de vendas, desempenho e avaliações das 4 lojas fictícias da Alura Store. O objetivo é identificar a loja com menor eficiência e apresentar uma recomendação final baseada nos dados.

# 📝 Etapas
- `Etapa 1`
  Calcular o faturamento total de cada loja. Somando os valores da coluna "Preço" de cada loja para estimar o faturamento.

  **Métodos utilizados:**

  * `.sum()` para o somatório da coluna "Preço"

  ![image](https://github.com/user-attachments/assets/76219fa8-ecdf-4cec-9060-0ae695c469dc)



- `Etapa 2`
  Calcular a quantidade de produtos vendidos por categoria em cada loja.
  

  **Métodos utilizados:**
  
  
  * `.groupby()` para agrupamento dos dados
  
  * `.count()` para contagem de elementos
  
  * `.sort_values()` com o parâmetro ascending=False para ordenação de forma decrescente

  * `.rename()` para renomear a coluna de contagem para 'Quantidade'
    
  * `.reset_index()` para transformar o agrupamento em um DataFrame limpo

  ![image](https://github.com/user-attachments/assets/c4fba84c-bf05-433d-8bdd-c22aca99cae2)


- `Etapa 3`
  Determinar a média de avaliação dos clientes para cada loja. Esta métrica reflete a satisfação geral com as compras.
  

  **Métodos utilizados**
  
  
  * `.mean()` para calcular a média dos valores na coluna "Avaliação da compra"
  
  * `.round(2)` para arredondar o resultado para duas casas decimais

  ![image](https://github.com/user-attachments/assets/7472bc2e-2680-4bbd-8ff1-f2e6f39b2d00)

  

- `Etapa 4`
  Identificar os produtos mais e menos vendidos em cada loja. Esta análise é crucial para entender o giro de estoque e a popularidade de itens específicos.
  

  **Métodos utilizados:**
  
  
  * `.groupby()` para agrupar os dados pela coluna "Produto"
  
  * `.count()` para contar as ocorrências de cada produto
    
  * `.sort_values()` com `ascending=False` para os mais vendidos e `ascending=True` para os menos vendidos
    
  * `.rename()` para nomear a coluna resultante como 'Quantidade'
    
  * `.head()` para exibir os primeiros (mais ou menos vendidos) resultados

  ![image](https://github.com/user-attachments/assets/a663cb56-90db-4ba7-8b65-d9983ee79d30)
  ![image](https://github.com/user-attachments/assets/b7e757f8-2b08-46ea-87d1-72811096c975)



- `Etapa 5`
  Calcular o custo médio do frete para cada loja. O frete é um fator que pode impactar a competitividade e a experiência do cliente.
  

  **Métodos utilizados:**
  
  
  * `.mean()` para calcular a média dos valores na coluna "Frete"
    
  * `.round(2)` para arredondar o resultado para duas casas decimais
 
  ![image](https://github.com/user-attachments/assets/5f3d9819-e884-4a91-bf18-7f980cd20909)


- `Etapa 6`
  Gerar visualizações gráficas para facilitar a compreensão dos dados e a comparação entre as lojas.
  

  **Métodos utilizados:**
  
  
  * `matplotlib.pyplot` para criação dos gráficos
    
  * `pandas.DataFrame()` para estruturar os dados para plotagem
    
  * `.plot(kind='bar')` para o comparativo de faturamento entre as lojas
    
  * `.plot(kind='barh')` para a visualização da quantidade de produtos por categoria em cada loja, permitindo fácil comparação das categorias mais vendidas
    
  * `.plot(kind='bar')` para comparar a média de avaliação dos clientes entre as lojas
    
  * `.plot(kind='scatter')` para visualizar o custo médio do frete, destacando a relação entre as lojas e o custo.
    

# 📈 Análise e Conclusão

Após a realização das etapas de análise e a geração dos gráficos, o projeto culmina em um relatório detalhado que sintetiza as descobertas. Esse relatório compara as lojas em termos de faturamento, vendas por categoria, avaliações, produtos mais/menos vendidos e frete, culminando em uma recomendação clara sobre qual loja o Senhor João deve considerar vender, com base nos dados e suas respectivas justificativas.






