# 📊 Projeto AVP II – Machine Learning  
### Tema: **Regressão Linear – Predição de Preço de Imóveis**

## 👥 Integrantes

- Pedro Humberto Gama de Medeiros – 01741824  
- Jonas Felipe Dantas Segundo Guimarães – 01720927  
- Vinicius de Freitas e Silva – 01707712  

---

## ▶️ **Executar no Google Colab**

Para facilitar a correção e demonstração, os notebooks estão disponíveis online:

| Modelo | Link do Colab |
|:--------|:---------------|
| 📘 Regressão Linear | [Abrir no Google Colab](https://colab.research.google.com/drive/1G2TSlATu9pbaPj3XmcqMKwwCM2ol4OH9?usp=sharing) |


> 💡 *Basta clicar no link e executar as células diretamente no navegador.*

---
## 🎯 **Objetivo**
Desenvolver um modelo de *Machine Learning* capaz de prever o preço médio de imóveis com base em variáveis numéricas, utilizando **Regressão Linear** como modelo paramétrico e **KNN Regressor** como modelo não paramétrico.  
O projeto segue as diretrizes da disciplina *Machine Learning (AVP II)*, com comparação entre modelos, visualizações gráficas e relatório técnico.

---

## 🧠 **Conceitos Teóricos**

### 🔹 Regressão Linear (Modelo Paramétrico)
A Regressão Linear busca ajustar uma relação **linear** entre variáveis independentes (X) e uma variável dependente (Y), assumindo a forma:

\[
Y = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + ... + \beta_n X_n
\]

É um modelo **paramétrico**, pois depende de parâmetros fixos (coeficientes β).  
✅ *Vantagens:* Simples, rápido e interpretável.  
⚠️ *Limitações:* Não capta relações não lineares entre as variáveis.

---

### 🔹 KNN Regressor (Modelo Não Paramétrico)
O **K-Nearest Neighbors Regressor** prevê o valor de uma amostra pela média dos **K vizinhos mais próximos**.  
Não assume nenhuma forma de função pré-definida — o modelo se ajusta conforme os dados.

✅ *Vantagens:* Capta padrões complexos e não lineares.  
⚠️ *Limitações:* Mais lento com grandes bases e sensível à escala das variáveis.

---

## 🏠 **Base de Dados**

- **Dataset:** [California Housing (Scikit-learn)](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset)
- **Registros:** 20.640 amostras  
- **Variável Alvo:** `MedHouseVal` (preço médio das casas)  
- **Principais Features:**
  - `MedInc` → Renda média da região  
  - `HouseAge` → Idade média das casas  
  - `AveRooms` → Número médio de cômodos  
  - `AveOccup` → Média de ocupantes  
  - `Latitude`, `Longitude`  

---

## ⚙️ **Metodologia**

1. **Carregamento do Dataset** via Scikit-learn  
2. **Análise Exploratória (EDA)** – Estatísticas, correlação e gráficos  
3. **Pré-processamento:**
   - Normalização dos dados (`StandardScaler`)
   - Divisão em treino e teste (80% / 20%)
4. **Treinamento dos Modelos:**
   - Regressão Linear (`LinearRegression`)
   - KNN Regressor (`KNeighborsRegressor`)
5. **Avaliação das Métricas:**
   - `MSE` (Erro Quadrático Médio)  
   - `MAE` (Erro Absoluto Médio)  
   - `R²` (Coeficiente de Determinação)
6. **Visualizações Gráficas:**
   - Dispersão com reta de regressão  
   - Gráfico Real vs Previsto  
   - Comparação de R² entre os modelos

---

## 📈 **Resultados Esperados**

| Modelo | MSE | MAE | R² |
|:-------|:----|:----|:----|
| Regressão Linear | ≈ 0.52 | ≈ 0.48 | ≈ 0.61 |
| KNN Regressor | ≈ 0.45 | ≈ 0.43 | ≈ 0.68 |

*(Os valores podem variar ligeiramente conforme a execução do código.)*

📊 O modelo **KNN** apresentou desempenho superior em R², mostrando maior capacidade de captar relações não lineares.  
Já a **Regressão Linear** se destacou pela simplicidade e rapidez na execução.

---

## 💬 **Conclusões**

- A Regressão Linear é eficiente e interpretável, ideal para problemas com relação aproximadamente linear.  
- O KNN, sendo não paramétrico, adapta-se melhor a relações complexas, mas exige mais processamento.  
- A escolha do modelo ideal depende do **equilíbrio entre precisão, simplicidade e custo computacional.**

---

## 🧩 Divisão de Funções (Grupo)

| Função                       | Integrante                                  | Responsabilidade principal                                      |
|-----------------------------|---------------------------------------------|------------------------------------------------------------------|
| Líder / Programador 1       | Vinicius de Freitas e Silva – 01707712      | Organização geral do projeto, GitHub e código da Regressão Linear |
| Redator / Apresentador      | Pedro Humberto Gama de Medeiros – 01741824  | Revisão teórica, escrita do relatório e preparação dos slides   |
| Programador 2 / Auxiliar    | Jonas Felipe Dantas Segundo Guimarães – 01720927 | Implementação do KNN, testes e apoio na apresentação         |

---

## 🧰 **Ferramentas Utilizadas**

- 🐍 **Python 3.10+**
- 📓 **Google Colab**
- ⚙️ **Bibliotecas:**  
  `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- 💻 **Controle de Versão:** Git + GitHub
- 📄 **Relatório:** Overleaf (LaTeX)
- 🖼️ **Apresentação:** Google Slides / Canva

---

## 🚀 **Como Executar o Projeto**

1. Clone o repositório:

   git clone https://github.com/vinicius024/Machine-Learning-AV-II-.git

2. Abra o arquivo no Google Colab:

    regressao_linear.ipynb

    knn_regressor.ipynb

3. Execute todas as células.

4. Verifique as métricas finais e gere os gráficos.

📚 Referências

Pedregosa et al. Scikit-learn: Machine Learning in Python. Journal of Machine Learning Research, 2011.

Géron, Aurélien. Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow. O’Reilly, 2023.

Documentação oficial: https://scikit-learn.org/stable/
