# Tema 4: Redes Neuronales en PLN

Ejercicios de redes neuronales aplicadas a clasificación de texto, abarcando desde redes feedforward y convolucionales hasta redes recurrentes (RNN, LSTM, Bi-LSTM).

- [Ejercicios](#ejercicios)
- [Entorno](#entorno)
- [Datasets](#datasets)
- [Modelos](#modelos)

## Ejercicios

Los enunciados de los ejercicios están en `exercises/`, y sus soluciones en `notebooks/`:

- **04_01_mlp_cnn**: Clasificación de sentimiento con MLP y CNN (Keras/TensorFlow, embeddings, tweets en español).

- **04_02_rnn_lstm**: Detección de noticias falsas con redes recurrentes (SimpleRNN, LSTM, Bi-LSTM, Word2Vec).



## Entorno


### Instalación

```bash
# Navegar al directorio
cd 04-redes-neuronales

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

- **`train.xlsx`** - Corpus de Fake News en español obtenido de https://github.com/jpposadas/FakeNewsCorpusSpanish. Contiene títulos (Headline), contenido (Text) y categoría (True/Fake). Utilizado en el Listado 2. Debe descargarse y colocarse en la carpeta `data/`.

- **Tweet Sentiment Multilingual** - Dataset de Hugging Face (`cardiffnlp/tweet_sentiment_multilingual`). Se descarga automáticamente desde el notebook.

## Modelos

Todos los comandos deben ejecutarse desde la carpeta `04-redes-neuronales` y guardarse dentro de la carpeta `models/`:

**Word Embeddings para Español - Kaggle**

Descarga manual
1. Descarga el dataset desde Kaggle: https://www.kaggle.com/datasets/rtatman/pretrained-word-vectors-for-spanish
2. Extrae el archivo `SBW-vectors-300-min5.txt` en la carpeta `models/`
