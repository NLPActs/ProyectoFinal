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
    * Reviews y datos tabulares de aplicaciones de la PlayStore usando

* Extra
    * Modelo clasficador multi-clase multimodal (5 clases) usando AutoGluon
    * Recolector y etiquetador de reviews de la playstore
---

## Ejecución

Este código esta pensado para ejecutarse desde una instancia de google colab asi que el primer paso es realizar una copia del colab cuyo link se encuentra hasta arriba de este documento. Además, primero lee el archivo Requirement.txt ubicado en este mismo repositorio.

Algunos archivos y bases de datos usados se encuentran en este mismo repositorio.

Estos archivos han de colocarse en el mismo directorio en el que este su archivo .ipynb.

Además, se han de decargar y extraer las tablas de las bases de datos utilizadas y cuyos links puede encontrar más abajo en este documento.

Idealmente estos son los archivos que tienes que tener en tu directorio raiz: <br>
![alt text](https://github.com/NLPActs/NLP_ActInt3/blob/main/Screenshot%202021-11-01%20013644.png)


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
