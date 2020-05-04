# TP_Bioinformatica


### ¿Por qué una celula querría destruir sus propias proteínas?  

Como las proteínas cumplen muchas funciones en la célula, estas entren en acción en determinaod momentos, realizan su función y le dejan de resultar importante a la celula. Es decir mantener una proteína en la celula que ya no le es util es acumular basura. Para ello la ubiquitina la marca para que luego sea destruida. 


### ¿Qué información nos provee esta página?

Esta página tiene mucha información sobre no solo la proteina per se, sino también sobre el experimento que se realizó para fotografiarla. 
Datos que se brinda:
-Nombre de la protína (UBIQUITIN).
-Tamaño de resolución (1.8 ANGSTROMS).
-Año y autores del experimento (1987-04-16  // Vijay-Kumar, S., Bugg, C.E., Cook, W.J.).
ademas de esto, los nombres son links a otros experimentos realizados por los mismos cientificos.
-Organismo del cual se extrajo para la fotografia (Homo sapiens).
-Una visualización en 3D sobre la estructura terciaria de la proteína.

### ¿Cómo se determinó la estructura de esta proteína?

Aplicando la investigación de Rosalind Franklin, se extrae de su ambiente original ya que recide en agua. Viendo con rayos X en donde hay lugares vacíos y lugares llenos, pudiendo así generar una representación mas exacta posible.

### ¿Qué significan las cintas, las flechas y las regiones angostas?

Esas regiones representan las diferentes estructuras secundarias que adopta esa proteina, al ver en detalle la representación especifica cual es el aminoácido que tiene esa forma en particular. 
Por ejemplo el aminoácido numero 45, la Fenilalanina esta en forma de alfa hélice.


### ¿Representa esta ímagen la realidad del sistema biológico?

No, no la representa. Como fue explicado en la pregunta de como se determina la estructura, para generar esta ímagen es necesesario separar a la proteina de donde esta está, por ende al encontrarla en un organismo no va a tener la misma forma.
Es decir su forma natural esta en constante moviento, cosa que impediría fotografiarla con certeza.  


### ¿Cuál es la utilidad y los condicionamientos de usar un modelo científico que sabemos inexacto?

Tiene muchos casos de uso tener un modelo inexacto, primero que nada ayuda a llevar algo imposible de visualizar con un ojo humano a una representación 3D, la cual podemos cambiar su estructura ver que aminoácidos la forman, etc. Por otra parte ayuda a la ciencia a 'simplificarse' ya que al poder ver esto, personas como los estudiantes de programación que no tenemos conocimientos de biologia, podemos llegar a entener que estamos viendo. 
Ahora hay que tener en cuenta que lo que vemos no es realmente lo que es, no tomar esa imagen 'con pinzas' ya que en la realidad no es como esta esa proteina y podría llegar a reaccionar de una forma inesperada si solamente nos basamos en las fotografias tomadas.

### ¿Qué diferencias y similitudes notamos respecto de la representación inicial?

La primera diferencia es que se abre un visualizador, donde moviendo el cursor podremos recorrer la proteína. No solo eso sino que esta detalla la estructura primaria y tenemos la posibilidad de cambiar la representación actual para ver cuales son las distintas formas que esta toma. 

### ¿Para qué podría ser útil visualizar lo mismo de distintas maneras? 

Cada tipo de representación nos brinda información diferente sobre la proteína, ver la estructura terciaria, nos sirve para ver en que regiones hay que tipo de estructura. Por otra parte ver los 'huecos' que tiene la misma es util para investigar sobre como se podría utilizar esa proteína en la producción de farmacos, es decir como utilizar esta misma para 'unirla' con otras.

### ¿Qué información esperaría encontrar como resultado un experimento destinado a determinar la estructura terciaria de una molécula biológica?

Esperaria tener las coordenadas de cada aminoácido, para saber su disposición espacial.

### ¿En que consiste un archivo PDB?

Consiste en toda la información sobre como fue realizado el experimento, quienes fueron los autores, un cuadro explayando información especifica sobre cada atomo que forma cada aminoácido que pertenece a la cadena primaria. 

### ¿Que tipo de información brinda esta sección? (ATOM)

Brinda la información de un atomo en especifico, por ejemplo nitrogeno. a Que amionoácido pertence, la posición de ese atomo en la cadena primaria(de 1 a la longitud de la cadena), luego hay tres columnas representando los ejes cartesiano (x, y z) representando en donde estaba ese atomo cuando se realizo el experimento.

### ¿Podríamos extraer de este archivo información sobre la estructura primaria de la proteína en cuestión? ¿Cómo se presenta dicha información y qué significa la representación? ¿De que tipo de dato se trata esta información?
Si, PDB te brinda al lado de cada atomo un numero, ese numero es la posición de la cadena primaria. Habria que parsear todos los atomos de todas las posiciones y sabriamos como esta conformada dicha estructura.
Viendo que las columnas tienen información breve (una sola letra para representar el tipo de atomo, tres numeros para los ejes), podriamos tener una lista de listas con la misma logica de las columnas de PDB. Pero en mi caso eligiria que cada fila sea un objeto para que sea mas facil trabajar con ellos. Ambas soluciones me parecen igual de funcionales. 

###¿Considera que el formato de PDB es útil para presentar los resultados del experimento?

Siendo una persona que no tiene contacto con la ciencia, me parece que el formato no es amigable pero cumple con la información que uno/a busca sobre una proteina, es nada mas aprender a leer el formato.

###¿Cuáles son los beneficios y las limitaciones de imponer una estructura para comunicar los resultados de un experimento?

Los beneficios es poder tener definido un protocolo, todos los archivos de PDB van a tener ese formato y simplifica el poder trabajar con el mismo. Poder parsear las partes o crear programas sobre un archivo PDB, nos va a servir para todos los que estén en la base de datos. Ahora del lado mas humano, al principío va a ser muy dificultoso leer, sin casi entender lo que estamos viendo, a menos que alguien nos explique o leer la documentación. Algo que me parece recurrente en la ciencia que nunca prioriza lo visual ya que al estar hablando entre biologos se espera un minimo nivel de conocimiento. Alejando así a personas ajenas a estos protocolos. 
