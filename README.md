# Modelo de Previsão de Custos de Seguro

## MBA em Inteligência Artificial para Devs- FIAP
### PÓS TECH FIAP 3IADT – GRUPO 11 - 2024

**Integrantes:**
- Adalberto Silva (RM 358647)
- Eduardo Tamaki (RM 359402)
- Carmem Arita (RM 357808)
- Marcio Godoi (RM 359476)

**Video Explicação:**
- https://www.youtube.com/watch?v=Js9t57HwBPc

## Visão Geral do Projeto
Este projeto é parte do Tech Challenge do MBA em Inteligência Artificial da FIAP. O objetivo é analisar custos de seguro saúde e desenvolver modelos de machine learning para prever despesas de seguro com base em diversos atributos dos clientes. A análise utiliza diferentes modelos de regressão para determinar a abordagem mais eficaz para previsão de custos.

## Dataset
O conjunto de dados (`insurance.csv`) contém informações sobre beneficiários de seguro, incluindo:
- Idade
- Sexo
- IMC (Índice de Massa Corporal)
- Número de filhos
- Status de fumante
- Região geográfica
- Custos do seguro

## Stack Técnica
- **Bibliotecas Python**:
  - pandas: Manipulação e análise de dados
  - numpy: Computações numéricas
  - matplotlib/seaborn: Visualização de dados
  - scikit-learn: Implementações de machine learning

## Modelos Implementados
1. **Regressão Linear**
   - Inclui ajuste de hiperparâmetros usando GridSearchCV
   - Padronização de features usando StandardScaler

2. **Árvore de Decisão**
   - Implementada com max_depth=5 para prevenir overfitting

3. **Random Forest**
   - Método ensemble utilizando 100 estimadores

## Etapas da Análise
1. Carregamento e Exploração Inicial dos Dados
2. Engenharia de Features
   - Codificação de variáveis categóricas usando LabelEncoder
3. Análise Exploratória de Dados (EDA)
   - Análise de distribuição
   - Análise de correlação usando mapas de calor
4. Pré-processamento dos Dados
   - Divisão treino-teste
   - Escalonamento de features
5. Treinamento e Avaliação dos Modelos
   - Múltiplos modelos treinados e comparados
   - Métricas de performance calculadas:
     - R² Score
     - Erro Médio Absoluto (MAE)
     - Erro Quadrático Médio (MSE)
     - Raiz do Erro Quadrático Médio (RMSE)
     - Erro Percentual Médio Absoluto (MAPE)

## Visualizações
- Histogramas para distribuição de features
- Gráficos de dispersão para análise de relacionamentos
- Mapa de calor de correlação
- Gráficos de Previsão vs Valor Real para avaliação dos modelos

## Utilização
A análise é apresentada em formato Jupyter notebook (`tech_challenge_notebook.ipynb`), permitindo execução interativa e visualização dos resultados.

## Melhorias Futuras
- Análise de importância das features
- Validação cruzada para avaliação mais robusta dos modelos
- Ajuste de hiperparâmetros para modelos baseados em árvore
- Implementação de outros algoritmos (XGBoost, LightGBM)
- Pipeline de deploy do modelo

## Como Executar
1. Clone o repositório
2. Instale as dependências necessárias
3. Execute o Jupyter Notebook
4. Siga as células do notebook em ordem sequencial

## Requisitos
- Python 3.x
- Jupyter Notebook
- Bibliotecas listadas na Stack Técnica

## Licença
Este projeto é parte do programa educacional da FIAP e deve ser utilizado apenas para fins acadêmicos.

---
Desenvolvido como parte do Tech Challenge do MBA em Inteligência Artificial da FIAP - 2024.
