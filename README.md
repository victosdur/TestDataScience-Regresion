# VTD - Test Data Science - Regresión Series Temporales

Este [repositorio](https://github.com/victosdur/TestDataScience-Regresion.git) contiene los datos y experimentos realizados referente a un ejemplo práctico, el cuál tiene como objetivo aplicar técnicas de data science (como limpieza, transformación, visualización de datos, y análisis de series temporales), asi como de inteligencia artificial, a un conjunto de datos de regresión, con la peculariedad de que la tipología de los datos corresponda con series temporales multivariantes. El objetivo principal será predecir valores futuros de la variable objetivo, por lo que estamos en un caso de regresión. En este caso será de predecir los futuros valores del consumo de gasolina en españa-

## Uso

1. Clonar este repositorio/carpeta:

```
git clone https://github.com/victosdur/TestDataScience-Regresion.git 
```

2. Crear un entorno virtual (en concreto este proyecto se ha desarrollado usando Python3.10.11). Particularmente, me gusta crear un entorno virtual para proyecto que voy a llevar a cabo, para no mezclar dependencias que puedan ser requeridas en otros proyectos. Para ello suelo proceder con la herramienta virtualenv de Python. De la misma manera, por agilizar la creación y activación de los entornos, suele denominarlos por `env`.

```
virtualenv -p python env # pip install virtualenv - instalarlo si no lo tienes instalado 
```

3. Activar el entorno virtual:

```
env\Scripts\activate
```

4. Instalar las dependencias necesarias:

```
pip install requeriments.txt
```


## Estructura del repositorio

- `requeriments.txt`: Contiene todas las dependencias del proyecto.

- `data\`: Contiene los datos usados en la experimentación.

- `results\`: Contiene el archivo referente al modelo finalmente seleccionado, así como un csv con las métricas de distintos modelos de predicción.

- `figures\`: Contiene las imágenes generadas durante la experimentación.

- `notebooks\`: Contiene el notebook (en este caso solo 1, `analisis.ipynb`) en el que se lleva a cabo todo el proceso de carga, limpieza, visualización de los datos, así como del análisis y la experimentación posterior.

- `outputs\`: Contiene los outputs de los notebooks en formato html, incluyendo el código y la salida de los mismos.

## Uso particular en VScode (usado habitualmente por mi parte como entorno de desarrollo).

Para poder seleccionar y ejecutar como `kernel` el referente al entorno creado en vscode, instalar ipykernel.

```
pip install ipykernel #incluido een el requeriments
```

Para obtener el pdf/html de los notebooks desarrollados hay que instalar y usar la herramienta nbconvert:

```
pip install jupyter nbconvert # instalación, jupyter y nbconvert necesario para poder ejecutar el siguiente comando
jupyter nbconvert --to html --execute notebook.ipynb --output notebook.html # incluye código y salidas
jupyter nbconvert --to html --execute notebooks/analisis.ipynb --output analisis.html --output-dir outputs/ # en el caso de querer producir el html del notebook analisis.ipynb del proyecto
```
