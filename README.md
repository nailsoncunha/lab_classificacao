# Previsão de resultados das partidas dos Campeonatos Europeus

## Descrição

Nesta tarefa construiremos modelos preditivos de classificação para a predição do resultado de partidas dos Campeonatos Europeus, da temporada 2012-2013 à temporada 2017-2018. Os dados a serem utilizados estão disponíveis no Kaggle, na aba Data, e seguem a seguinte descrição:

**Identificadores:**
- ID: Identificador único da linha
- League: Liga em que a partida foi disputada (Alemã, Inglesa, Espanhola ou Italiana)
- Date: Data da partida
- HomeTeam: Time mandante na partida
- AwayTeam: Time visitante na partida

**Estatísticas dos times:** cada uma dessas variáveis é uma lista, em que cada valor representa uma das 5 partidas anteriores do time.
- HS: Chutes do time mandante
- AS: Chutes do time visitante
- HST: Chutes a gol do time mandante
- AST: Chutes a gol do time visitante
- HF: Faltas do time mandante
- AF: Faltas do time visitante
- HC: Escanteios do time mandante
- AC: Escanteios do time visitante
- HY: Cartões amarelos do time mandante
- AY: Cartões amarelos do time visitante
- HR: Cartões vermelhos do time mandante
- AR: Cartões vermelhos do time visitante

**Estatísticas de Aposta:** cada linha abaixo descreve a probabilidade, de acordo com as apostas, de cada time vencer. Olhando para B365, B365H é a probabilidade para o time mandante vencer, B365D é a probabilidade de empate, e B365A é a probabilidade do time visitante vencer. Os demais descritores seguem o mesmo padrão.

- B365H
- B365D
- B365A
- BWH
- BWD
- BWA
- IWH
- IWD
- IWA
- LBH
- LBD
- LBA
- PSH
- PSD
- PSA
- WHH
- WHD
- WHA
- VCH
- VCD
- VCA

As variáveis abaixo também se relacionam com as apostas:

- BbMx>2.5: Probabilidade máxima de haver mais que 2.5 gols, pelo Betbrain
- BbAv>2.5: Probabilidade média de haver mais que 2.5 gols, pelo Betbrain
- BbMx<2.5: Probabilidade máxima de haver menos que 2.5 gols, pelo Betbrain
- BbAv<2.5: Probabilidade média de haver menos que 2.5 gols, pelo Betbrain

**Variável alvo**
- Result: Resultado da partida, 0 quando time visitante ganha, 1 quando empate, 2 quando time mandante ganha.

-----------

As atividades esperadas para essa etapa são descritas a seguir:

Realize uma análise exploratória nos dados, identificando e explorando:
Correlações entre as variáveis,
Distribuição das variáveis,
Valores ausentes,
Possíveis desbalanceamentos entre as classes.
Usando todas as variáveis disponíveis e tune, usando validação cruzada e outras medidas para controlar o overfitting caso necessário:
Um modelo de classificação com Regressão Logística,
Um modelo de classificação com Árvores de Decisão,
Um modelo KNN, e
Um modelo usando AdaBoost.
Use um modelo de Deep Learning
Identifique os valores de Precision, Recall, Acurácia e F1-Score para os modelos utilizados. Existe diferença entre o desempenho no treino e na validação? Justifique os resultados obtidos.
Re-treine o melhor modelo (usando os melhores valores de parâmetros encontrados em todos os dados, sem usar validação cruzada). Use esse último modelo treinado para prever os dados de teste disponíveis no challenge que criamos na plataforma Kaggle.

## Ideias para melhorar os resultados:

Use normalização das features.
Tente derivar novas features a partir das existentes.
Use outros métodos de classificação. Por exemplo, SVC, XGBoost e CatBoost.
Como devo entregar?

Link para o Colab. Além disso, pelo menos uma submissão deve ser feita no desafio que lançaremos no Kaggle.

Link para competição no Kaggle:

[Campeonatos Europeus](https://www.kaggle.com/c/ufcg-cdp-classificacao-20192)
