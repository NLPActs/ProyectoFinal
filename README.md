# PROYECTO FINAL

# Tecnologías de información emergentes: NLP

## Modelos multimodales

#### _Clasificadores multi-clase multimodales_
---
#### Link Google Colab:

https://colab.research.google.com/drive/1gUFre0aOY0Zyfm2ADFRlKQ4s5q2OVpQa?usp=sharing

---

## Funcionalidades

* Analisis de sentimientos (Negativo/Neutro/Positivo) sobre
    * Reviews y datos tabulares de aplicaciones de la PlayStore usando Multimodal Transformers

* Extra
    * Modelo clasficador multi-clase multimodal (5 clases) usando AutoGluon
    * Recolector y etiquetador de reviews de la playstore
---

## Ejecución

Este código esta pensado para ejecutarse desde una instancia de google colab asi que el primer paso es realizar una copia del colab cuyo link se encuentra hasta arriba de este documento. Además, primero lee el archivo Requirement.txt ubicado en este mismo repositorio.

El único archivo usado se encuentran en este mismo repositorio. Las bases de datos se pueden generar conforme la ejecución del notebook (colab). Este archivo se pide subir al inicio de la ejecución del notebook, por lo que no es necesario subirlo de antemano al directorio raíz.


Relativo a la ejecución, el primer modelo generado recibe como entrada una oración como cadena de texto (string) u oraciones como en una lista de cadenas de texto (string), así como datos tabulares (Género, Precio, Contenido de anuncios, Número de reviews, entre otros datos que pueden ser revisados en el enlace colab). Mientras que, el segundo modelo recibe adicionalmente imágenes por cada nueva entrada a predecir, así como otros datos tabulares distintos a los del primero modelo, tales como: tipo de mascota (gato o perro), edad, raza, sexo, color, vacunas recibidas, la salud, el precio o donación por adopción, entre otros datos administrativos.

---

## Bases de datos usadas

Google Play Store Apps: <br>
https://www.kaggle.com/gauthamp10/google-playstore-apps

Competición PetFinder: <br>
https://www.kaggle.com/c/petfinder-adoption-prediction/data

Reviews y metadatos (datos tabulares) de playstore: <br>
Estas fueron recolectadas mediante la API "google-play-scraper". Esta utiliza las IDs de las aplicaciones para la recolección de los datos encontrados en la playstore. Las IDs se recolectaron usando la primera base de datos de Kaggle adjunta. En total, se usaron 100 IDs de distintas aplicaciones. En este caso, se recolectaron alrededor de 6k reviews. Asimismo, las 5 categorías (estrellas) fueron englobadas en 3 categorías o sentimientos: negativo, neutro, y positivo. Para lo cual, aquellas con 1 o 2 estrellas se les atribuyó una connotación negativa. Para las de 3, una neutra. Por último, las de 4 y 5 una positiva. Cabe remarcar que, las clases no presentaban desbalance significativo. No obstante, se realizó "downsampling" para tener un balance ideal.

---

## Autores 📝

_Equipo #3:_

* **Carlos Adrián Guerra Vázquez**
* **Omar Osvaldo Hernández Díaz**
* **Jesús Carlos Martínez González**
* **Luis Miguel Maawad Hinojosa**
* **Juan Edgar Juarez Mendoza**
