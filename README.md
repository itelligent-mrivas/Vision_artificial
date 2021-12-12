# Vision artificial

Este repositorio contiene códigos de ejemplos para la realización de Caso de Uso de *Visión artificial*.

Cada uno de estos ejemplos se encuentra en un Jupyter Notebook.

Ademas de los Jupyter Notebook, se encuentra las siguientes carpetas:

- `recursos_yolo`. Carpeta con los ficheros de configuracion de YOLO. Debido al tamaño del fichero es necesario realizar la descarga de pesos de yolov3, que se puede realizar desde el siguiente link https://pjreddie.com/media/files/yolov3.weights
- `datasets`. Carpeta donde se leen los datos necesarios para los ejercicios
- `salidas`. Carpeta donde se escriben las imagenes de salida

## Ejemplos

### 1. Detección de elementos

En este ejemplo se implementa la detección de objetos haciendo uso de Yolo. Este ejercicio se ha realizado de dos formas distintas, que son:

- **OPCIÓN 1**. Haciendo uso de DarkFlow. Esta opcion ofrece una mejor calidad pero una mayor complejidad en la instalación. [Notebook](https://github.com/itelligent-mrivas/Vision_artificial/blob/main/Deteccion_elementos_yolo.ipynb)
- **OPCION 2**. Hacienndo uso de OpenCV, lo cual facilita enormemente la intalación. [Notebook](https://github.com/itelligent-mrivas/Vision_artificial/blob/main/deteccion%20de%20elementos_openCV.ipynb)