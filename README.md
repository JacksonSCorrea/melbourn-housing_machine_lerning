# melbourne-housing_machine_lerning

Este é um projeto de Ciência de Dados que tem o intuito de elaborar modelos de regressão linear para prever preços de casas em Melbourne, Austrália.

Trata-se de um projetos para estudo e composição de portfólio.

Foi realizada uma análise exploratória dos dados, com o intuito de descrever algumas relações e demonstrar alguns insights que podem ser estratégicos na tomada de decisões.

Adiante, os dados foram pré-processados, ocorrendo a remoção de valores missing e outliers. Também foi realizada a conversão de variáveis categóricas emnuméricas.

Feito isso, os dados foram separados em dados de treino e de teste. Os dados de teste representam 20% dos dados totais, e são utilizados somente na verificação do desempenho do modelo final treinado.

Na sequência, foram criados três modelos baseline, treinados com os dados de treino (80% dos dados totais): Regressão Linear, Árvore de Decisão e Floresta Aleatória. Nenhum hiperparâmetro foi modificado, adotando-se assim os valores default. A partir da análise das métricas de cada modelo foi selecionado o algoritmo de Floresta Aleatória como sendo o mais promissor para a sequência do projeto.

Foi realizada a validação cruzada neste modelo, treinados com os dados de treino (80% dos dados totais), e utilizando-se 5 folds.
Os valores dos resultados de desempenho são exibidos através de um quadro resumo.

Como tentativa de melhoria dos resultados, foi realizada a normalização e padronização dos dados, aos quais não apresentaram muita eficácia em relação ao modelo treinado.

Por fim, a partir do modelo de Floresta Aleatória já treinado (baseline) foram feitas novas predições com dados nunca antes vistos (X_teste, que representa 20% dos dados do dataset original)

Observa-se que o modelo de Floresta Aleatória, por se tratar de um modelo ensemble e mais complexo, obteve melhores resultados, visto que as correlações entre as variáveis e o target possuem distribuição complexa e não linear.

Enjoy!
