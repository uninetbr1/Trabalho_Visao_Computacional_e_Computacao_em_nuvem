# Trabalho de Visão Computacional e Computação em Nuvem

# Análise Preditiva de Métricas Ofensivas e Defensivas da Premier League utilizando Machine Learning

## Autor

Eddio Pellegrini Netto

---

# 1. Descrição do Projeto

Este projeto tem como objetivo aplicar técnicas de Machine Learning supervisionado para análise preditiva de estatísticas de jogadores da Premier League 2024/2025.
O trabalho utiliza dados reais disponibilizados na plataforma Kaggle contendo métricas ofensivas, defensivas e estatísticas gerais de desempenho dos atletas.
A proposta do projeto consiste em desenvolver e comparar modelos preditivos capazes de estimar diferentes indicadores de desempenho dos jogadores, permitindo analisar padrões ofensivos e defensivos dentro do futebol profissional.
O modelo principal utilizado será o Random Forest Regressor, implementado com a biblioteca Scikit-Learn.

---

# 2. Objetivos

## Objetivo Geral
Aplicar técnicas de Machine Learning para prever estatísticas ofensivas e defensivas de jogadores da Premier League utilizando dados esportivos reais.

---

## Objetivos Específicos

* Realizar o pré-processamento do dataset.
* Tratar valores ausentes e inconsistências.
* Realizar análise exploratória dos dados.
* Treinar modelos de regressão supervisionada.
* Comparar métricas ofensivas e defensivas.
* Avaliar o desempenho dos modelos utilizando RMSE.
* Interpretar os resultados obtidos.

---

# 3. Dataset Utilizado

Colunas do conjunto de dados

Jogador: Nome do jogador
Time: Time ao qual o jogador pertence
'#': Número da camisa do jogador
Nacionalidade: Nacionalidade do jogador
Posição: Posição principal em campo
Idade: Idade do jogador
Minutos: Total de minutos jogados
Gols: Número de gols marcados
Assistências: Número de assistências
Pênaltis a Gol: Pênaltis cobrados a gol Pênaltis: Total de pênaltis cobrados Total de Chutes
: Total de chutes a gol
Chutes no Alvo: Chutes a gol Cartões Amarelos: Número de cartões amarelos recebidos Cartões Vermelhos: Número de cartões vermelhos recebidos
Toques na Bola : Total de toques na bola Dribles: Total de dribles tentados Desarmes: Total de desarmes realizados Bloqueios: 
Total de bloqueios Gols Esperados (xG): Gols esperados, calculados com base nas posições de chute e na probabilidade de marcar 
Gols Esperados sem Pênaltis (xG sem Pênaltis): Gols esperados, excluindo pênaltis Assistências Esperadas (xAG): Assistências esperadas, com base nas ações que levaram a um gol esperado (xG) Ações de Criação de Chute: 
Ações que levaram a uma tentativa de chute Ações de Criação de Gol: Ações que levaram a uma finalização Passes Completos: Passes bem-sucedidos concluídos em direção ao gol Passes Tentados: Total de passes tentados % de Passes Completos: 
Taxa de passes completos, expressa em porcentagem (algumas entradas têm valores ausentes aqui) Passes Progressivos: Passes que avançam a bola significativamente em direção ao gol adversário Conduções: 
Total de conduções de bola Conduções Progressivas: Conduções que avançam a bola significativamente em direção ao gol adversário Tentativas de Drible: Total de dribles tentados Dribles Bem-Sucedidos: 
Total de dribles bem-sucedidos Data: Data da coleta de dados ou data da partida.

Cada linha representa um jogador e suas respectivas estatísticas.

---

# 4. Tecnologias Utilizadas

## Linguagem
* Python 3

## Bibliotecas
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Imbalanced-Learn

## Ferramentas
* Jupyter Notebook
* Git
* GitHub
* WSL Ubuntu

---

# 5. Metodologia

## 5.1 Pré-processamento dos Dados
Nesta etapa serão realizadas:

* Conversão de tipos de dados
* Limpeza do dataset
* Conversão de colunas percentuais
* Tratamento de valores ausentes
* Ajuste de colunas numéricas

---

## 5.2 Análise Exploratória dos Dados
Será realizada uma análise estatística e visual dos dados utilizando:

* Estatística descritiva
* Histogramas
* Boxplots
* Correlação entre variáveis
* Análise de distribuição
* Verificação de possíveis outliers

---

## 5.3 Modelos Preditivos
O projeto utilizará o algoritmo Random Forest Regressor para prever métricas ofensivas e defensivas dos jogadores.

6. Comparação entre Modelos
Serão desenvolvidos três modelos preditivos distintos.

Modelo 1 — Goal Contribution (Utilizando um notebook pronto como base)
Objetivo:
Prever a contribuição ofensiva geral do jogador.

Features utilizadas
Minutes
Goals
Assists
Touches
Passes Completed
Pass Completion %
Target
Goal Contribution

Modelo 2 — Shots on Target
Objetivo:
Analisar a capacidade ofensiva e agressividade de finalização dos jogadores.

Features utilizadas
Minutes
Goals
Assists
Touches
Passes Completed
Pass Completion %
Target
Shots on Target

Modelo 3 — Interceptions
Objetivo:
Analisar padrões defensivos e capacidade de recuperação de posse de bola.

Features utilizadas
Minutes
Touches
Passes Completed
Pass Completion %
Blocks
Tackles
Target
Interceptions

7. Algoritmo Utilizado

O algoritmo principal utilizado será o Random Forest Regressor.
O Random Forest é um algoritmo de aprendizado supervisionado baseado em múltiplas árvores de decisão.
O modelo funciona combinando diversas árvores para gerar previsões mais robustas e reduzir problemas de overfitting.
A escolha do algoritmo ocorre devido à sua boa capacidade de generalização e robustez em datasets tabulares contendo múltiplas variáveis numéricas.

8. Avaliação dos Modelos

Os modelos serão avaliados utilizando a métrica RMSE (Root Mean Squared Error).
O RMSE mede o erro médio entre os valores previstos e os valores reais.
Quanto menor o valor do RMSE, melhor o desempenho do modelo.

9. Resultados Esperados

Espera-se que os modelos consigam:

Identificar padrões ofensivos em jogadores.
Identificar padrões defensivos.
Comparar métricas ofensivas e defensivas.
Demonstrar a aplicação prática de Machine Learning em análise esportiva.
Obter modelos com baixo erro preditivo.
Além disso, o projeto busca investigar quais métricas apresentam maior previsibilidade utilizando aprendizado supervisionado.

10. Estrutura do Repositório
trabalho-1/
│
├── dataset.csv
├── data_preparation_EPL.ipynb
├── README.md

12. Referências
Kaggle – Premier League Player Stats 24/25 (PALMIERI, E.)- https://www.kaggle.com/datasets/eduardopalmieri/premier-league-player-stats-season-2425/data
Premier League 2425 Player Stats Secrets (RISK, B.) - https://www.kaggle.com/code/devraai/premier-league-2425-player-stats-secrets

14. Considerações Finais
Este trabalho busca integrar conceitos de Machine Learning, análise estatística e ciência de dados aplicados ao contexto esportivo.
A comparação entre métricas ofensivas e defensivas permitirá avaliar o comportamento preditivo de diferentes atributos do futebol profissional.
Além disso, o projeto busca demonstrar aplicações práticas de inteligência artificial em análise esportiva utilizando dados reais da Premier League.
