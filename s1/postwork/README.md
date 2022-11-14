# Postwork Sesión 1.

#### Objetivo

"El Postwork tiene como objetivo que practiques los comandos básicos aprendidos 
durante la sesión, de tal modo que sirvan para reafirmar el conocimiento. Recuerda 
que la programación es como un deporte en el que se debe practicar, habrá caídas, 
pero lo importante es levantarse y seguir adelante. Éxito"

# Desarrollo

"El siguiente postwork, te servirá para ir desarrollando habilidades como si se 
tratara de un proyecto que evidencie el progreso del aprendizaje durante el módulo, 
sesión a sesión se irá desarrollando.
A continuación aparecen una serie de objetivos que deberás cumplir, es un ejemplo 
real de aplicación y tiene que ver con datos referentes a equipos de la liga española 
de fútbol (recuerda que los datos provienen siempre de diversas naturalezas), en 
este caso se cuenta con muchos datos que se pueden aprovechar, explotarlos y generar 
análisis interesantes que se pueden aplicar a otras áreas. Siendo así damos paso a las instrucciones:" 

# 1. Del siguiente enlace, descarga los datos de soccer de la temporada 2019/2020 de la primera división de la liga española: 
https://www.football-data.co.uk/spainm.php

# 2. Importa los datos a R como un Dataframe. NOTA: No olvides cambiar tu dirección de trabajo a la ruta donde descargaste tu archivo

setwd("~/R Fase 2/9-nov-22")
sp1 <- read.csv("SP1.csv")
View(sp1)
