# Prolog: Operaciones con polinomios.

Si bien la manipulación de polinomios puede ser una labor fácil, su manejo se complica conforme crece el grado de estas expresiones matemáticas. Debido a esto es que desarrollamos un programa capaz de **crear, sumar, multiplicar, evaluar y derivar polinomios**.

Puedes encontrar el código de este programa [aquí](https://github.com/Jony198207/ProyectoProlog/blob/main/C%C3%B3digo_Operador_de_Polinomios), y para utilizarlo necesitarás tener instalado Prolog, más no se requiere tener conocimiento previo del mismo. Si aún no cuentas con esta aplicación, puedes descargarla en [este link](https://www.swi-prolog.org/download/stable), sin importar si eres usuario Windows o MacOSX.

## Inicializar el proyecto

Para usar el código sigue estos pasos:

1) Haz click en "File", seguido de "consult" y selecciona el archivo previamente descargado que contiene el código:
![Imágen2](https://github.com/179786-moises/imagen/blob/main/B2.jpeg)

   Se mostrará una pantalla como la siguiente, con la que sabrás que la compilación del programa se ejecutó correctamente:
  ![Imágen3](https://github.com/179786-moises/imagen/blob/main/B3.jpeg)

   Finalmente, escribe la sentencia `maini`, lo que inicializará el programa y te desplegará un menú de opciones de posibles operaciones de polinomios.
   ![image](https://user-images.githubusercontent.com/101894380/159102602-e9dc22f7-b1d0-44e8-aa49-48c68f4a07ac.png)

## Crear polinomios 
Debe ser la primera acción a ejecutar, pues si no existen polinomios creados, no podrás realizar ninguna operación.
Cronstructor(A,B). Dónde A es el coeficiente del polinomio y B es el grado y esta formado por el siguiente codigo:
![Cosntructor](https://github.com/179786-moises/imagen/blob/main/Constructor.png)
Sigueindo con la forma de programación de Prolog este código es recursivo y sus condiciones están definidas por otros constructores como "poli". Está diseñado para crear una lista en la cúal se ponga 0 en todos los lugares en los que no hay constante y A en el lugar del valor de B.

## Sumar

## Multiplicar

## Evaluar

## Derivar

## Posibles errores de ejecución (QUIZÁ)
