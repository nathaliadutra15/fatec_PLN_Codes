- Introduzir os fundamentos de modelagem de tópicos com LDA e realizar uma prática guiada para implementar o modelo em um corpus de notícias, permitindo aos alunos identificar automaticamente tópicos em textos extensos.

## O que aprendemos:
1. **O que é LDA?**
   - LDA é um modelo generativo de modelagem de tópicos que tenta entender o processo que gerou os documentos.
   - Assume que:
     - Cada documento é composto por uma mistura de tópicos.
     - Cada tópico é uma distribuição de palavras.

2. **Etapas Práticas**
   - Preparo de corpus para análise.
   - Implementação do modelo LDA com `gensim`.
   - Visualização de tópicos utilizando a biblioteca `pyLDAvis`.

---

## Exemplo 01 - Implementação do LDA em um Corpus de Notícias

O exemplo utiliza o corpus `Reuters` da biblioteca `nltk` para demonstrar a modelagem de tópicos. As etapas incluem:

- **Pré-processamento:** Tokenização, remoção de stopwords e lematização.
- **Criação do Dicionário e Corpus:** Representação BoW para análise.
- **Treinamento do Modelo:** Geração de 5 tópicos principais.

```python
# Etapas principais do código
# Pré-processamento
from nltk.corpus import stopwords
from nltk.tokenize import word_tokenize
from nltk.stem import WordNetLemmatizer
from nltk.corpus import reuters

# Configuração do LDA
from gensim.corpora import Dictionary
from gensim.models import LdaModel

# Visualização
import pyLDAvis.gensim_models as gensimvis
lda_vis = gensimvis.prepare(lda_model, corpus, dictionary)
pyLDAvis.display(lda_vis)
```

## Exemplo 02 - Implementação do LDA com um Corpus Personalizado

**Utilizamos um pequeno corpus de frases para demonstrar a modelagem de tópicos:**

- **Pré-processamento:** Tokenização das frases.
- **Criação do Dicionário e Corpus:** Transformação em representação BoW.
- **Treinamento do Modelo: Criação** de 5 tópicos utilizando o corpus.
  
**Exemplo de Frases no Corpus:**

- "Eu gosto de aprender sobre inteligência artificial e ciência de dados"
- "A análise de dados é muito importante em projetos de aprendizado de máquina"
- "Redes neurais são úteis para processamento de linguagem natural"
- "A modelagem de tópicos ajuda a descobrir temas em textos grandes"
- "Python é uma ferramenta poderosa para trabalhar com PLN"

**Código para Treinamento:**
```python
from nltk.tokenize import word_tokenize
from gensim.corpora import Dictionary
from gensim.models import LdaModel

# Pré-processamento
tokenized_docs = [word_tokenize(doc.lower()) for doc in documents]

# Criando Dicionário e Corpus
dictionary = Dictionary(tokenized_docs)
corpus_bow = [dictionary.doc2bow(doc) for doc in tokenized_docs]

# Modelo LDA
lda_model = LdaModel(
    corpus=corpus_bow,
    id2word=dictionary,
    num_topics=5,
    passes=10,
    random_state=42
)

# Visualização:
A visualização é feita utilizando pyLDAvis:

lda_vis = gensimvis.prepare(lda_model, corpus_bow, dictionary)
pyLDAvis.display(lda_vis)
```

## Ferramentas e Bibliotecas Utilizadas:
- Python 3.x
- NLTK
- Gensim
- pyLDAvis
  
## Como executar:
- Certifique-se de que as bibliotecas estão instaladas:

```python
pip install nltk gensim pyLDAvis
```