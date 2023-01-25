# Segundo Proyecto Individual

Para este proyecto se nos otorgo un dataset relacionado con la venta de inmuebles de Estados Unidos y segun sus caracteristicas lograr clasificarlos si estos son caros(0) o son baratos(1), estos datos de testeo y entrenamiento se han obtenido del siguiente link:
https://drive.google.com/drive/folders/1nJ9ZMj6E6zh6McC9NwCA6KopfUIOG_1O
Se comparte este link debido a que no se pudo subir los datasets originales al repositorio debido a que excedian el tamaño permitido en github.

En este repositorio se compartio 3 notebooks donde se desarrollo el proyecto, vamos a explicar brevemente lo que se hizo en cada uno:

-Limpieza.ipynb: en este notebook se limpio el dataset de entrenamiento, eliminando valores duplicados comprobando la republicacion de venta de un inmueble, tambien se eliminaron outliers, se agrego la columna 'target', el tratamiento de lo valores nulos y la conversion de valores string a numericos. En cada paso proporcionando una grafica para analizar los datos tanto su correlacion y proporcion, finalmente retornando el archivo train_numerico.csv.

-Modificacion_de_test.ipynb : se modifica el dataset a testear al igual que el dataset de entrenamiento solo que sin eliminar filas para que en el proceso de prediccion la dimension del resultado no sea afectada, retornando el archivo test_numerico.csv.

 -Prediccion.ipynb: se usa el modelo supervisado de arbol de decisiones, aplicando el entrenamiento en el archivo train_numerico.csv y obteniendo las predicciones a partir del archivo train_numerico.csv.

El codigo esta debidamente comentado cada paso que se ejecuto. Se podria sumar a manera de conclusion que aunque el modelo predictivo usado retorno un acurrancy y recall considerable, este pudo aumentar si no tuvieramos en cuenta los valores nulos que se presentaron en el dataset de testeo en las columnas de latitud y longitud, aunque se podria hacer uso de librerias alternativas para la ubicacion a partir de los datos de region y estado, o tambien usar apis es una opcion, aunque esto no se aplico en el proceso, se puede tomar en cuenta para futuros trabajos.