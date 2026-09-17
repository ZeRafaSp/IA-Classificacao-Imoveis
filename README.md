# 🏡 Classificação de Imóveis na Califórnia — Machine Learning

#### 📌 Sobre o Projeto
Este repositório contém o desenvolvimento de um modelo de **Machine Learning (Inteligência Artificial)** para prever faixas de preços de imóveis na Califórnia. O projeto foi desenvolvido como parte de uma atividade acadêmica, adaptando o clássico problema de Regressão do Capítulo 2 do livro *"Mãos à Obra: Aprendizado de Máquina com Scikit-Learn & TensorFlow"* para um problema de **Classificação Multiclasse**.

O objetivo de negócio simulado é categorizar os imóveis em três classes de preço (**Baixo, Médio e Elevado**) utilizando técnicas de amostragem estratificada e algoritmos de classificação, fornecendo suporte para estratégias de precificação e análise de mercado.

---

### 🛠️ Tecnologias e Ferramentas Utilizadas
* **Python (Pandas & NumPy):** Aquisição automatizada via URL, limpeza de dados ausentes, categorização por quantis (33.3% e 66.7%) e manipulação estrutural.
* **Scikit-Learn:** Construção de `Pipeline` e `ColumnTransformer`, imputação de dados com `SimpleImputer`, padronização (StandardScaler), One-Hot Encoding e modelagem com **RandomForestClassifier**.
* **Matplotlib:** Análise Exploratória de Dados (EDA), plotagem de histogramas e Matriz de Confusão.
* **Jupyter Notebook / VS Code:** Ambiente interativo de desenvolvimento.

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
```

---

### 📊 Resultados e Métricas de Negócio
O modelo classificador floresta aleatória atingiu uma Acurácia Geral de 80% nos dados de teste isolados. A análise da Matriz de Confusão revelou insights cruciais de precificação:

Alta Precisão nos Extremos: O algoritmo provou ser altamente seguro para identificar os limites do mercado, alcançando um F1-Score de 0.84 para imóveis de preço Baixo e 0.85 para imóveis de preço Elevado. O índice de falsos positivos entre essas duas extremidades foi praticamente nulo.

Fronteira da Classe Média: A categoria Médio apresentou um F1-Score de 0.72. Isso demonstra um comportamento estatístico natural onde imóveis localizados exatamente na fronteira de corte dos quantis possuem características muito semelhantes, concentrando a margem de dúvida do modelo apenas nas zonas de transição.

---

### 📂 Estrutura do Repositório
Plaintext


📁 IA-Classificacao-Imoveis/
│
├── 📄 solucao_housing.ipynb      # Notebook completo (EDA, Pipeline e ML)
├── 📄 README.md                  # Documentação do projeto
└── 📁 datasets/                  # Diretório gerado automaticamente para os dados baixado

---

### 🚧 Roadmap de Desenvolvimento

[x] Fase 1: Aquisição automatizada dos dados e Análise Exploratória (EDA).

[x] Fase 2: Engenharia de Atributos (Criação do target multiclasse).

[x] Fase 3: Separação estratificada (80/20) e imputação de valores ausentes pela mediana.

[x] Fase 4: Tratamento de variáveis categóricas (One-Hot Encoding) e Padronização.

[x] Fase 5: Treinamento de Modelos e Avaliação de Métricas (Acurácia, F1-Score e Matriz de Confusão).

👨‍💻 Autor
José Rafael Santos Pereira
Desenvolvendo soluções práticas de dados | Power BI | SQL | Python | Machine Learning

LinkedIn:  https://www.linkedin.com/in/rafaelsantospereirarsp/

GitHub:  https://github.com/ZeRafaSp/