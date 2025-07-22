Ejercicio 1 : Creamos una función que se llama frecuencia_letras y toma como argumento una cadena de texto. Dentro de la función definimos el diccionario_frecuencias que será lo que devuelva la función. Creamos el diccionario iterando en los caracteres que componen la cadena con el bucle for. Incluimos la condición de que salte los espacios en blanco. Luego con otra condición queremos hacemos que asocie el caracter i de la cadena (texto) con un número (el número de veces que aparece la letra en la cadena de texto). En la condición ponemos que si la letra ya ha aparecido sume uno, y si es la primera vez que sale que se le asocie el valor 1. 

Ejercicio 2: Definimos una función que se llama duplicar_lista y coge como argumento una lista. Después con la función map hacemos que coga los valores de la lista y los multiplique por dos, usando la sintaxis que tiene. Como resultado se devuelve una lista con los valores de la lista inicial dupicados.

Ejercicio 3: Definimos una función qeu tome como argumento una lista y una palabra. Creamos una lista vacía qeu se llama resultado y será lo que devuelva la función. Mediante un bucle for qeu recorre las palabras de la lista argumento, imponemos la condición de que si la palabra argumento está dentro de las distintas palabras de la lista, las añada a la lista resultado con la función resultado.append(). Cuadno termina el bucle devuelve la función resultado. 

Ejercicio 4: Definimos una función que tome como argumento dos listas, y devuelve una lista con la diferencia de ambas. Lo definimos con la función map usando lambda.

Ejercicio 5: Definimos una función que toma como argumentos una lista de números y la nota que por defecto es 5. Calculamos la media de los valores de la lista, y mediante una condición if else definimos si es aprobado o suspenso. Devolvemos en una tupla la media y la evaluación.

Ejercicio 6. Definimos una función que toma como argumento un número, n. Para que no nos dé error debido a la multiplicación por 0, hacemos que nos devuelva el valor 1 si n=0 o n=1. Para el resto de casos hacemos que nos devuelva el factorial de (n-1) multiplicado n veces.

Ejercicio 7. Definimos una funcion que toma como argumento una lista de tuplas, y queremos eliminar las tuplas y convertirlo a strings. Lo hacemos mediante la función map en dos veces. Primero definimos el parámetro lambda t con los elementos de la lista, es decir con cada tupla. Hacemos map(str, t) para convertir cada elemento de la tupla  atexto (por si son números). Después hacemos ''.join() que toma la lista de strings del paso anterior y los une con un espacio. Por esto, lambda t: ' '.join(map(str, t)) es una función que coge una tupla t, convierte cada elemento a string, y los une con espacios. Hacemos un map a toda esta función para que lo haga con cada tupla de la lista, y por último con un list() lo convertimos en lista. 

Ejercicio 8. Primero pedimos los inputs al usuario. Hacemos un bucle while qeu se repite hasta que se pueda dar un resultado válido (termina con break). Construimos el programa mediante try/except. Hacemos un try donde intentamos convertir los inputs a float y hacer la divisiómn. Si no puede, el programa da los errores que aparecen en except. El primero si el valor no es númerico  y el segundo si el denominador es 0. Si nohay error, directametne despues de hacer la división muestra el resultado y se termina el blucle. 

Ejercicio 9. Definimos una función que toma como argumento una lista que se llama mascotas con nombres de mascotas. Definimos la lista mascotas_prohibidas donde incluimos las mascotas prohibidas del enunciado. Usamos la función filter() con una función lambda que devuelve solo para las mascotas que no están en mascotas_prohibidas. Por último devolvemos una lista con dichas mascotas que cumplan la condición. 

Ejercicio 10. Definimos la función que tome como argumento una lista. Hacemos un try/except por si la lista está vacía, lo que sería un error tipo ValueError. Como condición imponemos que la longitud de la lista sea distinta de cero para que haga el promedio.

Ejercicio 11. Hacemos un bucle infinito con el while True que termina cuanod se introduce un número válido. Pedimos el input e imponemos  la condición dle rango de edad, si no se cumple lanzamos un ValueError. Si se cumple se imprime el número  y se termina el bucle. Si no es un valor numérico lanzamos otro ValueError y pedimos por pantalla q se introduzca un vaor numérico.

Ejercicio 12. La función toma como argumento una frase, es decir caracteres de texto. Con la función frase.split() separamos la frase por palabras. Con la función len cuenta la longitud de cada palabra y devuelve el resultado en una lista. 

