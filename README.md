# Challenge Alura - Data Science
![image](https://github.com/user-attachments/assets/59a9b23d-4522-439e-be93-5896c641087a)

# Descrição do Projeto
O projeto visa a ajudar o Senhor João a decidir qual loja da sua rede Alura Store vender para iniciar um novo empreendimento, por meio de análise de dados de vendas, desempenho e avaliações das 4 lojas fictícias da Alura Store. O objetivo é identificar a loja com menor eficiência e apresentar uma recomendação final baseada nos dados.

# 📝 Etapas
- `Etapa 1`
  Calcular o faturamento total de cada loja. Somando os valores da coluna "Preço" de cada loja para estimar o faturamento.

  **Método utilizado:**

  *.sum() para o somatório da coluna "Preço"*

![image](https://github.com/user-attachments/assets/a12ed6bb-2c33-459e-a7dd-f664ed01ba4f)


- `Etapa 2`
  Calcular a quantidade de produtos vendidos por categoria em cada loja.

  **Foram utilizados os métodos:**
  
  *.groupby() para agrupamento dos dados*;
  
  *.count() para contagem de elementos* e
  
  .*sort_values() com o parâmetro ascending=False para ordenação de forma decrescente*
