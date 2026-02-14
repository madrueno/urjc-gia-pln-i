# Tema 3: Representación del Texto

Ejercicios de representación del texto, abarcando desde métodos clásicos hasta embeddings estáticos y contextuales.

- [Ejercicios](#ejercicios)
- [Entorno](#entorno)
- [Datasets](#datasets)
- [Modelos](#modelos)

## Ejercicios

Los enunciados de los ejercicios están en `exercises/`, y sus soluciones en `notebooks/`, con el mismo nombre base:

- **03_01_bolsa_palabras**: Representación clásica basada en conteos (BoW/TF-IDF), vectorización y primeros análisis.

- **03_02_matriz_coocurrencias**: Construcción de matrices de coocurrencia basadas en ventanas de contexto. Comparación de métricas de similitud usando coocurrencias directas vs PPMI (Positive Pointwise Mutual Information).

- **03_03_modelos_latentes**: Latent Dirichlet Allocation para descubrir tópicos. Exploración de hiperparámetros (alpha, beta, número de tópicos) y evaluación.

- **03_04_embeddings_estaticos**: Embeddings estáticos preentrenados de diferentes fuentes (Google News, Wiki Gigaword, Facebook). Analogías semánticas, visualización con PCA y similitudes entre oraciones.

- **03_05_embeddings_estaticos_plus**: Técnicas avanzadas: Sense2Vec para desambiguación de sentidos según etiquetas POS, y Doc2Vec para representaciones a nivel de documento. Entrenamiento con abstracts de Wikipedia.

- **03_06_recuperacion_informacion**: Aplicación práctica de diferentes representaciones (TF-IDF, Word2Vec, Doc2Vec) a recuperación de información sobre corpus de noticias falsas en español. Evaluación del impacto del preprocesamiento.

- **03_07_embeddings_contextuales**: Embeddings contextuales que generan representaciones dinámicas según el contexto. ELMo (TensorFlow Hub), BERT (Transformers) con extracción de capas ocultas, y Sentence-BERT para similitud semántica.



## Entorno


### Instalación

```bash
# Navegar al directorio
cd 03-representacion-texto

# Instalar dependencias
uv sync
```

### Ejecución

**VSCode**

Abre el directorio y selecciona el kernel del entorno virtual:

```bash
code .
```

**Jupyter Lab**
```bash
uv run jupyter lab
```

## Datasets

Los datasets requeridos se encuentran incluidos en la carpeta `data/`:

- **`Noticias.json`** - Artículos de noticias en español para modelado de tópicos y coocurrencias.
- **`train.xlsx`** - Corpus de Fake News obtenido de https://github.com/jpposadas/FakeNewsCorpusSpanish

## Modelos

Todos los comandos deben ejecutarse desde la carpeta `03-representacion-texto` y guardarse dentro de la carpeta `models/`:


**FastText - Wiki Simple**

Descarga por terminal
```bash
cd models && \
  wget https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/wiki.simple.zip && \
  unzip wiki.simple.zip
```

Descarga manual
1. Descarga el archivo desde tu navegador: https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/wiki.simple.zip
2. Extrae el archivo `wiki.simple.bin` en la carpeta `models/`


**Sense2Vec - Reddit 2015**


Descarga por terminal
```bash
cd models && \
  wget https://github.com/explosion/sense2vec/releases/download/v1.0.0/s2v_reddit_2015_md.tar.gz && \
  tar -xzf s2v_reddit_2015_md.tar.gz
```

Descarga manual
1. Descarga el archivo desde tu navegador: https://github.com/explosion/sense2vec/releases/download/v1.0.0/s2v_reddit_2015_md.tar.gz
2. Extrae la carpeta `models/s2v_old/` en la carpeta `models/`


**Word Embeddings para Español - Kaggle**

Descarga manual
1. Descarga el dataset desde Kaggle: https://www.kaggle.com/datasets/rtatman/pretrained-word-vectors-for-spanish
2. Extrae el archivo `SBW-vectors-300-min5.txt` en la carpeta `models/`
