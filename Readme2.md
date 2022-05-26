# Prolog: Operaciones con polinomios.

Si bien la manipulación de polinomios puede ser una labor fácil, su manejo se complica conforme crece el grado de estas expresiones matemáticas. Debido a esto es que desarrollamos un programa capaz de **crear, sumar, restar, multiplicar y derivar polinomios**.

Puedes encontrar el código de este programa [aquí](https://github.com/Jony198207/ProyectoProlog/blob/main/C%C3%B3digo_Operador_de_Polinomios), y para utilizarlo necesitarás tener instalado Prolog, más no se requiere tener conocimiento previo del mismo. Si aún no cuentas con esta aplicación, puedes descargarla en [este link](https://www.swi-prolog.org/download/stable), sin importar si eres usuario Windows o MacOSX.

### Tabla de contenidos
* [Inicializar el proyecto](#inicializar-el-proyecto)
* [Crear polinomios](#crear-polinomios) 
  * [Sumar](#sumar)  
  * [Restar](#restar) 
  * [Multiplicar](#multiplicar) 
  * [Derivar](#derivar) 
* [Posibles errores de ejecución](#posibles-errores-de-ejecución) 

## Inicializar el proyecto

Para usar el código sigue estos pasos:

1) Haz click en "File", seguido de "consult" y selecciona el archivo previamente descargado que contiene el código:
![Imágen2](https://github.com/179786-moises/imagen/blob/main/B2.jpeg)

2) Se mostrará una pantalla como la siguiente, con la que sabrás que la compilación del programa se ejecutó correctamente:
  ![Imágen3](https://github.com/179786-moises/imagen/blob/main/B3.jpeg)

3) Finalmente, escribe la sentencia `maini`, lo que inicializará el programa y te desplegará el menú de opciones de las operaciones que podrás realizar.
   ![image](https://user-images.githubusercontent.com/101894380/159102602-e9dc22f7-b1d0-44e8-aa49-48c68f4a07ac.png)

## Crear polinomios 

Como se muestra en la imagen anterior, en el menú de opciones para crear un polinomio debes escribir la letra `C`. **Es imperativo que esta sea la primera acción a ejecutar**, pues si no existen polinomios creados en el sistema, no podrás realizar ninguna operación.

Esta función trabaja mediante listas proporcionadas por el usuario, asociando los coeficientes en orden descendente con la incognita y su respectivo grado según la secuencia en la que se ingresan los datos, por lo que **la consola te solicitará una lista de coeficientes para crear un polinomio**. Si ingresas simplemente el valor *15*, el sistema lo tomará como un monomio de grado cero, es decir, como una constante. En cambio, si generas una lista de coeficientes, el resultado será un polinomio con esas variables.

Por ejemplo: 
Si la lista es **[8,7,6,5,4]**, el polinomio que el sistema reconocerá y con el que posteriormente podremos hacer operaciones será:
                                    ![image](https://user-images.githubusercontent.com/101894380/159103921-39d9280b-77e3-4651-a90f-b510674e821d.png).

Ahora bien, si el polinomio que deseas crear no es completo, es decir, no contiene todos los grados de n hasta 0, puedes crearlo con el uso de ceros. Por ejemplo:


**[4,3,0,0,1]** ------------->   ![image](https://user-images.githubusercontent.com/101894380/159104133-5f5008ee-068e-41ff-bf25-6575785e69e3.png)



## Sumar

Para poder hacer uso de esta función deberás haber creado previamente dos polinomios y, acto seguido, escribir en la consola el comando `Suma` para indicar que queremos sumar dichos polinomios. De esta manera, para realizar una operación de este tipo tendríamos una secuencia como la siguiente:

![image](https://user-images.githubusercontent.com/101894380/159105013-e66e20f9-e278-4c6f-940f-44d3cec94694.png)

Como se muestra en la imágen anterior, funciona de tal manera que suma todos aquellos elementos del mismo grado y, sí existe un elemento de grado *j* en un polinomio pero no en el otro, simplemente reporta el elemento existente.



## Restar

Al escribir en la consola `-` podrás utilizar esta función. Una resta puede entenderse como una suma, pues `A - B` = `A + (-B)`. Debido a ello es que tanto la lógica como el código son analogós a los de la suma. Por tanto, la secuencia a seguir para solicitar a la consola la resta de dos polinomios sería la misma que en la suma, intercambiando el comando de `Suma` por el de `-`.



## Multiplicar

Se seleciona con la sentencia  `*`. A diferencia de la suma o la resta, la multiplicación no opera solamente entre elementos del mismo grado. Toma el primer elemento del primer polinomio que se creó y lo multiplica por todos los elementos del segundo, después repite este proceso recursivamente hasta que el primer polinomio termina con los elementos que lo constituyen.

Internamente toma los polinomios que se le indica se quiere multiplicar y funciona así: 
![image](https://user-images.githubusercontent.com/101894380/159106566-50e72bbe-349e-492b-a0bc-085f61db3a17.png)

Es decir, toma como argumentos el polinomio **P** y **Q**, realiza la multiplicación entre ellos y guarda el resultado en **S** para posteriormente mostrarlo en la pantalla de la consola.



## Derivar

Para esta función sólo es necesario porporcionar a la consola un polinomio (si se tienen 2, Prolog te solicitará que vuelvas a ingresar los coeficientes del polinomio de tu elección), del cual nos devolverá su respectiva derivada.
Por ejemplo, si ingresas este polinomio:

![image](https://user-images.githubusercontent.com/101894380/159107454-cf57cf95-684c-4159-b75f-9dedad7bee0f.png)

Y, posteriormente escribes en el menú el comando  `D`, obtendrás como respuesta la primera derivada:

![image](https://user-images.githubusercontent.com/101894380/159107352-b995529e-f679-4b88-9f9e-77b6414e8d05.png)



## Posibles errores de ejecución 

La consola de Prolog informará que ocurrió un error si por equivocación escribes una sentencia equivocada o indicas una acción para la que no haz proporcionado la información necesaria, como por ejemplo:
   - [0,4,!,&,9]
   - Resta (en lugar de "-"). En general, ingresar en el menú de operaciones una letra no contenida dentro de las opciones será causa de error. 

Cabe mencionar que los errores en Prolog no se muestran como en otros lenguajes de programación, con letras rojas y un mensaje que indica que es lo que está mal. Sino que despliega una serie de puntos:

![image](https://user-images.githubusercontent.com/101894380/159106274-00e8e065-aaf8-4c15-a4c5-e38426f6b636.png)

Para solucionar este tipo de problemas basta con escribir la sentencia `maini`, lo que te devolverá al menú para reiniciar operaciones.