Ejercicio 13. La función toma como argumento un conjunto de caracteres (que pueden ser letras o no). Lo primero que hcaemos es crear dos conjuntos vacíos, letras_vistas() que guarde las letras que ya han salido, y letras_ordenadas que es una lista vacía a la que le vamos a añadir las letras que irán apareciendo. Hacemos un bucle for que recorra los caracacteres que le hayamos introducido a la función. Para que solo lea los númericos hacemos isalpha() y con c.lower() not in letras_vistas no repetimos letras que hayan salido (filtrando por las minúsculas para q no cuente mayículas y minúsculas). Si la letra cumple ambas condiciones se anañen a letras_vistas y letras_ordenadas. Por último hacemos un map entre las letras mayúculas y minúculas que aparcen en letras_ordenadas, y devolvemos una lista de tuplas.

Ejercicio 14. La función coge como argumento una lista y una letra. Hacemos letra.lower() para que no distinga entre mayúcula y minúcula. Con palabra.lower().startswith(letra) se verifica si la palabra empieza o no con la letra, y con filter() hacemos q solo se conserven las palabras que cumplan esta condición. Por último se devuelv en forma de lista.

Ejercicio 15. La función con map hace que se aplique a cada elemtno de la lista, lambda x, y genera una nueva lista  ala que se le suman 3, x+3 . 

Ejercicio 16. La función toma como argumentos un s cadena de texto  y un número. Separamos la cadena de texto en palabras con la función .split(). Mediante lambda y  imponemos la condición de que se guarden solo las palabras cuya longitud sea mayor que n. Devolvemos las palabras en una lista.

Ejercicio 17. Importamos la función reduce del móduclo functools. Reduce es una función que reduce la lista a un valor y va iterando de izuqierda a drecha. Como tenemos q cambiar los dígitos a formato decimal lo que hacemos es multiplicar por 10 cada dígito e ir sumando las unidades. 

Ejercicio 18. Primero creamos un diccionario que contenga los nombres, edad y calificación de distintos alumnos. Usamos la función filter para eliminar aquellos que no cumplen la condición de q la calificación>=90. Esto lo hacmoes con la función lambda, ponemos califiación entre [] porque es la clave y no el valor (del diccionario). Se imprimen aquellos estudiantes que cumplen la condición. 

Ejercicio 19. Para saber si el número de la lista es par o impar utilizamos un lambda que evalúa si la división entre 2 es distinta de 0 (se trata de números enteros). En caso de que sea distinto de 0 usamos filter para que solo guarde esos valores (o sea los impares) en una lista. 

Ejercicio 20. Para filtrar por tipo de elemento, hacemos un filter con lambda en que solo se guarden en la lista los valores cuyo tipo sea integer. 

Ejercicio 21. Usamos la funciónn lambda para definir el cubo del parámetro, x en este caso. El uso de lambda hace que sea posible hacerlo de forma más compacta.

Ejercicio 22. Importamos la función reduce. Luego aplicamos esta función mediante lambda a toda la lista, ya que itera sobre todos los elementos de la lista acumulándolos y evaluándolos de izuqierda a derecha.

Ejercicio 23. En este caso reduce va sumando, es decir concatenando las palabras de la lista de izquierda a derecha hasta terminar el total de la lista. 

Ejercicio 24. En este caso la función devuelve la diferencia total de los valores de la lista restanto los elementos de izquierda a derecha.

Ejercicio 25. En este caso se utiliza la función len() para contar el número de caracteres que incluye la cadena de texto que pide como argumento la función, incluyendo espacios y signos de puntuación. 

Ejercicio 26. Mediante la función lambda hacemos la división utilizando % (el operador resto) para que nos devuelva e resto de la división. 

Ejercicio 27. Antes de realizar la división evaluamos la longitud de la lista con len() para evitar la división entre 0. Si es distinta de 0, devuelve el promedio de los valores de la lista. 

Ejercicio 28. La función toma una lista como argumento. Primero creamos una lista vacía, vistos, donde almacenamos los elementos que ya han sido analizados. Mediante un bucle for recorremos los elementos de la lista, y si el elemento está ya presente en la lista vistos, sería el primer elemento repetido y devuelve ese valor. Si no hay ningún elemento repetido devuelve la frase. 

