# Aula 08 - Introdução a Machine Learning para PLN

## Objetivo
Introduzir os fundamentos de aprendizado de máquina aplicados ao Processamento de Linguagem Natural (PLN), com foco em:
- Classificação de texto.
- Regressão utilizando algoritmos como **Naive Bayes** e **SVM (Support Vector Machines)**.

## Conteúdo da Aula
1. **Exemplo 01**: Aplicação do modelo de Naive Bayes para classificação de textos simples:
   - Definição de um corpus com frases e rótulos positivos/negativos.
   - Pré-processamento do texto (tokenização e conversão para minúsculas).
   - Implementação do cálculo de probabilidades e posterior classificação de novos textos.

2. **Exemplo 02**: Uso de **SVM** para classificação de textos:
   - Construção de um corpus com frases rotuladas.
   - Transformação de texto em vetores numéricos usando **TF-IDF**.
   - Treinamento e avaliação de um modelo SVM linear.

3. **Exemplo 03**: Comparação entre Naive Bayes e SVM:
   - Utilização do corpus de avaliações de filmes do **NLTK (Movie Reviews)**.
   - Transformação do texto em vetores com **TF-IDF**.
   - Treinamento e avaliação dos dois modelos utilizando métricas como precisão, recall e F1-score.

## Pré-requisitos
Certifique-se de instalar as dependências antes de executar o código:
- **Python 3.x**
- Bibliotecas:
  - `nltk`
  - `scikit-learn`

Para instalar as dependências:
```bash
pip install nltk scikit-learn
```

## Comandos importantes
- Para baixar o dataset de exemplo do NLTK:
  
```bash
import nltk
nltk.download('movie_reviews')
```

- Para exibir o relatório de classificação:
  
```bash
from sklearn.metrics import classification_report
print(classification_report(y_true, y_pred))
```