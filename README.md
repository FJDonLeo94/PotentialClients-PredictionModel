# PotentialClients-PredictionModel

Este repo trata sobre una red neuronal creada y entrenada utilizando un dataframe, a esta red neuronal se le ha creado una API y un demo utilizando Gradio.

El modelo toma tres variables sobre gente que navega en la pagina web de una tienda y predice cual de esos potenciales clientes pasan a clientes reales. 

La eficacia del modelo no es especialmente alta, se ha realizado asi a posta para facilitar el ingreso de datos de forma manual, con mas entradas la eficacia del modelo puede llegar al 94%,
pero no es viable que alguien que quiera probar la demo de Gradio o la API ingrese cientos de datos.

Para realizar este proyecto se ha utilizado Numpy, Pandas, Seaborn, Matplotlib, Keras, Tensorflow, Scikit-learn y Gradio

Los pasos a seguir han sido:
- Descargar el dataset, balancear los datos igualando a la baja las ocurrencias de la columna a predecir.
- Utilizar la matriz de correlacion para saber que columnas tienen valor a la hora de predecir el valor deseado y eliminar las que no sean utiles.
- Sustituir los valores nulos de las columnas elegidas.
- Normalizar y dividir el dataset en conjuntos de entrenamiento y test.
- Generar un reporte de modelo que permita ver de forma sencilla su eficacia.
- En base a las entradas a la red neuronal, crear una red neuronal con Keras que procese los datos y de un valor predecido en forma de 0 o 1.
- Tras ello, con Gradio se forma una API y una pequeña demo que permite el uso del modelo a cualquier persona interesada sin falta de ningun conocimiento tecnico.
