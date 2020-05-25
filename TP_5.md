# TP_Bioinformatica

## Pensar los pasos a seguir en un alineamiento de dos secuencias cortas
 
Lo primero que habría que hacer al momento de alinearlas es saber cual es el mejor camino posible que tenemos frente a estas cadenas,
para eso necesitamos utilizar el algoritmo de Needleman-Wunsch. Dependiendo de lo que estemos buscando o investigando, le pondremos
los valores de MissMatch, Match y gap. Una vez que obtenido estos valores comenzamos a contar posición por posición cual es son
los valores de las mismas. Una vez que toda la matriz esta completada, aplicamos el algoritmo buscando el camino con el mas alto valor
(este valor depende de los valores iniciales que elegimos para el MM, M y gaps). Una vez tenido ese camino ya sabremos cual es la forma
optima de alinear esa cadena, esta forma no es única sino que es la que mejor se adecua a nuestros valores, podría tener otro tipo de busqueda,
que me de otra cadena diferente.

## probá distintos Gap penalties para el ejemplo propuesto y observá lo que ocurre.

Primero fuí bajando de a poco el valor de gap ( de uno en uno) y me di cuenta que no cambiaba la solución, hasta que cambie de negativo (originilmente -2) 
a un valor positivo (gap = 1) y la solución fue una cadena totalmente diferente, viendo esto llego a la conclusión de que dependiendo de esos valores, la solución puede 
ser radicalmente diferente y hay que estar seguro de que esta buscando para no tener un resultado que no le sirve. 

## calculá el E-value y % identidad utilizando el programa Blast de la siguiente secuencia input usando 20000 hits, un e-value de
100 y tomando aquellos hits con un mínimo de 70% cobertura. Observe y discuta el comportamiento de : E-value vs. % id, Score vs %
id, Score vs E-value

Parece que estos tres valores estan altamente relacionados, ya que cuando varia uno varian también los otros dos. El e-value es nuestro
valor de referencia para saber que tan certero es esa proteina en esa cadena, cuando menor sea el valor mas confianza nos transmite.
Cuando corrí en blast la proteina que tiene el menor e-value también tiene el mayor score y porcentaje de identidad, es decir que era la misma
proteína. De igual forma, hay varias secuencias que disminuye el e-value pero el porcentaje de identidad sigue siendo 100%, viendo esto
entre el score para desempatar y así podemos ver cual es la proteina que comparada con toda esta base de datos es la mas cercana o directamente es la misma

##  Realizá nuevas búsquedas usando la mitad de la
secuencia problema y para un cuarto de la secuencia original. Compará
los gráficos obtenidos.¿Qué conclusiones puede sacas?
