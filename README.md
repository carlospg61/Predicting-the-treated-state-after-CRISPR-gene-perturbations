# Predicting the treated state after CRISPR gene perturbations

This repository contains the final project for the Deep Learning course in the Master's Degree in Data Science at the University of Navarra (UNAV). It includes the development and results of the final project, which aims to predict cellular states and expression profiles following CRISPR gene perturbations. Utilizing advanced Deep Learning architectures—including diffusion models and latent data processing—this project tackles the challenge of systematically modeling cellular responses at the genomic level. The pipeline ranges from genetic index processing and latent scaling to training generative models capable of accurately inferring the phenotypic effects of gene editing.

The four attached PDFs correspond to the Google Colab notebooks used throughout this project:

* **First PDF (Task 1):** Implements a Ridge regression baseline across all 3 cell lines and both split types. Additionally, it features a latent space diffusion model (encoder → diffusion → decoder) developed to predict the treated state specifically for the PC3 cell line.
* **Second PDF (Task 2.0):** Combines the 3 cell lines into a single dataset to train the model using the "unseen interventions" split type, followed by an evaluation of its performance.
* **Third PDF (Task 2.1):** Follows the exact same pipeline as the previous task but utilizes a "random" split type. The models from this notebook are saved, as they are later required for the extra credit section.
* **Fourth PDF (Cross-cell-line):** Contains the code for cross-cell-line generalization. The model is trained on the first 2 cell lines and tested entirely on the PC3 cell line using the "unseen interventions" split to rigorously test whether the model truly captures the underlying biology.

Lastly, the `punto_extra` folder contains a Colab notebook with the requested function to generate predictions for a new cell line. This folder also includes a resource subfolder with all the necessary assets to run these predictions (model weights, required variables, scalers, etc.).


---------------------------------------------------------------------------------------------------------------------------------------------------------------------

En este repositorio tengo el trabajo final de la asignatura Deep Learning del Master en Ciencia de datos de la UNAV. Contiene el desarrollo y los resultados del Trabajo Final orientado a predecir el estado celular y los perfiles de expresión tras perturbaciones genéticas mediante CRISPR. Utilizando arquitecturas avanzadas de Deep Learning (incluyendo modelos de difusión y procesamiento de datos latentes), el proyecto aborda el desafío de modelar sistemáticamente las respuestas celulares a nivel genómico. El pipeline abarca desde el procesamiento de índices genéticos y escalado latente hasta el entrenamiento de modelos generativos capaces de inferir con precisión los efectos fenotípicos de la edición genética.

En los 4 PDFs están los colabs que he utilizado para realizar el trabajo. 

En el primero tenemos la realización del primer Task. En el que hago un Ridge con las 3 líneas celulares y los 2 tipos de splits y hago un modelo de difusión en espacio latente (encoder -> diff - > decoder) para predecir el estado treated solamente en la linea celular PC3. 

En el segundo PDF (2.0) junto las 3 líneas celulares en un dataset y entreno el modelo con este dataset (usando el tipo de Split unseen interventios) y evaluó sus resultados.

En el tercero (2.1) hago exactamente lo mismo que en el anterior pero usando el tipo de Split random ( Tambien guardo los modelos porque estos seran los que use para el punto extra) 

En el ultimo pdf encontramos el codigo para el Cross-cell-line , en el que entreno el modelo que he relaizado con las 2 primeras lienas celulares y como test utilizo toda la linea celualr PC3 . Para esto uso el split unseen interventios, para poner a prueba lo maximo posible si el modelo entiende la biologia real.

Por ultimo en la carpeta punto extra se encuentra un colab con la funcion solicitada para realizar las predicciones de la linea celular nueva. Tambien esta dentro la carpeta de recursos con todos los documentos necesarios para hacer las predicciones (pesos de los modelos , variables necesarias , escaladores ...) 
