# TP_Bioinformatica

### ¿Podrías buscar un ejemplo de macromoléculas que almacenen información sobre la 'identidad' de un organismo dado?

Las macromoleculas que albergan información de un organismo son: el ADN y el RNA
## Proponé una forma de expresar la información contenida en la estructura primaria de las proteínas usando tipos de datos de los lenguajes de programación que conocés. 

Al tener que representar una cadena de veinte aminoácidos, se podría representar de muchas maneras. En mi caso usaría un String siendo cada character un residuo diferete.
### ¿En qué tipo de datos prodrías expresar la información de la esctructura terciaria proteica?

Manteniendo la lógica del ejercicio anterior, tendría que implementar un Array de Arrays. Donde cada elemento es un residuo diferente, Ahora ese elemento es otra lista donde la primer posición es el aminoácido per se y los siguientes representan, con la misma lógica matemática el eje x, eje y y eje z. Por ejemplo: [[A, 12, 45, 59] , [B, 12, 34, 50]]
### Rosalind Franklin es una científica muy relevante, que tuvo menos reconocímiento del merecido. ¿Cuáles fueron sus contribuciones en este campo? ¿Qué nos cuenta su historia acerca del mundo de la ciencia?

Fue una investigadora en el campo de los rayos x, siendo su investigación la que deriva en poder sacar la primer fotografia de la estructura de doble hélice del ADN. Ademas de esto, según el articulo. Ella había llegado a la misma conclusión sobre el ADN que los que publicaron la investigación, pero estos cientificos fueron mas rápidos.
### Proponé en pseudocódigo un programa que prediga la estructura secundaria que adoptará cada residuo de la secuencia proteica dada, especificandola como H(si es una hélice), B(Si es una hoja beta plegada) y L(Si es un bucle o loop).
```
public function posicionDe(Char aminoacido){
  if(aminoacido.tieneTendenciaEnH()){ return 'H'}
    else if(aminoacido.tieneTendenciaEnB()){ return 'B'}
      else return 'L';
}
public function prediccion_proteina(List[String] cadenaDeAminoacidos){
  List[String] estructuraSecundaria = new List();
    cadenaDeAminoacidos.forEach(unAminoacido -> estructuraSecundaria.add(posicionDe(unAminoacido));
      return estructuraSecundaria;
}
```
### ¿Qué hace distintos a dos individuos de una especie? Propone una forma de corrobarar tu respuesta realizando un diagrama de un posible método computacional para dicho fin.

La diferencia es el ADN, tanto su longitud como su composición, ya que al ser diferente la estructura primaria, los aminoácidos sintetizados van a ser diferentes. Por otro lado, si tienen la misma estructura primara pero la longitud es diferente
uno va a producir mas codones que el otro.
Un programa que resuelva esta duda podría tener una función que reciba dos cadenas primarias de individuos de una misma especie y retorna si son distintos o iguales
```
public function sonCadenasIguales(String[] cadena_primaria_a, String[] cadena_primaria b){
  var proteinas_individuo_a = proteinasSintetizadasEn(cadenaPrimaria_a);
  var proteinas_individuo_b = proteinasSintetizadasEn(cadenaPrimaria_b);
  
    return proteinas_individuo_a === proteinas_individuo_b;
```

