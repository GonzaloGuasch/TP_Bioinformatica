# TP_Bioinformatica

### ¿Podrías buscar un ejemplo de macromoléculas que almacenen información sobre la 'identidad' de un organismo dado?

Las macromoleculas que albergan información de un organismo son: el ADN y el RNA
## Proponé una forma de expresar la información contenida en la estructura primaria de las proteínas usando tipos de datos de los lenguajes de programación que conocés. 

Al tener que representar una cadena de veinte aminoácidos, se podría representar de muchas maneras. En mi caso usaría un String siendo cada character un residuo diferete.
### ¿En qué tipo de datos prodrías expresar la información de la esctructura terciaria proteica?

Manteniendo la lógica del ejercicio anterior, tendría que implementar un Array de Arrays. Donde cada elemento es un residuo diferente, Ahora ese elemento es otra lista donde la primer posición es el aminoácido per se y los siguientes representan, con la misma lógica matemática el eje x, eje y y eje z. Por ejemplo: [[A, 12, 45, 59] , [B, 12, 34, 50]]
### Rosalind Franklin es una científica muy relevante, que tuvo menos reconocímiento del merecido. ¿Cuáles fueron sus contribuciones en este campo? ¿Qué nos cuenta su historia acerca del mundo de la ciencia?


### Proponé en pseudocódigo un programa que prediga la estructura secundaria que adoptará cada residuo de la secuencia proteica dada, especificandola como H(si es una hélice), B(Si es una hoja beta plegada) y L(Si es un bucle o loop).


### ¿Qué hace distintos a dos individuos de una especie? Propone una forma de corrobarar tu respuesta realizando un diagrama de un posible método computacional para dicho fin.
