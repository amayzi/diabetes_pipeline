# 🩺 Esteira de Aprendizado de Máquina — Predição de Diabetes
 
Projeto desenvolvido para a disciplina de Machine Learning do curso de Análise e Desenvolvimento de Sistemas — FATEC Praia Grande.
 
## Descrição
 
Este notebook implementa uma esteira completa de aprendizado de máquina para **classificação binária**, prevendo se um paciente tem ou não diabetes com base em dados clínicos.
 
**Dataset:** [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  
**Fonte dos dados:** Repositório público (carregado automaticamente via URL)  
**Modelo:** Random Forest Classifier  
 
### Etapas implementadas
 
| # | Etapa |
|---|-------|
| 1 | Carregamento e exploração dos dados |
| 2 | Estatísticas descritivas e visualizações |
| 3 | Transformação nas **colunas** — substituição de zeros inválidos pela mediana |
| 4 | Transformação nas **linhas** — remoção de duplicatas e outliers via IQR |
| 5 | Divisão em treino (60%), validação (20%) e teste (20%) |
| 6 | Normalização com StandardScaler |
| 7 | Treinamento do modelo Random Forest |
| 8 | Avaliação: matriz de confusão e acurácia |
| 9 | Predição para nova paciente |
 
---
 
## Estrutura do Repositório
 
```
.
├── diabetes_pipeline.ipynb   # Notebook principal com toda a esteira
└── README.md                 # Este arquivo
```
 
---
 
## Como reproduzir
 
### Pré-requisitos
 
- Python 3.8+
- Jupyter Notebook ou [Google Colab](https://colab.research.google.com/) (recomendado)
### Opção 1 — Google Colab (mais fácil, sem instalação)
 
1. Acesse [colab.research.google.com](https://colab.research.google.com/)
2. Clique em **Arquivo > Fazer upload de notebook**
3. Selecione o arquivo `diabetes_pipeline.ipynb` deste repositório
4. Clique em **Ambiente de execução > Executar tudo** (`Ctrl+F9`)
> O dataset é carregado automaticamente via URL — não é necessário baixar nada.
 
### Opção 2 — Ambiente local
 
```bash
# 1. Clone o repositório
git clone https://github.com/amayzi/diabetes_pipeline.git
cd SEU_REPOSITORIO
 
# 2. Instale as dependências
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
 
# 3. Abra o notebook
jupyter notebook diabetes_pipeline.ipynb
```
 
4. No Jupyter, clique em **Kernel > Restart & Run All**
---
 
## Dependências
 
```
pandas
numpy
matplotlib
seaborn
scikit-learn
```
 
---
 
## Resultados esperados
 
- **Acurácia no teste:** ~75–80%
- **Feature mais relevante:** Glicose (consistente com a literatura médica)
- **Saídas geradas:** matriz de confusão, gráfico de importância das features e predição para nova paciente
---
 
## Autora
 
**Mayara Zimmermann Xavier**  
Análise e Desenvolvimento de Sistemas — FATEC Praia Grande
