# VTD - Test Data Science - Regresión Series Temporales

Este [repositorio](https://github.com/victosdur/VTD-TestDataScience-Regresion.git) contiene los datos y experimentos realizados referente a un ejemplo práctico, el cuál tiene como objetivo aplicar técnicas de data science e inteligencia artificial a un conjunto de datos de regresión, con la peculariedad de que la tipología de los datos corresponda con series temporales multivariantes. El objetivo principal será predecir valores futuros de la variable objetivo, por lo que estamos en un caso de regresión.

## Uso

1. Clonar este repositorio/carpeta:

```
git clone https://github.com/victosdur/VTD-TestDataScience-Regresion.git 
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

- `data\`: Contiene los datos usados en la experimentación.

- `results\`: Contiene el archivo referente al modelo finalmente seleccionado, así como el archivo del procesamiento a aplicar a los datos para que estos sean recibidos de manera correcta por el modelo.

- `figures\`: Contiene las imágenes generadas durante la experimentación.

- `requeriments.txt`: Contiene todas las dependencias del proyecto.

- `notebooks\`: Contiene el notebook (en este caso solo 1) en el que se lleva a cabo todo el proceso de carga de los datos, así como la experimentación posterior.

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
```
