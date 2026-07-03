# 🍄 Classificação de Cogumelos com Machine Learning

Projeto desenvolvido como parte do MVP da disciplina de Machine Learning & Analytics, com o objetivo de construir, comparar e avaliar modelos de aprendizado supervisionado capazes de classificar cogumelos como **comestíveis** ou **venenosos** a partir de características morfológicas.

---

## 📌 Objetivo

Desenvolver um pipeline completo de Machine Learning para classificação binária utilizando o dataset **Mushroom** da UCI Machine Learning Repository, comparando diferentes algoritmos e avaliando seu desempenho com foco na redução de falsos negativos (cogumelos venenosos classificados como comestíveis).

---

## 📊 Dataset

O projeto utiliza o **Mushroom Dataset (UCI)**, contendo:

- **8.124 amostras**
- **22 atributos categóricos**
- Classe alvo:
  - `e` → Comestível
  - `p` → Venenoso

O notebook tenta carregar automaticamente os dados pela URL oficial da UCI e, caso ela esteja indisponível, permite o upload manual do arquivo `.data`, garantindo maior reprodutibilidade.

---

## 🛠️ Tecnologias utilizadas

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📖 Estrutura do notebook

O notebook está organizado em etapas que representam um fluxo completo de um projeto de Machine Learning:

1. Definição do problema
2. Ambiente e bibliotecas
3. Seleção e carga dos dados
4. Análise exploratória (EDA)
5. Preparação dos dados
6. Pipeline de pré-processamento
7. Definição dos modelos
8. Treinamento e avaliação inicial
9. Otimização de hiperparâmetros
10. Avaliação final
11. Comparação dos modelos
12. Boas práticas e rastreabilidade
13. Discussão crítica e limitações
14. Conclusão

---

## 🤖 Modelos avaliados

Foram comparados os seguintes algoritmos:

- DummyClassifier (Baseline)
- Logistic Regression
- Decision Tree
- Random Forest


---

## 🧪 Experimentos realizados

Além do treinamento tradicional, o projeto inclui um experimento adicional para analisar a influência de atributos altamente discriminativos.

Foi realizado um novo treinamento removendo a variável **`odor`**, permitindo avaliar o impacto dessa característica no desempenho dos modelos e discutir a robustez das soluções encontradas.

---

## 📈 Principais resultados

- Construção de um Pipeline completo utilizando Scikit-learn.
- Comparação entre diferentes algoritmos de classificação.
- Otimização automática de hiperparâmetros.
- Avaliação utilizando Accuracy, Precision, Recall, F1-Score e ROC-AUC.
- Discussão sobre generalização, limitações do dataset e possíveis aplicações.

---

## ⚠️ Limitações

Embora o dataset apresente excelente desempenho para os modelos avaliados, algumas limitações devem ser consideradas:

- O conjunto de dados contempla apenas espécies dos gêneros **Agaricus** e **Lepiota**.
- Os dados foram coletados na América do Norte.
- Não há imagens dos cogumelos, apenas atributos categóricos.
- Alguns atributos apresentam valores ausentes e foram tratados por imputação.

---
Caso a URL da UCI esteja indisponível, basta realizar o upload do arquivo `agaricus-lepiota.data` quando solicitado.

---

## 📚 Referências

- UCI Machine Learning Repository – Mushroom Dataset
**Thiago Fernandes**

Projeto desenvolvido para fins acadêmicos na disciplina **Machine Learning & Analytics**.
