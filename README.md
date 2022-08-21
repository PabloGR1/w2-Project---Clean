# w2-Project---Clean
Repo proyecto W2. Limpieza y presentación

## Introduction

Iniciamos el proyecto con un fichero en crudo que contiene mas de 25.000 filas, y tenemos que depurar. 


## Proceso

Durante el proceso de limpieza, lo primero que hemos hecho ha sido navegar sobre las distintas columnas para informarnos bien sobre la tematica, para poder tomar las mejores decisiones a la hora de limpiar los datos

Lo primero que observamos es que contiene muchas filas en blanco al final del libro, las cuales procedemos a quitar ya que no aportan información.

Tenemos una columna Date, donde nos muestra información de la fecha en la que se registra el ataque. De esta columna solo nos interesa saber el mes que se produjo el ataque, puesto que nuestro analisis no va a profundizar tanto hasta el detalle de dia.

En la columna Year, limpiamos los datos hasta obtener los años de manera limpia

Observamos que el 60% de los ataques, se producen en 3 grandes paises, por lo que nos quedamos con estos 3 (Usa, Australia y Shouta Africa)

Para homogenizar valores hemos utilizado tecnicas como lower, para tener todo el texto en minusculas, y poder hacer remplace.

Hemos quitado duplicados utilizando el drop.duplicate.

Para homogenizar columnas como Activity, Species... no he sido capaz de sacar un patron regex, a si que he tenido que hacer un codigo feo, que mediante un bucle for, e infinitos ifs (sorry), fuese homogenizando las columnas.


## Presentación

Para realizar la presentación, me he basado en lo que mas conozco, que es el excel y el power bi. Una vez que ya tenia la data limpia, he exportado un CSV y lo he trabajado por fuera de python.

Los graficos estan hechos en Power BI

La presentación se ha realizado con un template de power point descargada de internet sobre la tematica Sharks.

La presentación, la podria ampliar aun mas, mostrando por ejemplo los ataques que se producen por estacionalidad del año y por pais. Probablemente no se produzcan los mismos ataques en Junio en USA, que en Australia...
Mostrando un desglose de mortalidad por pais, incluso segregando el genero...


## Conclusión

La conclusión final es que pese a que finalmente he sido capaz de realizar una limpieza de base de datos, me he visto muy verde (entiendo que es normal, es la primera...)
He necesitado apoyo del excel, para ir visualizando los datos por fuera, para poder determinar cual serian los siguientes pasos. En python no soy capaz de ver la información de una manera que me ayude a visualmente saber lo proximo que quiero hacer
Tambien me he frustrado con regex, por que no he sido capaz de hacer un patron que me simplificase el codigo.

Supongo que con el tiempo iremos cogiendo practica.

Si que me gustaria recibir un feedback, y algun consejo de como optimizar un poco el codigo.Seguro que se puede no utilizar tantos if y ors (sin llegar a Regex), un punto intermedio.
