# SISTEMA DE AGRUPACION DE CASAS  

Queremos ser capaces de clasificar casas según su la región en la que se encuentren y del ingreso medio. Para ello, utilizaremos el famoso conjunto de datos California Housing. Se construyó utilizando los datos del censo de California de 1990. Contiene una fila por grupo de bloques censales. Un grupo de bloques es la unidad geográfica más pequeña para la que se publican datos del censo de USA.

Paso 1: Carga del conjunto de datos

Paso 2: Construimos un K-Means
Clasificamos los datos en 6 clusters utilizando, para ello, el modelo K-Means. 
Almacenamos el cluster al que pertenece cada casa como una columna nueva del dataset. 
Observamos qué formato y valores tiene y actúamos en consecuencia. 
Grafícamos en un diagrama de puntos y describimos.

Paso 3: Predice con el conjunto de test
Utilizamos el modelo entrenado con el conjunto test y añadimos los puntos al gráfico anterior para confirmar que la predicción es satisfactoria o no.

Paso 4: Entrenamos un modelo de clasificación supervisada
Una vez que el K-Means nos ha devuelto una categorización (agrupación) de los puntos para los conjuntos de entrenamiento y prueba, estudiamois qué modelo podría ser más útil y lo entrénamos. 
Obtenemos las estadísticas y describimos.

Este flujo es muy común cuando contamos con datos no etiquetados: utilizar un modelo de aprendizaje no supervisado para etiquetarlos de forma automática y a continuación, un modelo de aprendizaje supervisado.

Paso 5: Guardamos los modelos

# ESTRUCTURA

The project is organized as follows:

- `app.py` - The main Python script that you run for your project.
- `explore.py` - A notebook to explore data, play around, visualize, clean, etc. Ideally the notebook code should be migrated to the app.py when moving to production.
- `utils.py` - This file contains utility code for operations like database connections.
- `requirements.txt` - This file contains the list of necessary python packages.
- `models/` - This directory should contain your SQLAlchemy model classes.
- `data/` - This directory contains the following subdirectories:
  - `interin/` - For intermediate data that has been transformed.
  - `processed/` - For the final data to be used for modeling.
  - `raw/` - For raw data without any processing.
 
    
## Setup

**Prerequisites**

Make sure you have Python 3.11+ installed on your. You will also need pip for installing the Python packages.

**Installation**

Clone the project repository to your local machine.

Navigate to the project directory and install the required Python packages:

```bash
pip install -r requirements.txt
```

## Running the Application

To run the application, execute the app.py script from the root of the project directory:

```bash
python app.py
```

## Contributors

This template was built as part of the 4Geeks Academy [Data Science and Machine Learning Bootcamp](https://4geeksacademy.com/us/coding-bootcamps/datascience-machine-learning) by [Alejandro Sanchez](https://twitter.com/alesanchezr) and many other contributors. Find out more about [4Geeks Academy's BootCamp programs](https://4geeksacademy.com/us/programs) here.

Other templates and resources like this can be found on the school GitHub page.
