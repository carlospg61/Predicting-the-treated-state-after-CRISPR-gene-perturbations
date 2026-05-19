# Predicting the treated state after CRISPR gene perturbations
En este repositorio tengo el trabajo final de la asignatura Deep Learning del Master en Ciencia de datos de la UNAV. Contiene el desarrollo y los resultados del Trabajo Final orientado a predecir el estado celular y los perfiles de expresión tras perturbaciones genéticas mediante CRISPR. Utilizando arquitecturas avanzadas de Deep Learning (incluyendo modelos de difusión y procesamiento de datos latentes), el proyecto aborda el desafío de modelar sistemáticamente las respuestas celulares a nivel genómico. El pipeline abarca desde el procesamiento de índices genéticos y escalado latente hasta el entrenamiento de modelos generativos capaces de inferir con precisión los efectos fenotípicos de la edición genética.

En los 4 PDFs están los colabs que he utilizado para realizar el trabajo. 

En el primero tenemos la realización del primer Task. En el que hago un Ridge con las 3 líneas celulares y los 2 tipos de splits y hago un modelo de difusión en espacio latente (encoder -> diff - > decoder) para predecir el estado treated solamente en la linea celular PC3. 

En el segundo PDF (2.0) junto las 3 líneas celulares en un dataset y entreno el modelo con este dataset (usando el tipo de Split unseen interventios) y evaluó sus resultados.

En el tercero (2.1) hago exactamente lo mismo que en el anterior pero usando el tipo de Split random ( Tambien guardo los modelos porque estos seran los que use para el punto extra) 

En el ultimo pdf encontramos el codigo para el Cross-cell-line , en el que entreno el modelo que he relaizado con las 2 primeras lienas celulares y como test utilizo toda la linea celualr PC3 . Para esto uso el split unseen interventios, para poner a prueba lo maximo posible si el modelo entiende la biologia real.

Por ultimo en la carpeta punto extra se encuentra un colab con la funcion solicitada para realizar las predicciones de la linea celular nueva. Tambien esta dentro la carpeta de recursos con todos los documentos necesarios para hacer las predicciones (pesos de los modelos , variables necesarias , escaladores ...) 
