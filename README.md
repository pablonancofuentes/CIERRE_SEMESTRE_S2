# CIERRE_SEMESTRE_S2


**Ejercicio Cierre de Semestre Big Data Secci�n 2**

Desarrollo.

1.- "Construya un script en R, que cuente la cantidad de elementos "positivo", "negativo" y "neutros"."

Antes de contar la cantidad de elementos es necesario crear las 100 variables aleatorias con el comando: "ejemplos = sample(c("positivo","negativo","neutro"),100, replace = TRUE)"

Teniendo las 100 V.A es posible contar los elementos con el comando: "table(ejemplos)"

Los resultados obtenidos son: 

**positivo:28, negativo:39, neutro:33.**


2.- "Experimente ejecutando el set.seed(10), previo a la creaci�n de elementos aleatorios, sin ejecutarlo antes y comente, c�mo impact� la implementaci�n del set.seed(10) en los resultados."

Al ejecutar el comando "set.seed(10), este solo fija una cantidad especifica de valores del siguiente comando "ejemplos = sample(c("positivo", "negativo", "neutros"), 10, replace = TRUE)".

Elementos fijados son:

**negativo:2, neutro:7, positivo:1**

En cambio si se ejecuta el comando "ejemplos = sample(c("positivo", "negativo", "neutros"), 10, replace = TRUE)" sin fijar se obtienen elementos aleatorios.

Por ejemplo:

**negativo:4, neutro:1, positivo:1**


3.- "Asuma que los valores "positivo", "negativo" y "neutros" generados a partir de
set.seed(66), corresponde a los resultados recolectados de todas las noticias que hablan
sobre una crisis econ�mica, �qu� impacto tendr�a si se consideran o no los neutros?"

Al realizar nuevamente los pasos anteriores pero esta vez con 66 elementos a partir de la recoleccion de una noticia sobre la crisis econ�mica

El comando a utilizar es el siguiente: "ejemplos = sample(c("positivo", "negativo", "neutros"), 66, replace = TRUE)"

Sin utilizar "set.seed(66)":

**negativo:19, neutros:29, positivo:18**

Con "set.seed(66)":

**negativo:20, neutros:20, positivo:26**

Por lo tanto, se puede concluir que sin utilizar el comando "set.seed(66)" el numero de neutros corresponden al 43,93%, 
en cambio si se utiliza el comando "set.seed(66) los elementos neutros ser�a el 30,3%, existiendo una diferencia de 13,63%.
Por lo que la omisi�n de este comando influenciar�a las noticias negativas sobre las positivas, en caso contrario, las noticias
positivas sobrepasar�a el numero en 6 noticias.


4.- "Construya un script capaz de calcular la probabilidad del conjunto de cartas que est� por salir,
para crear datos de prueba utilizando la funci�n sample considerando que han salido 31
cartas"

Se asume que el mazo contiene 52 cartas, y ya se han descartado 31 de ellas, queda un total de 21 cartas, se utiliza el comando sample
agrupando las cartas en altas, bajas y medianas. Con las siguientes probabilidades:

**altas: 9(37,5%), bajas: 2(25%), medianas: 9(37,5%)**
Obteniendo un total de: 0 puntos finales.


5.- "Si en el ejercicio anterior utilizamos la funci�n set.seed. �Qu� grupo de cartas tiene m�s
probabilidades de salir?"

Las probabilidades de salir cada grupo de cartas al aplicar el comando set.seed(21) son:

**altas: 4(19,05%), bajas: 10(47,62%), medianas: 7(33,33%).**

Por lo que el grupo de cartas que tiene mas probabilidades de salir son las bajas con un 47,62%.







4.-