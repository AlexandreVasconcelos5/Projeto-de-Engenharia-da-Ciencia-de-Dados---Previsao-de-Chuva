## 🌧️ Projeto de Classificação de Engenharia da Ciência de Dados - Previsão de Chuva

Este projeto aplica um ciclo end-to-end de Engenharia da Ciência de Dados para prever se irá, ou não, chover no dia seguinte, com base em dados meteorológicos históricos da Austrália., durante um período de aproximadamente 8,5 anos.
O foco principal foi construir um pipeline de classificação robusto, desde o data profiling até à modelação, com especial atenção à sensibilidade, uma métrica crítica em cenários reais onde é fundamental minimizar falsos negativos (por exemplo: impacto na agricultura e na segurança pública).
________________________________________

## Destaques do Projeto
- Conjunto de dados real com 145.460 registos e 23 variáveis.
- Tratamento dos valores omissos através da imputação pela moda e tratamento dos valores atípicos pelo truncamento aos valores mínimo e máximo.
- Normalização de escala por Z-Score.
- Balanceamento: sobreamostragem por SMOTE.
- Engenharia de Variáveis: codificação temporal, geográfica, cíclica e binária.
- Avaliação de 6 modelos de classificação: Naïve Bayes, KNN, Árvores de Decisão, Random Forest, Gradient Boosting e Percetrão Multicamadas.
- Análise de overfitting para cada modelo.
________________________________________

## Resultados Principais
- KNN (k=23, distância Euclidiana) → melhor desempenho em sensibilidade (0.82), com boa AUC.
- Percetrão Multicamadas (taxa de aprendizagem adaptativa, taxa de aprendizagem = 0.05, 500 iterações) → sensibilidade de 0.76, sem sinais de overfitting.
- Árvore de Decisão (entropia, profundidade=4) → recall de 0.71, modelo interpretável e de fácil explicação.
- Variável mais relevante: Humidade_15h (forte correlação com Chuva_Amanha).
- Conclusão: os modelos de KNN e Percetrão Multicamadas mostraram-se ser os mais adequados para o problema, maximizando a deteção correta dos dias chuvosos, ainda que com uma taxa considerável de falsos positivos.
________________________________________

## Estrutura do Projeto
1.	Perfilamento dos Dados → análise exploratória, valores em falta, valores atípicos e correlações.
2.	Pré-processamento dos Dados → imputação de valores em falta e de valores atípicos, normalização de escala e balanceamento.
3.	Engenharia de Variáveis: codificação de variáveis.
4.	Modelação → treino e validação de múltiplos algoritmos de classificação.
5.	Avaliação → Métricas Exatidão, Sensibilidade, Precisão, AUC e F1 e estudo de overfitting.
6.	Análise Crítica → trade-offs entre recall e precisão, explicabilidade vs desempenho.
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
- Email: alex-0.5@hotmail.com
- LinkedIn: https://www.linkedin.com/in/alexandre-vasconcelos-396227167/
