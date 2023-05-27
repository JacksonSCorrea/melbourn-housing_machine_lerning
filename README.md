# melbourne-housing_machine_lerning

Este é um projeto de Ciência de Dados que tem o intuito de elaborar modelos de regressão linear para prever preços de casas em Melbourne, Austrália.

Trata-se de um projeto para estudo e composição de portfólio.

Inicialmente, foi realizada uma análise exploratória dos dados, com o intuito de descrever algumas relações e demonstrar alguns insights que podem ser estratégicos na tomada de decisões.

A seguir, os dados foram pré-processados, ocorrendo a análise de valores missing e análise de outliers. Também foi realizada a conversão de variáveis categóricas em numéricas. Não foram imputados valores aos dados faltantes para que se evite o problema de data leakage (por exemplo, os valores faltantes não foram substituídos pela média de valores, que é calculada com todo conjunto de treino e teste)

Feito isso, os dados foram separados em dados de treino e de teste, antes de qualquer manipulação através dos algortitmos de Machine Learning. Os dados de teste obtidos representam 20% dos dados totais, e são utilizados somente na verificação do desempenho do modelo final já treinado.

Na sequência, foram criados três modelos baseline, treinados com os dados de treino (80% dos dados totais): Regressão Linear, Árvore de Decisão e Floresta Aleatória. Nenhum hiperparâmetro foi modificado, adotando-se assim os valores default. A partir da análise das métricas de cada modelo foi selecionado o algoritmo de Floresta Aleatória como sendo o mais promissor para a sequência do projeto.

No modelo selecionado (Floresta Aleatória) foi realizada a validação cruzada com o objetivo de se obter métricas um pouco mais realistas, utilizando-se os dados de treino (80% dos dados totais), divididos em 5 folds. Os valores dos resultados de desempenho são exibidos através de um quadro resumo.

Como tentativa de melhoria dos resultados, foi realizada a normalização e padronização dos dados, aos quais não apresentaram muita eficácia em relação ao modelo treinado.

Por fim, a partir do modelo de Floresta Aleatória já treinado (baseline) foram feitas novas predições com dados nunca antes vistos (X_teste, que representa 20% dos dados do dataset original)

Observa-se que o modelo de Floresta Aleatória, por se tratar de um modelo ensemble e mais complexo, obteve melhores resultados, visto que as correlações entre as variáveis são complexas e em sua grande maioria a distribuição é complexa e não linear

Enjoy!
