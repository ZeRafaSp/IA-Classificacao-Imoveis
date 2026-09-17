# 🏡 Classificação de Imóveis na Califórnia — Machine Learning

#### 📌 Sobre o Projeto
Este repositório contém o desenvolvimento de um modelo de **Machine Learning (Inteligência Artificial)** para prever faixas de preços de imóveis na Califórnia. O projeto foi desenvolvido como parte de uma atividade acadêmica, adaptando o clássico problema de Regressão do Capítulo 2 do livro *"Mãos à Obra: Aprendizado de Máquina com Scikit-Learn & TensorFlow"* para um problema de **Classificação Multiclasse**.

O objetivo de negócio simulado é categorizar os imóveis em três classes de preço (**Baixo, Médio e Elevado**) utilizando técnicas de amostragem estratificada e algoritmos de classificação, fornecendo suporte para estratégias de precificação e análise de mercado.

---

### 🛠️ Tecnologias e Ferramentas Utilizadas
* **Python (Pandas & NumPy):** Aquisição, limpeza de dados ausentes, categorização por quantis e manipulação estrutural.
* **Scikit-Learn:** Separação de dados em treino e teste (amostragem estratificada), imputação de dados com `SimpleImputer` e treinamento de modelos.
* **Matplotlib:** Análise Exploratória de Dados (EDA) e plotagem de histogramas.
* **Jupyter Notebook / VS Code:** Ambiente de desenvolvimento interativo.

---

### ⚙️ Arquitetura e Pipeline dos Dados

```text
[Dados Brutos do Censo Imobiliário] 
       │
       ▼
[01. Python (Pandas)] ──► Conversão de Preço Contínuo em Classes (Tercis: 33% e 66%)
       │
       ▼
[02. Scikit-Learn] ──► Separação Estratificada (Treino/Teste) e Tratamento de Nulos (Imputer)
       │
       ▼
[03. Machine Learning] (Em Desenvolvimento) ──► Treinamento, Validação Cruzada e Avaliação

---

### 🚧 Roadmap de Desenvolvimento

[x] Fase 1: Aquisição automatizada dos dados e Análise Exploratória (EDA).

[x] Fase 2: Engenharia de Atributos (Criação do target multiclasse).

[x] Fase 3: Separação estratificada (80/20) e imputação de valores ausentes pela mediana.

[ ] Fase 4: Tratamento de variáveis categóricas (One-Hot Encoding) e Padronização.

[ ] Fase 5: Treinamento de Modelos e Avaliação de Métricas (Acurácia, F1-Score e Matriz de Confusão).

👨‍💻 Autor
José Rafael Santos Pereira
Desenvolvendo soluções práticas de dados | Power BI | SQL | Python | Machine Learning

LinkedIn:  https://www.linkedin.com/in/rafaelsantospereirarsp/

GitHub:  https://github.com/ZeRafaSp/