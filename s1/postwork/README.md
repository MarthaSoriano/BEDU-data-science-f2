# Postwork Sesión 1.

#### Objetivo

"El Postwork tiene como objetivo que practiques los comandos básicos aprendidos 
durante la sesión, de tal modo que sirvan para reafirmar el conocimiento. Recuerda 
que la programación es como un deporte en el que se debe practicar, habrá caídas, 
pero lo importante es levantarse y seguir adelante. Éxito"

## Desarrollo

"El siguiente postwork, te servirá para ir desarrollando habilidades como si se 
tratara de un proyecto que evidencie el progreso del aprendizaje durante el módulo, 
sesión a sesión se irá desarrollando.
A continuación aparecen una serie de objetivos que deberás cumplir, es un ejemplo 
real de aplicación y tiene que ver con datos referentes a equipos de la liga española 
de fútbol (recuerda que los datos provienen siempre de diversas naturalezas), en 
este caso se cuenta con muchos datos que se pueden aprovechar, explotarlos y generar 
análisis interesantes que se pueden aplicar a otras áreas. Siendo así damos paso a las instrucciones:" 

## 1. Del siguiente enlace, descarga los datos de soccer de la temporada 2019/2020 de la primera división de la liga española: 
https://www.football-data.co.uk/spainm.php

## 2. Importa los datos a R como un Dataframe. NOTA: No olvides cambiar tu dirección de trabajo a la ruta donde descargaste tu archivo

[Archivo CSV de datos](https://github.com/MarthaSoriano/BEDU-data-science-f2/main/SP1.csv)

```
setwd("~/R Fase 2/9-nov-22")
sp1 <- read.csv("SP1.csv")
View(sp1)
```
[-> Ver descripción de datos](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/notes.txt)
[-> Ver descripción de datos](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/dat/notes.txt)

![csv cargado](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/loaded_csv.png)
![csv cargado](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/img/loaded_csv.png)

## 3. Del dataframe que resulta de importar los datos a `R`, extrae las columnas que contienen los números de goles anotados por los equipos que jugaron en casa (FTHG) y los goles anotados por los equipos que jugaron como visitante (FTAG); guárdalos en vectores separados
```
(goles.locales <- c(sp1$FTHG))
(goles.visitantes <- c(sp1$FTAG))

```
![vectores](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/vectors_FTAG_FTHG.png)
![vectores](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/img/vectors_FTAG_FTHG.png)
## 4. Consulta cómo funciona la función `table` en `R`. Para ello, puedes ingresar los comandos `help("table")` o `?table` para leer la documentación.
```
help("table")
@@ -33,7 +33,7 @@ help("table")
```
table(vector.FTHG,vector.FTAG, dnn=list("FTHG","FTAG"))
```
![tabla](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/result_table.png)
![tabla](https://github.com/adavals/bedu-datascience-f2/blob/main/s1/postwork/img/result_table.png)

### a) ¿Cuántos goles tuvo el partido con mayor empate?
     R. 4 goles  
###  b) ¿En cuántos partidos ambos equipos empataron 0 a 0?
     R. 33 partidos
###  c) ¿En cuántos partidos el equipo local (HG) tuvo la mayor goleada sin dejar que el equipo visitante (AG) metiera un solo gol?
     R. 1 partido   (local:6 - visitante: 0)
