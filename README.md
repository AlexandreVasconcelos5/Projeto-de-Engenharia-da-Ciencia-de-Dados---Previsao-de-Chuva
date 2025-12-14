## Projeto de Classificação de Engenharia da Ciência de Dados - Previsão de Chuva 🌧️

Este projeto aplica um ciclo end-to-end de Engenharia da Ciência de Dados para prever a ocorrência de chuva no dia seguinte (variável alvo: Chuva_Amanha), com base em dados meteorológicos históricos da Austrália, durante um período de aproximadamente 8,5 anos. O conjunto de dados em questão é real, tendo sido retirado do Kaggle.
O foco principal deste projeto foi construir um pipeline de classificação robusto, desde a fase do perfilamento de dados até à fase da modelação, com especial atenção dada à sensibilidade, uma métrica de avaliação crítica em cenários onde é fundamental minimizar os falsos negativos (por exemplo: impacto na agricultura e na segurança pública).
________________________________________

## Destaques do Projeto
- Projeto avaliado com 18 valores, demonstrando rigor e qualidade na implementação de um pipeline end-to-end da Engenharia de Ciência de Dados.
- Conjunto de dados real com 145.460 registos e 23 variáveis.
- Tratamento dos valores omissos através da imputação pela moda e tratamento dos valores atípicos pelo truncamento aos valores mínimo e máximo.
- Normalização de escala por Z-Score.
- Balanceamento: sobreamostragem por SMOTE.
- Engenharia de Variáveis: codificação temporal, geográfica, cíclica e binária.
- Avaliação de 6 modelos de classificação: Naïve Bayes, KNN, Árvores de Decisão, Random Forest, Gradient Boosting e Percetrão Multicamadas.
- Análise de overfitting para cada modelo.
________________________________________

## Resultados Principais
- Modelo de KNN (hiperparâmetros: k=23 e distância Euclidiana): melhor desempenho em sensibilidade, de 0.82, com alta exatidão e AUC.
- Modelo de Percetrão Multicamadas (hiperparâmetros: taxa de aprendizagem escala inversa, taxa de aprendizagem = 0.05 e 500 iterações): sensibilidade de 0.76, com alta exatidão e AUC, sem sinais de overfitting.
- Variável mais relevante: Humidade_15h (forte correlação com a variável Chuva_Amanha).
- Conclusão: os modelos de KNN e Percetrão Multicamadas revelaram-se os mais adequados para o problema em questão, maximizando a deteção correta dos dias chuvosos, ainda que com uma taxa considerável de falsos positivos.
________________________________________

## Estrutura do Projeto
1.	Perfilamento dos Dados: análise exploratória, valores em falta, valores atípicos e correlações.
2.	Pré-processamento dos Dados: imputação de valores em falta e de valores atípicos, normalização de escala e balanceamento.
3.	Engenharia de Variáveis: codificação de variáveis.
4.	Modelação: treino e validação de 6 modelos de classificação.
5.	Avaliação: métricas de avaliação (Exatidão, Sensibilidade, Precisão, AUC e F1), matriz de confusão e estudo de overfitting.
6.	Análise Crítica.
________________________________________

## Ferramentas Utilizadas
- Jupyter Notebook
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
________________________________________

## Conteúdos do Repositório
- Jupyter Notebook - Projeto - Engenharia da Ciência de Dados - Conjunto de Dados Chuva - Alexandre Vasconcelos.ipynb - Código do projeto
- Relatório PDF - Projeto - Engenharia da Ciência de Dados - Conjunto de Dados Chuva - Alexandre Vasconcelos.pdf - Relatório do projeto, detalhado com a descrição e os resultados da análise
________________________________________

## Como Visualizar os Resultados
1. Clonar o repositório
2. Abrir no Jupyter Notebook o ficheiro `.ipynb`
3. Executar as células por ordem para reproduzir a análise
________________________________________

## Contactos
- Nome: Alexandre Vasconcelos
- Email: alex.vasconcelos.2057@gmail.com
- LinkedIn: https://www.linkedin.com/in/alexandre-vasconcelos-396227167/
