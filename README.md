# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Bem-vindo ao desafio de projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas. Neste Lab DIO, aprendi a usar o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML). Vou falar um pouco como pude completar o desafio!

## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)

O objetivo desse desafio foi de fato colocar em prática o que aprendemos sobre plataformas no-code no Bootcamp Nexa - Machine Learning para iniciantes na AWS na plataforma [DIO](https://dio.me), nesse caso o SageMaker Canvas da AWS.


## 🚀 Passo a Passo

### 1. Selecionar Dataset

-   Tive dificuldade de acessar a plataforma da AWS, para realização do desafio, porém, consegui fazer a demonstração gratuita da plataforma. Após isso, tive a oportunidade de acessar um Lab no Skill Builder na AWS para realização na plataforma, porém, por que stão de convergencia de contas, tive novamente problemas em acessar, mesmo após muitas tentativas. Ainda assim, fiquei feliz, pois mesmo utilizando uma modelo menos completo, pude entender como a plataforma funciona.
-   A escolha do dataset usado para treinar meu modelo de previsão de estoque foi o [on-time-delivery-data].
-   Não precisei fazer o upçoad, pois a plataforma já disponibilizou esse recurso no próprio SageMaker Canvas.

### 2. Construir/Treinar

-   No SageMaker Canvas, foi importado o dataset.
-   Selecionei quais seriam as propriedades a serem consideradas para o treinamento do modelo.
-   Iniciei o treinamento do modelo.

### 3. Analisar

-   Após o treinamento, examinei as métricas de performance do modelo e percebi que não havia chegado nem a 80% de acuracia, por tanto retornei ao passo anterior de selecionar mais propriedades que influenciariam no treinamento do modelo, para melhorar a precisão dos resultados.
-   Verifiquei as principais características que influenciam as previsões, que no meu caso foram a 'umidade' e 'total de itens no caminhão', esse último, sendo o conjunto de dados com maior importancia para os resultados mais apurados.
-   Após ajustes no modelo e re-treino, obtive um desempenho satisfatório, com 95,67% de precisão do meu modelo.

### 4. Prever

-   Meu modelo foi treinado e re-treinado para previsão de estoque, buscando prever a porcentagem de 'Atrasos' e de entregas 'Na Hora', observando quais propriedades eram mais relevantes para essa analise.
-   Exportei os resultados e analisei as previsões geradas.
-   Após análise pude perceber que em dias com umidade relativa e com menor quantidade de itens no caminhão a porcentagem de entregas na hora eram maiores, do que num cenário oposto. E que mesmo em dias com clima favorável a porcentagem de entregas com atraso aumentaria se houvesse uma grande quantidade de itens para entrega no caminhão, o que tornou a propriedade 'total de itens no caminhão' a mais crucial para tomada de decisão nesse processo. 

💜 por [Gabriela Silva](https://github.com/SabrinaAll)
