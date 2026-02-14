# Tema 2: Análisis Textual y Recursos Lingüísticos

Ejercicios de análisis textual y recursos lingüísticos, abarcando desde tokenización y análisis morfológico hasta análisis sintáctico, semántico y de sentimiento.

- [Ejercicios](#ejercicios)
- [Entorno](#entorno)
- [Datasets](#datasets)

## Ejercicios

Los enunciados de los ejercicios están en `exercises/`, y sus soluciones en `notebooks/`:

- **02_01_analisis_nltk**: Procesamiento básico con NLTK (tokenización, POS tagging, stemming, lematización).

- **02_02_analisis_spacy**: Procesamiento con spaCy (tokenización, lemas, similitud, Matcher/PhraseMatcher).

- **02_03_analisis_sintactico**: Análisis sintáctico (chunking con RegexpParser) y NER con NLTK y spaCy.

- **02_04_expresiones_regulares**: Tareas de PLN con regex (tokenización, normalización, fechas, teléfonos, NER).

- **02_05_analisis_wordnet**: Análisis semántico con WordNet (synsets, similitud, desambiguación WSD).

- **02_06_recursos_linguisticos**: Análisis de sentimiento, clasificación con Naive Bayes, y uso de corpus lingüísticos.


## Entorno


### Instalación

```bash
# Navegar al directorio
cd 02-analisis-textual

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

Los datasets se encuentran en la carpeta `data/`:

- **`Data_Science.txt`** - Texto en inglés sobre ciencia de datos.
- **`Ciencia_de_datos.txt`** - Texto en español sobre ciencia de datos.
- **`openAustralia1.txt`** / **`openAustralia2.txt`** - Textos sobre el Open de Australia.
- **`crisisUcrania.txt`** - Texto sobre la crisis de Ucrania.
- **`atp.txt`** - Texto sobre el circuito ATP.
- **`Cycling.txt`** - Texto sobre ciclismo.
- **`Health_IA.txt`** - Texto sobre salud e IA.
- **`lemmatization-es.txt`** - Recurso para lematización en español.
- **`textsSentimentsPNN.csv`** - Dataset para análisis de sentimientos.
