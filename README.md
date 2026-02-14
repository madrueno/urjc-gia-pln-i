# Procesamiento del Lenguaje Natural I

[![SWH](https://archive.softwareheritage.org/badge/swh:1:dir:6eb4b542c8b99bf3f4b5ebae14f6822b0aaa8635/)](https://archive.softwareheritage.org/swh:1:dir:6eb4b542c8b99bf3f4b5ebae14f6822b0aaa8635;origin=https://github.com/madrueno/urjc-gia-pln-i;visit=swh:1:snp:365d51cf1e6a3a418c3672d78848d3048d5b3b63;anchor=swh:1:rev:647b40cdde3c7f4067662f5f656832d7f6e0c373)

Material docente en abierto de la Universidad Rey Juan Carlos para la asignatura de Procesamiento del Lenguaje Natural I del Grado en Inteligencia Artificial.

Este repositorio incluye ejercicios prácticos y códigos de ejemplo:
- **GitHub**: [madrueno/urjc-gia-pln-i](https://github.com/madrueno/urjc-gia-pln-i)
- **Software Heritage**: [swh:1:dir:6eb4b542c8b99bf3f4b5ebae14f6822b0aaa8635](https://archive.softwareheritage.org/swh:1:dir:6eb4b542c8b99bf3f4b5ebae14f6822b0aaa8635)

Actualizado el 14/02/2026. Elaborado por:
- Soto Montalvo Herranz (soto.montalvo@urjc.es) - URJC
- Natalia Madrueño Sierro (natalia.madrueno@urjc.es) - URJC


## Índice de Temas

1. [Introducción al PLN](01-introduccion-pln/)
2. [Análisis textual y recursos lingüísticos](02-analisis-textual/)
3. [Representación del texto](03-representacion-texto/)
4. [Redes neuronales en PLN](04-redes-neuronales/)
5. [Transformers y modelos de lenguaje](05-transformers/)
6. [Aumento de Datos](06-aumento-datos/)
7. [Reconocimiento de entidades nombradas](07-entidades-nombradas/)

## Requisitos Previos

- **Python 3.12+** (recomendado)
- **uv** - Gestor de dependencias

Puedes instalar uv mediante los siguientes comandos:
```bash
# Linux/macOS
curl -LsSf https://astral.sh/uv/install.sh | sh

# Windows
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"

# Alternativamente con pip
pip install uv
```

## Cómo Usar este Repositorio

### Estructura del Repositorio

Cada tema tiene su propia carpeta. El primer tema proporciona un proyecto de ejemplo de procesamiento del lenguaje natural. A partir del segundo tema la estructura base tiene la siguiente forma:

```bash
XX-nombre/
├── README.md          # Descripción y contenidos del tema
├── pyproject.toml     # Dependencias específicas
├── uv.lock            # Lockfile del entorno
├── exercises/         # Enunciados de los ejercicios
├── notebooks/         # Ejercicios resueltos con notebooks
├── data/              # Datasets empleados para resolverlos
└── models/            # Modelos descargados y entrenados
```

### 1. Clonar el repositorio

```bash
git clone git@github.com:madrueno/urjc-gia-pln-i.git
cd urjc-gia-pln-i
```

### 2. Trabajar con un tema específico

Cada tema tiene sus propias dependencias aisladas. Hay dos formas principales de trabajar:

#### Opción A: Usando VSCode (Recomendado)

```bash
# Navegar al tema deseado
cd 03-representacion-texto

# Instalar dependencias y crear entorno virtual
uv sync

# Abrir en VSCode
code .
```

Luego, en VSCode:
1. Abre un notebook (archivo `.ipynb`)
2. VSCode detectará automáticamente el entorno `.venv/`
3. Selecciona el kernel de Python del `.venv/` si no se selecciona automáticamente
4. Comienza a trabajar directamente en VSCode

#### Opción B: Usando Jupyter Lab/Notebook (Terminal)

```bash
# Navegar al tema deseado
cd 03-representacion-texto

# Instalar dependencias y crear entorno virtual
uv sync

# Ejecutar Jupyter Lab (interfaz moderna)
uv run jupyter lab

# O Jupyter Notebook (interfaz clásica)
uv run jupyter notebook
```

### Convenciones de Nomenclatura

#### Temas
- Formato: `XX-nombre` donde XX es el número del tema (01-07)
- Ejemplo: `03-representacion-texto`

#### Ejercicios
- Formato: `XX_MM_nombre`
  - `XX` = número del tema
  - `MM` = número del notebook dentro del tema
  - `nombre` = descripción breve
- Ejemplos: `03_01_bolsa_palabras.pdf`, `03_01_bolsa_palabras.ipynb`


## Licencia

Este trabajo está licenciado bajo [Creative Commons Reconocimiento-CompartirIgual 4.0 Internacional](https://creativecommons.org/licenses/by-sa/4.0/).

>©2026 Soto Montalvo Herranz, Natalia Madrueño Sierro.
>Algunos derechos reservados  
>Este documento se distribuye bajo la licencia  
>“Atribución-CompartirIgual 4.0 Internacional” de Creative Commons, disponible en  
>https://creativecommons.org/licenses/by-sa/4.0/deed.es