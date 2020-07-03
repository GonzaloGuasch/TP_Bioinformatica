# TP_Bioinformatica


## RETO I: Detalla las tácticas y/o metodologías que deberían utilizarse para darles una respuesta a los padres del niño.

Lo primero que habría que hacer es saber que predominancia tiene este humano-mosca, si es mas mosca que humano o vice versa. Para ello necesitamos comparar las secuencias de humano, mosca y humano-mosca. Pero antes que hacer eso es necesario que estén alineadas todas las secuencias, para ello utilizaremos la herramienta de CLUSTAL para alinear las mismas, una vez hecho esto llevamos las secuencias alineadas a otro programa IQTREE para saber el arbol de esta nueva criatura. Podríamos parar ahí y mostrarle a los padres este nuevo arbol con tres muestras nada mas e inferir que si esta del lado del humano/mosca es de donde tiene predominancia pero este resultado no seria tan preciso como para calmar a una pareja de padres enfurecidos con la ciencia. Para ampliar el resultado y que sea de mayor calidad es necesario agregar mas secuencias a al arbol, siguendo paso a paso las acciones que tuvimos que hacer para todas las secuencias (Alinearlas -> llevarlas al IQTREE junto al resto)

## RETO II: Como vimos anteriormente existen algunos softwares optimizados para confeccionar alineamientos de secuencias. En particular hemos trabajado con Clustal (Larkin et al. 2007). Confecciona los alineamientos para los del punto Ia y Ib análisis.

![](https://github.com/GonzaloGuasch/TP_Bioinformatica/blob/master/bart%20vs%20mosca%20vs%20hombre.png?raw=true)

![](https://github.com/GonzaloGuasch/TP_Bioinformatica/blob/master/arbolBartHumanoMosca.png)


Como se puede ver cuando alineamos las tres secuencias nada mas no tenemos mucha información que nos sea relevante. Pero si agregamos muchas secuencias el OUTPUT cambia radicalmente

![](https://github.com/GonzaloGuasch/TP_Bioinformatica/blob/master/bartVsTodos.png)
![](https://github.com/GonzaloGuasch/TP_Bioinformatica/blob/master/arbolBartYSecuencias.png)

Viendo esto sabemos que ahora el bart mosca es mas bart que mosta pero sigue estando altamente relacionado. 


## RETO III
## Como vemos, el servidor nos permite elegir el modelo de sustitución ¿A qué serefiere?
El IQtree ofrece una basta variedad de modelos, entre ellas la Blosum62. Eligiendo así cual es la matrix de sustitución que queremos para nuestros aliniamientos.

## ¿Qué es el Bootstrap? ¿De qué manera nos habla de la calidad de nuestro árbol? ¿Cómo influye el número de Bootstraps en el resultado?

## ¿Es necesario realizar algún paso extra, previo a la interpretación del árbol? ¿Por qué?
Si, primero hay que abrir el archivo del arbol en el programa. Una vez hecho esto, es necesario rutear el arbol, selecionando la rama con las secuencias mas alejadas y elegír la opción "Reroot" para poder realizar el analisis de forma correcta. 
