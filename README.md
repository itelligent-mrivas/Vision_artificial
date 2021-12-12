# Vision artificial

Este repositorio contiene códigos de ejemplos para la realización de Caso de Uso de *Visión artificial*.

Cada uno de estos ejemplos se encuentra en un Jupyter Notebook.

Ademas de los Jupyter Notebook, se encuentra las siguientes carpetas:

- `recursos_yolo`. Carpeta con los ficheros de configuracion de YOLO. Debido al tamaño del fichero es necesario realizar la descarga de pesos de yolov3, que se puede realizar desde el siguiente link https://pjreddie.com/media/files/yolov3.weights
- `datasets`. Carpeta donde se leen los datos necesarios para los ejercicios
- `salidas`. Carpeta donde se escriben las imagenes de salida

## Paquetes necesarios

A continuación se describirán los paquetes utilizados en los ejercicios, así como su proceso de instalación 

### Tensor Flow

Biblioteca de aprendizaje automático, que toman como base muchas otras de las que usaremos

`conda install tensorflow`

### Instalar keras

Esta librería proporciona modelos de deep learning, entre ellos modelos preentrenados de CNN.

`conda install keras`

### Instalar PIL

Biblioteca que proporciona funcionalidades para el procesamiento de imágenes

`conda install pillow`

### Open CV

Biblioteca para el procesamiento de imágenes

`conda install -c menpo opencv`

### Darkflow

Biblioteca para el uso de los modelos de YOLO.

Para la instalación de esta biblioteca es necesaria su descarga desde github (https://github.com/thtrieu/darkflow), ya que no se encuentra disponible en ningún gestor de paquetes.

Una vez descargado el proyecto se debe ir a la carpeta en la que se encuentra este y ejecutar:

```
python setup.py build_ext --inplace
pip install -e .
```

También es necesario descargar los pesos de entrenamiento para YOLOv2 608x608 desde el siguiente enlace (https://pjreddie.com/darknet/yolov2/), colocando estos dentro de una carpeta llamada bin en la carpeta donde se tiene descargado Darkflow.

## Ejemplos

### 1. Detección de elementos

En este ejemplo se implementa la detección de objetos haciendo uso de Yolo. Este ejercicio se ha realizado de dos formas distintas, que son:

- **OPCIÓN 1**. Haciendo uso de DarkFlow. Esta opcion ofrece una mejor calidad pero una mayor complejidad en la instalación. [Notebook](https://github.com/itelligent-mrivas/Vision_artificial/blob/main/1_1_Deteccion_elementos_yolo.ipynb)
- **OPCION 2**. Hacienndo uso de OpenCV, lo cual facilita enormemente la intalación. [Notebook](https://github.com/itelligent-mrivas/Vision_artificial/blob/main/1_2_deteccion%20de%20elementos_openCV.ipynb)

### 2. Extraccion de *features* 

En este ejemplo se implementa el código para la extraccion de *features* de alto nivel para imágenes haciendo uso de CNN.

### 3. Clasificación

En este ejemplo se realiza un clasificador que permite detectar personas que llevan chaleco o no. Haciendo uso de las *features* extraidas.

### 4. Ejercicio final