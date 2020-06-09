# TP_Bioinformatica

Completando el cuadro del PDF con los nombres cómunes:
 a) gallus gallus = Gallo
 b) Pan troglodytes = Chimpanzee
 c) Equus caballus = Caballo
 d) Canis lupus familiaris = Perro
 e) Gorilla gorilla = Gorila occidental
 f) Oncorhynchus tshawytscha = Salmón
 g) Xenopus laevis = Rana
 h) Drosophila melanogaster = Mosca
 
# ¿Cuán sencillo será alinear dos o más secuendias a mano?¿Cuánto influira el numero de secuencias a alinear, su longitud, y la similutud entre ellas?

 Viendo como clustal alinea las secuencias me parace bastante dificil realizarlo a mano, ya que hay que ver residuo por residuo si son iguales
 o ir agregando gaps para emparejar las secuencias. Ademas, pienso que a mayor numero de las mismas la dificultad crece exponencialmente al igual que la taza 
 de errores. 
 El orden de dificulta parece ir de la mano tanto de la longitud como de la similaridad de las secuencias, ya que no es lo mismo alinear una secuencia
 de dos mil residuos diferentes que una con tres que sean iguales. 
 
# ¿Son parecidos los citocromos c de humano y gallo?
No solo que son parecidas, sino que son excatamente iguales, aminoácido por aminoácido.
 
# ¿Que teorias subyacen a este análisis?
 Para poder llegar a la conclusión de que una cadena sea igual, parecida o no es necesario saber todas las posiciones de las dos cadenas, para esto no solo es necesario haber analizado ambas secuencias por separado para conocerlas sino que hay que alinear ambas para conocer en la posición N los residuos que hay en ambas. para saber cual es la alineación mas precisa hay que aplicar un algoritmo de alineación.
 
# ¿Cómo nos ayuda la evolución a explicar sus similitudes y diferencias?
Viendo que especies tan diferentes comparten una proteina con una cadena primaria tan similar, la teoria de que provenimos de un ancestro en común cobra un peso mucho mas importante y viendo las cadenas alineadas, no parace tan dificil de creer en ella.
Al mismo tiempo, la teoria de la evolución habla de un constante cambio y evolución, eso podria ser el emotivo por el cual algunas proteínas son un poco mas diferentes, ya que estas especias estuvieron enfretadas a diferentes ambientes y mutaciones.
 
# Podemos elegir verlo en colores (Show color). ¿Qué indican los colores?
Cada color representa un aminoácido diferente, esta representación ayuda a la vista para rapidamente darnos cuenta de las similutades/diferencias de las secuencias, por lo menos a un modo mas amplio. 

# ¿Qué indican el guión(-), los dos puntos(:) y el asterisco (*)?
El asterisco indica que en la posición n que esta todas las cadenas tienen los mismos residuos, el guion nos indica una inserción de un gap en la cadena y los dos puntos representan una buena conservación, siendo menos confiable que si fuera un '*'.
# ¿Se conserva la secuencia del citocromo c en los organismos?

Si, se conservan ya que el alineamiento se realiza en una muestra del citocromo c, no en el mismo organismo.

# ¿Creeríamos que todos los organismo se asemejan por igual al resto, o se pueden identificar grupos de mayor similitud? Si es así, ¿tienen sentid?¿Qué evidencias nos aportaría este análisis, a la luz de la evolución?¿Cuáles creeria que deberian estar más agrupados en el árbol filogenético?
 Hay organismo que se asemejan mas que otros ya que hay especies que se relacionan mas entre si, por ejemplo el humano tiene mas relación con un gorila que con una mosca. Sabiendo las bases de la teoria de la evolución, esta nos dice que partimos de un ancestro común que en algun punto de la historia nos empezamos a diferenciar creand dos tipos de especies que hoy son diferentes pero seguimos compartiendo muchas caracteristicas a nivel de código genetico 

# Observando el árbol filogénetico ¿Concuerda con lo esperado?¿De qué organismos son los citocromos c mas parecidos?¿Cómo se exploca?

Según el árbol filogénetico la especie menos relacionada es la mosca, después relaciona el salmón con la rana. Cosa que parece lógico porque son los únicos animales de la lista que tienen tanto contacto con el agua. 
Eso en una "rama" del árbol y en la otra mas alejada se relaciona el hombre muy cercano con el Chimpance y a la vez con los gorilas.
Me parece un resultado mas que esperado, ya que son especies que parecieran tener relación hace miles de años. 
