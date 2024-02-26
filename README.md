# Prueba Final

En este estudio, se explora el rendimiento de diferentes optimizadores al clasificar un conjunto de datos de imágenes de carnes. El conjunto de datos utilizado contiene diversas clases de carnes y se emplea para entrenar modelos de redes neuronales convolucionales (CNN) con el objetivo de clasificar correctamente las imágenes según su tipo de carne. Se evalúan tres optimizadores populares: Adam, Nadam y Adamax, considerando su efecto en la precisión del modelo y su capacidad para generalizar a datos no vistos. A lo largo de este análisis, se detallan los pasos desde la carga y preparación de los datos hasta la evaluación y comparación de los modelos entrenados. Este estudio proporciona una visión integral sobre la importancia de la selección del optimizador en el proceso de entrenamiento de modelos de aprendizaje automático para tareas de clasificación de imágenes.

# Importación de Librerías:
Se importan varias bibliotecas necesarias para el procesamiento de imágenes y el entrenamiento de modelos de redes neuronales, incluyendo TensorFlow, Matplotlib y NumPy.
Además, se importan funciones específicas de estas bibliotecas, como ImageDataGenerator para la generación de datos de imágenes y confusion_matrix para evaluar la precisión del modelo.
# Carga de Datos de Entrenamiento
Se carga un conjunto de datos de imágenes de carne desde un directorio especificado, dividiéndolo en un conjunto de entrenamiento y un conjunto de validación con una proporción del 80/20.
Las imágenes se redimensionan a un tamaño de 300x300 píxeles.
# Visualización de Ejemplos de Datos de Entrenamiento
Se muestran algunas imágenes de muestra del conjunto de entrenamiento junto con sus etiquetas correspondientes.
Se imprime el número de lotes de entrenamiento en el conjunto de datos.
# Preparación del Conjunto de Datos de Entrenamiento
Se establece el número de clases y se define el conjunto de datos de entrenamiento para su uso posterior.
Se define la arquitectura del modelo de red neuronal convolucional utilizando capas de convolución, agrupación máxima, aplanamiento y capas completamente conectadas.
Se imprime un resumen del modelo para ver su estructura.
# Entrenamiento del Modelo con Distintos Optimizadores
Se compila y entrena el modelo utilizando tres optimizadores diferentes: Adam, Nadam y Adamax.
Se guardan los historiales de entrenamiento de cada modelo para su posterior visualización.
# Visualización de Pérdida de Entrenamiento
Se grafica la pérdida de entrenamiento en función del número de épocas para cada modelo entrenado con los distintos optimizadores.
# Visualización de Precisión de Entrenamiento
Se grafica la precisión de entrenamiento en función del número de épocas para cada modelo entrenado con los distintos optimizadores.
# Guardado y Carga de Modelos Entrenados
Se guardan los modelos entrenados con cada optimizador en archivos HDF5.
Se cargan los modelos guardados para su posterior evaluación y uso.
# Evaluación del Modelo en un Conjunto de Datos de Prueba
Se cargan datos de prueba desde un directorio específico.
Se evalúan los modelos entrenados utilizando los datos de prueba y se imprimen los resultados de pérdida y precisión.
# Visualización de la Matriz de Confusión
Se calculan las matrices de confusión para cada modelo utilizando los datos de prueba.
Se visualizan las matrices de confusión para analizar el rendimiento del modelo en la clasificación de cada clase.
# Resumen Final
Se concluye que el optimizador Nadam no es adecuado para el entrenamiento de estos datos debido a su bajo rendimiento.
Se proporciona una visualización completa del rendimiento de los modelos entrenados con los optimizadores Adam y Adamax en términos de precisión y confusión entre clases.
Teniendo como resultado que ambos se manejan de manera similar. 
Para este modelo 10 convuluciones son suficientes, pero podria funcionar bien desde las 8. 
