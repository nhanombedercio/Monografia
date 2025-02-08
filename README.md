# Monografia
 Aplicação de Aprendizagem de Máquina para avaliação do risco de mortalidade infantil por malária no Distrito da Manhiça, Moçambique

 
## Descrição do Projeto
Este projeto tem como objetivo desenvolver um modelo preditivo utilizando técnicas de **Aprendizado de Máquina** para avaliar o risco de **mortalidade infantil por malária** no Distrito da Manhiça, Moçambique. A análise será realizada exclusivamente com os **dados de internamento (INPD4)**, que contêm informações clínicas relevantes sobre crianças hospitalizadas devido à malária.

O projeto está inserido no contexto da dissertação de Mestrado em Estatística Aplicada e segue um plano estruturado para limpeza, exploração, modelagem e avaliação de diferentes algoritmos de **Machine Learning**.

---

## 1. Estrutura do Projeto
```
📂 Analise_Mortalidade_Malaria
│── 📁 data                  # Contém os datasets originais e processados
│── 📁 notebooks             # Jupyter Notebooks com análises exploratórias e modelagem
│── 📁 models                # Modelos treinados e avaliados
│── 📁 reports               # Relatórios e gráficos gerados
│── 📁 scripts               # Scripts Python para limpeza, análise e modelagem
│── 📜 README.md             # Documentação do projeto
│── 📜 requirements.txt      # Bibliotecas Python necessárias
```
 

## 2. Descrição dos Dados
O estudo utiliza exclusivamente a base de dados de **internamento (INPD4)**, que inclui variáveis como:

- **Características do paciente**: Idade, sexo, peso
- **Informações clínicas**: Temperatura, frequência cardíaca, frequência respiratória, nível de parasitemia
- **Tratamento hospitalar**: Tipo de tratamento administrado
- **Desfecho clínico (OUTCOME)**: Mortalidade ou sobrevivência da criança

A variável alvo da análise será a **mortalidade infantil por malária**, derivada da variável `OUTCOME`.

---

## 4. Etapas do Projeto

### 4.1. Aquisição e Pré-processamento dos Dados
✔️ Carregar a base de dados **INPD4**  
✔️ Tratar valores ausentes e inconsistências  
✔️ Normalizar variáveis numéricas e converter variáveis categóricas  

**Script:** `scripts/data_preprocessing.py`

---

### 4.2. Análise Exploratória
✔️ Estatísticas descritivas das variáveis  
✔️ Distribuição de variáveis clínicas  
✔️ Análise da relação entre variáveis e mortalidade  
✔️ Visualização dos dados (histogramas, boxplots, correlações)  

**Notebook:** `notebooks/exploratory_analysis.ipynb`

---

### 4.3. Seleção de Modelos de Machine Learning
Os seguintes algoritmos serão comparados:

1. **Random Forest**
2. **Redes Neurais Artificiais (ANN)**
3. **Máquinas de Vetores de Suporte (SVM)**

✔️ Definir features e variável alvo  
✔️ Dividir os dados em treino (80%) e teste (20%)  

**Notebook:** `notebooks/model_selection.ipynb`

---

### 4.4. Treinamento e Avaliação dos Modelos
✔️ Treinar cada modelo com validação cruzada  
✔️ Avaliar o desempenho usando métricas:
   - Acurácia
   - Sensibilidade e especificidade
   - Matriz de confusão
   - Área sob a curva ROC (AUC-ROC)

**Notebook:** `notebooks/model_evaluation.ipynb`

---

### 4.5. Comparação e Ajuste dos Modelos
✔️ Selecionar o modelo com melhor desempenho  
✔️ Ajustar hiperparâmetros para otimização  
✔️ Salvar modelo treinado para futuras previsões  

**Notebook:** `notebooks/final_model_tuning.ipynb`

---

## 5. Resultados Esperados
🔹 Identificar **fatores críticos** que influenciam a mortalidade infantil por malária  
🔹 Desenvolver um modelo de predição **robusto e preciso**  
🔹 Propor um sistema de **avaliação de risco** baseado em Machine Learning  

---

## 6. Ferramentas Utilizadas
- **Linguagem:** Python (Pandas, NumPy, Scikit-learn, TensorFlow)
- **Visualização:** Matplotlib, Seaborn
- **Ambiente:** Jupyter Notebook
- **Modelagem:** Random Forest, Redes Neurais, SVM
- **Versionamento:** GitHub

---

## 7. Contato
👤 **Autor:** Dércio Justino Nhanombe  
📧 Email: [dercio.nhanombe@hayusten.com]  
📌 Universidade: Faculdade de Ciências, Maputo, Moçambique  

---
 

🚀 **Este estudo pode servir de base para implementação de modelos preditivos em outras regiões endêmicas!**





