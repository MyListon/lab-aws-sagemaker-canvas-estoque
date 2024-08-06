# Projeto de Previsão de Estoque com Amazon SageMaker Canvas

## Descrição do Projeto

Este projeto tem como objetivo prever a quantidade de estoque de produtos em uma loja utilizando o Amazon SageMaker Canvas. Utilizamos um dataset contendo informações diárias sobre o estoque de diversos produtos, bem como a presença ou não de promoções. Com base nesses dados, construímos um modelo preditivo capaz de auxiliar na gestão de estoque, otimização de vendas e planejamento de promoções.

## Dataset

O dataset utilizado no projeto contém as seguintes colunas:

- **ID_PRODUTO**: Identificação única de cada produto.
- **DIA**: Data da observação no formato `YYYY-MM-DD`.
- **FLAG_PROMOCAO**: Indicador binário (0 ou 1) que mostra se o produto estava em promoção no dia.
- **QUANTIDADE_ESTOQUE**: Quantidade de unidades do produto em estoque no dia.

## Objetivo

O objetivo principal deste projeto é prever a `QUANTIDADE_ESTOQUE` dos produtos para os dias seguintes, levando em consideração o histórico de dados e a presença de promoções.

## Passos para Utilização do Amazon SageMaker Canvas

1. **Preparação do Dataset:**
   - Certifique-se de que o dataset está no formato CSV com as colunas mencionadas acima.

2. **Acesso ao SageMaker Canvas:**
   - Entre na sua conta AWS e navegue até o serviço Amazon SageMaker.
   - Acesse o SageMaker Canvas e crie um novo projeto.

3. **Importação do Dataset:**
   - No projeto criado, importe o arquivo CSV contendo os dados de estoque.

4. **Construção do Modelo de Previsão:**
   - No SageMaker Canvas, selecione a opção para construir um novo modelo.
   - Escolha o dataset importado e defina `QUANTIDADE_ESTOQUE` como a variável alvo.
   - Configure o modelo para considerar `DIA` como variável de tempo e `FLAG_PROMOCAO` como fator relevante.
   - Inicie o treinamento do modelo.

5. **Avaliação e Uso do Modelo:**
   - Após o treinamento, avalie o desempenho do modelo com as métricas fornecidas pelo SageMaker Canvas.
   - Utilize o modelo para fazer previsões em novos dados ou dados históricos não incluídos no treinamento.
   - Exporte as previsões geradas para um arquivo CSV para análise posterior.

## Tecnologias Utilizadas

- **Amazon SageMaker Canvas:** Ferramenta utilizada para construção e treinamento do modelo preditivo.
- **Python (opcional):** Pode ser utilizado para manipulação e limpeza de dados antes de importar para o SageMaker Canvas.

## Resultados Esperados

Com o modelo preditivo treinado, espera-se obter previsões precisas da quantidade de estoque de produtos, permitindo uma melhor gestão de inventário, otimização de vendas e planejamento de promoções.

## Conclusão

Este projeto demonstra como o Amazon SageMaker Canvas pode ser utilizado para construir modelos preditivos eficazes para a gestão de estoque. Através da análise dos dados históricos e da presença de promoções, o modelo proporciona insights valiosos para decisões de negócios mais informadas.
