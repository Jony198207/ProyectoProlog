# Prolog: Operaciones con polinomios.

Si bien la manipulación de polinomios puede ser una labor fácil, su manejo se complica conforme crece el grado de estas expresiones matemáticas. Debido a esto es que desarrollamos un programa capaz de **crear, sumar, multiplicar, evaluar y derivar polinomios**.

Puedes encontrar el código de este programa [aquí](https://github.com/Jony198207/ProyectoProlog/blob/main/C%C3%B3digo_Operador_de_Polinomios), y para utilizarlo necesitarás tener instalado Prolog, más no se requiere tener conocimiento previo del mismo. Si aún no cuentas con esta aplicación, puedes descargarla en [este link](https://www.swi-prolog.org/download/stable), sin importar si eres usuario Windows o MacOSX.

## Inicializar el proyecto

Para usar el código sigue estos pasos:

1) Haz click en "File", seguido de "consult" y selecciona el archivo previamente descargado que contiene el código:
![Imágen2](https://github.com/179786-moises/imagen/blob/main/B2.jpeg)

   Se mostrará una pantalla como la siguiente, con la que sabrás que la compilación del programa se ejecutó correctamente:
  ![Imágen3](https://github.com/179786-moises/imagen/blob/main/B3.jpeg)

   Finalmente, escribe la sentencia `maini`, lo que inicializará el programa y te desplegará el menú de opciones de las operaciones que podrás realizar.
   ![image](https://user-images.githubusercontent.com/101894380/159102602-e9dc22f7-b1d0-44e8-aa49-48c68f4a07ac.png)

## Crear polinomios 
Como se muestra en la imagen anterior, en el menú de opciones para crear un polinomio debes escribir la letra *C*. **Es imperativo que esta sea la primera acción a ejecutar**, pues si no existen polinomios creados en el sistema, no podrás realizar ninguna operación.

Esta función trabaja mediante listas, asociando los coeficientes en orden descendente con la incognita y su respectivo grado según la secuencia en la que se ingresan los datos. Si ingresamos simplemente el valor *15*, el sistema lo tomará como un **monomio de grado cero, es decir, como una constante**. En cambio, si generamos una lista de coeficientes, el resultado será un polinomio con esas variables.

Por ejemplo: 
Si la lista es **[8,7,6,5,4]**, el polinomio que el sistema reconocerá y con el que posteriormente podremos hacer operaciones será:
                                    ![image](https://user-images.githubusercontent.com/101894380/159103921-39d9280b-77e3-4651-a90f-b510674e821d.png).
Ahora bien, si el polinomio que deseas crear no es completo, es decir, no contiene todos los grados de n hasta 0, puedes crearlo con el uso de ceros. Por ejemplo:

 **[4,3,0,0,1]** ------------->  ![image](https://user-images.githubusercontent.com/101894380/159104133-5f5008ee-068e-41ff-bf25-6575785e69e3.png)



## Sumar

## Multiplicar

## Evaluar

## Derivar

## Posibles errores de ejecución (QUIZÁ)
