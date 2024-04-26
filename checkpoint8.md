# 1.¿Qué tipo de bucles hay en JS?

Los bucles, son una estructura de programación que te permiten ejecutar instrucciones de forma repetitiva, dentro de un bloque de programación. En este artículo se te explicara la sintaxis con ejemplos en el JavaScript sobre los bucles.

Los bucles son una herramienta muy importante en la programación, ya que nos permiten ejecutar un bloque de código varias veces seguidas, se trata de uno de los conceptos básicos en programación. Hay dos tipos principales de bucles: los bucles «while» y los bucles «for».

Evidentemente, si estás pensando en formarte como desarrollador Full Stack, Data Scientist o incluso si quieres empezar con cualquier lenguaje de programación, deberías conocer los bucles cuanto antes.

Esta estructura de programación existe en la mayoría de lenguajes de programación.

### 1.1 Declaración for

Es un tipo de bucle cuya ejecución dura hasta que su condición se evalué como falsa (false). Es similar a los ciclos for de Java, PHP, C# y otro lenguajes de programación.

Además, este tipo de bucle es el más empleado en la programación.

Sintaxis:
~~~
for ([expresiónInicial]; [expresiónCondicional]; [expresiónDeActualización])
    cuerpoBucle
~~~

La estructura se describe de la siguiente manera:

* **expresiónInicial:** Esta expresión indica la condición para el inicio del ciclo. Usualmente es la declaración de una variable numérica.
* **expresiónCondicional:** Esta expresión es la condición que se debe mantener para que siga ejecutando el ciclo.
* **expresiónDeActualización:** Esta expresión cambia el valor de la variable numérica indicada en la [expresionInicial]
* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración del bucle.
 

##### Ejemplo N° 1
En este ejemplo declaras una variable x con valor inicial 1 y por cada iteración su valor va incrementando a 1.

~~~   
for(var x=1;x<=6;x=x+1){
    console.log(x);
}
~~~
Puedes revisar  este ejemplo y considerar a la variable x como la expresión de condición para que se inicie, mantenga y finalice el bucle. El bucle tiene las siguientes partes:

* **Expresión Inicial (var x=1):** Consiste en la declaración de la variable x con el valor inicial 1 para que comience el bucle.

* **Expresión Condicional (x<=6):** Consiste en la evaluación la variable x para que ejecute la iteración. En este ejemplo la variable x condiciona que el bucle se ejecutara hasta que dicha variable x no sea menor o igual a 6. En este caso, cuando la variable x tenga el valor 7 ya no volverá a ejecutarse y terminara el bucle. Como se explicó este bucle se mantiene hasta que la condición llegue a un valor falso (false). El valor de la variable x se evalúa antes que inicie cada ciclo.

* **Expresión de Actualización (x=x+1):** En esta declaración se actualiza el valor de la variable x. En este ejemplo por cada iteración el valor de la variable x a 1. En caso de solo incrementar el valor de una variable numérica a 1 se puede emplear también esta expresión: (x++).

Resultado:
![](https://estilow3b.com/wp-content/uploads/2021/05/2-JavaScript-Bucles-Declaracion-for.png)


### 1.2 Declaración do…while

Es similar al ciclo for explicado anteriormente. Se ejecuta hasta que la condición sea falsa (false). La diferencia se basa en que la evaluación se realiza al final de cada iteración.

Sintaxis
~~~
do
  cuerpoBucle       
while (expresionCondicional);
~~~

La estructura se describe de la siguiente manera:
* **expresiónCondicional:** Es la expresión que condiciona la ejecución de la iteración del bucle.

* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración.
 

##### Ejemplo N° 1

En este ejemplo se evaluará la variable i como expresión condicional para la ejecución del bucle. Cuya variable incrementara dentro del cuerpo del bucle.

~~~
let i=0;
do{
    i=i+1;
    console.log(i);
}
while(i<5);
~~~

Puedes revisar  este ejemplo y considerar a la variable i como la expresión de condición para que dure la iteración del bucle. El ciclo tiene las siguientes partes:
* **Declaración Variable (let i=0):** Se declara la variable i antes de ingresar al ciclo con el valor inicial 0.

* **Actualización de Variable (i=i+1):** Dentro del cuerpo del bucle se actualiza el valor de la variable i a más 1.

* **Evaluación de Expresión Condicional (while(i<5)):** En esta declaración se evalúa la expresión condicional; en este caso la variable es i. Cuando termine cada iteración se realiza dicha evaluación para mantener o terminar el bucle y seguir con las instrucciones siguientes. En este caso se ejecuta la iteración 5 veces.
 

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/3-JavaScript-Bucles-Declaracion-do-while.png)

##### Ejemplo N° 2

En este ejemplo es igual al Ejemplo N° 1 solo que la variable i se iniciara con el valor 6.

~~~   
let i=6;
do{
    i=i+1;
    console.log(i);
}
while(i<5);
~~~

Puedes revisar  este ejemplo y considerar a la variable **i** como la expresión de condición para que dure la iteración del bucle. El ciclo tiene las siguientes partes:
* **Declaración Variable (let i=6):** Se declara la variable i antes de ingresar al ciclo con el valor inicial 6.

* **Actualización de Variable (i=i+1):** Dentro del cuerpo del bucle se actualiza el valor de la variable i a más 1. Es decir antes de su evaluación tendrá la variable el valor 7 y se ejecutara una vez las instrucciones del cuerpo del bucle. Pues la variable de valor inicial 6 se ha incrementado más a 1.

* **Evaluación de Expresión Condicional (while(i<5)):** En esta declaración se evalúa la expresión condicional. Pero después de la iteración del cuerpo del bucle el valor de la variable es 7. Por tal razón, la expresión condicional es falsa y en consecuencia termina el ciclo y solo tiene una iteración.
 

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/4-JavaScript-Bucles-Declaracion-do-while.png)
 

### 1.3 Declaración while

Este ciclo se ejecutara mientras la condición sea verdadera (true).

~~~
Source code	   
while (expresionCondicional)
       cuerpoBucle
~~~

La estructura se describe de la siguiente manera:
* **expresiónCondicional:** Es la expresión que condiciona la ejecución de la iteración del bucle.

* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración.
 

##### Ejemplo N° 1

En este ejemplo se evaluará la variable x como expresión condicional para la ejecución del bucle. Cuya variable incrementara dentro del cuerpo del bucle.

~~~	   
let x=0;
while(x<5){
    x=x+1;
    console.log(x);
}
~~~

Puedes revisar  este ejemplo y considerar a la variable x como la expresión de condición para que dure la iteración del bucle. El bucle tiene las siguientes partes:
* **Declaración Variable (let x=0):** Se declara la variable x antes de ingresar al ciclo con el valor inicial 0.

* **Actualización de Variable (x=x+1):** Dentro del cuerpo del bucle se actualiza el valor de la variable x a más 1.

* **Evaluación de Expresión Condicional (while(x<5)):** En esta declaración se evalúa la expresión condicional; en este caso la variable x. La evaluación se realiza antes de cada iteración. El resultado en este ejemplo es la iteración de 5 veces. Cuando la variable x tenga el valor 6, ya no cumplirá la condición de verdadero y terminara la iteración del ciclo.

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/5-JavaScript-Bucles-Declaracion-while.png) 

### 1.4 Declaración for…in

Este bucle es diferente a los anteriores, pues recorre los elementos de una lista (array) y las propiedades de un objeto.

~~~
Source code	   
for (variable in objeto|array)
 
    cuerpoBucle
~~~

La estructura se describe de la siguiente manera:

* **variable:** Es la expresión que representa el índice cada uno de los elementos de una lista o el índice de las propiedades de un objeto.

* **objeto|array:** Puede ser un objeto con sus respectivas propiedades o una lista (array) y sus elementos.

* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración del bucle.
 

##### Ejemplo N° 1

En este ejemplo el bucle recorrerá un objeto con sus respectivas propiedades y valores respectivos. El objeto es Persona.

~~~	   
var Persona={
    Nombre:'Williams',
    Apellidos:"Morales",
    Edad:36,
    }
 
for(item in Persona){   
    //Obtener cada propiedad del objeto
    console.log(item);
 
    //Obtener cada valor de cada propiedad
    //del objeto
    console.log(Persona[item]);    
}
~~~

En este ejemplo se recorre el objeto Persona para obtener el nombre de sus propiedades y sus respectivos valores. El ciclo tiene las siguientes partes:

* **Declaración Objeto ( var Persona = {} ):** Se declara el objeto persona con las propiedades Nombre (Nombre = “Williams”), Apellidos (Persona.Apellidos=”Morales”), Edad ( Persona.Edad = 36 ).

* **Ciclo de Recorrido (for(item in Persona) ):** Representa el recorrido de la variable ítem en el objeto Persona. La variable ítem contiene el nombre de la propiedad del objeto por cada iteración.

* **Mostrar la propiedad del objeto ( ítem ):** Se obtiene el nombre de la propiedad por iteración.

* **Mostrar el valor de la propiedad del objeto ( Persona\[ítem] ):** Se obtiene el valor de la propiedad según el nombre de la propiedad.
 
Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/6-JavaScript-Bucles-Declaracion-for-in.png)

##### Ejemplo N° 2

En este ejemplo el bucle recorrerá una lista (array) con sus respectivos elementos. El objeto es Paises.

~~~
var Paises=[];
 
Paises.push('Peru');
Paises.push('Colombia');
Paises.push('Chile');
Paises.push('Brasil');
 
for(item in Paises){   
    //Obtener el indice 
    console.log(item);
 
    //Obtener el valor de la lista 
    //según el su indice
    console.log(Paises[item]);    
}
~~~

En este ejemplo se recorre la lista (array) Paises para obtener el índice del array y los valores correspondientes según su índice. El bucle tiene las siguientes partes:

* **Declaración Lista (Array) ( var Paises = \[] ):** Se declara el listado de países con sus elementos (‘Peru’,’Colombia’,’Chile’,’Ecuador’). Los elementos se agregan a la lista con el método push.

* **Ciclo de Recorrido (for(item in Paises) ):** Representa el recorrido de la variable ítem en el listado Paises. La variable ítem contiene el índice del listado Paises por cada iteración.

* **Mostrar el índice ( ítem ):** Se obtiene el índice del listado. Se comienza desde cero.
 
* **Mostrar el valor del listado ( Paises\[ítem] ):** Se obtiene el valor del listado, según el índice.
 
Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/7-JavaScript-Bucles-Declaracion-for-in.png)

### 1.5 Declaración for…of

Este bucle recorre los elementos de un array. No incluye las propiedades de un objeto y sus valores.

~~~	   
for (variable of objetoIteracion)
 
    cuerpoBucle
~~~

La estructura se describe de la siguiente manera:

* **variable:** Es la expresión que representa un elemento del objetoIterable (array, map, etc.).

* **objetoIteracion:** Es un objeto de iteración como una lista (array).

* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración del bucle.
 

##### Ejemplo N° 1

En este ejemplo el bucle recorrerá un objeto de tipo lista (array) para obtener sus valores. La lista es Empleado.

~~~	   
var Empleado=['Williams','Morales',36,1500];
Empleado.Pais='Peru';
 
for(let item of Empleado){
    console.log(item)
}
~~~

En este ejemplo se recorre la lista (array) Empleado para obtener sus valores. El bucle tiene las siguientes partes:

* **Declaración Array ( var Empleado = \[] ):** Se declara la lista (array) Empleado con los elementos: “Williams”, ”Morales”, 36, 1500 ).

* **Declaración de Propiedad (Pais=’Peru’ ):** A la lista (array) se le asigna una propiedad y valor.

* **Ciclo de Recorrido (for(let item of Empleado) ):** Representa el recorrido de la variable ítem en la lista (array) Empleado. La variable ítem contiene el elemento del array.

* **Mostrar el índice ( ítem ):** Se obtiene el elemento del array por cada iteración. Pero la declaración ítem no muestra la propiedad y/o su valor.
 

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/8-JavaScript-Bucles-Declaracion-for-of.png)


### 1.6 Declaración break

La declaración break permite terminar el ciclo antes que se cumpla la expresión condicional

~~~   
bucle (expresionCondicional)
      cuerpoBucle
      expresionSalto;
~~~

La estructura se describe de la siguiente manera:
* **expresionCondicional:** Es la expresión que condiciona la iteración del bucle.

* **expresionSalto:** Es la declaración que da por terminado el bucle.
cuerpoBucle: Es el conjunto de instrucciones que se ejecutan durante cada iteración.
 
##### Ejemplo N° 1

En este ejemplo el bucle recorrerá hasta que la variable x tenga el valor 5. Sin embargo, terminara el ciclo del bucle cuando el valor tenga 3. Pues habrá un flujo condicional que evalué, si la variable x tenga el valor 3 entonces se ejecute la declaración **break** y se termine el bucle.

~~~   
for(var x=0;x<=5;x=x+1){
    if(x==3){
        break;
    }
    console.log(x);
}
~~~

En este ejemplo el bucle se ejecutara hasta que la variable tenga una valor superior a 5 ( x=6 ). El ciclo tiene las siguientes partes:

* **Expresión Inicial (var x=0):** Consiste en la declaración de la variable x con el valor inicial 0 para que comience el bucle.

* **Expresión Condicional (x<=5):** Consiste en la evaluación de la variable x para que ejecute la iteración. En este ejemplo la variable x condiciona que el bucle se ejecutara hasta que dicha variable x no sea menor o igual a 5. Según la condición del bucle, cuando la variable x tenga el valor 6 ya no debería volverá a ejecutarse y terminara el bucle. Como se explicó este ciclo se mantiene hasta que la condición llegue a un valor falso (false). El valor de la variable x se evalúa antes que inicie cada ciclo.

* **Expresión de Actualización (x=x+1):** En esta declaración se cambia el valor de la variable x. En este ejemplo por cada iteración el valor de la variable x sea más 1. En caso de solo incrementar el valor de la variable numérica a 1 se puede emplear también esta expresión: (x++).
* **Expresión de Salida del Bucle ( break ):** Esta expresión se ejecutara cuando la condicional if evalué la variable x y tenga el valor 3. En consecuencia, se terminara el bucle sin que la variable llegue a tener el valor 6; como se esperaba en la expresión condicional.

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/9-JavaScript-Bucles-Declaracion-break.png)


### 1.7 Declaración continue

La declaración continue termina la iteración actual de bucle y continua con la siguiente iteración del bucle.

~~~   
bucle (expresionCondicional)
      cuerpoBucle
      expresionSalto;
~~~

La estructura se describe de la siguiente manera:

* **expresionCondicional:** Es la expresión que condiciona la iteración del bucle.

* **expresionSalto:** Es la declaración que da por terminado la iteración actual del bucle y pasa a ejecutar la siguiente iteración.

* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración.
 

##### Ejemplo N° 1

En este ejemplo el bucle recorrerá hasta que la variable x tenga el valor 5. Sin embargo, cuando la variable tenga el valor 3 terminara la iteración y continuara con la siguiente iteración. Pues habrá un flujo condicional (if) que evaluara, si la variable x tiene el valor 3. En consecuencia, se ejecutara la declaración **continue** y se termine la iteración actual del bucle.

~~~	   
for(var x=0;x<=5;x=x+1){
    if(x==3){
        continue;
    }
    console.log(x);
}
~~~

En este ejemplo el bucle se ejecutara hasta que la variable tenga una valor superior a 5 ( x=6 ). El bucle tiene las siguientes partes:

* **Expresión Inicial (var x=0):** Consiste en la declaración de la variable x con el valor inicial 0 para que comience el bucle.

* **Expresión Condicional (x<=5):** Consiste en la evaluación la variable x para que ejecute la iteración. En este ejemplo la variable x condiciona que el bucle se ejecutara hasta que dicha variable x no sea menor o igual a 5. En teoría, cuando la variable x tenga el valor 6 ya no debería volverá a ejecutarse y terminara el bucle. Como se explicó este bucle se mantiene hasta que la condición llegue a un valor falso (false). El valor de la variable x se evalúa antes que inicie cada iteracion.

* **Expresión de Actualización (x=x+1):** En esta declaración se cambia el valor de la variable x. En este ejemplo por cada iteración el valor de la variable x se incrementa a 1. En caso de incrementar el valor de la variable numérica a 1 se puede emplear también esta expresión: (x++).

* **Expresión de Salida del Bucle ( continue ):** Esta expresión se ejecutara cuando la condicional if evalué la variable x y tenga el valor 3. En consecuencia, se terminara la iteración actual del bucle y prosiga con la iteración siguiente.

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/10-JavaScript-Bucles-Declaracion-continue.png)

 

### 1.8 Declaración labeled

Es una etiqueta, semejante a una variable que hace referencia a un bucle determinado. Esta etiqueta se puede emplear para ejecutar un **break o continue** en el bucle referenciado.

~~~	   
etiquetaBucle: Bucle (expresionCondicional)
        cuerpoBucle
~~~

La estructura se describe de la siguiente manera:

* **etiquetaBucle:** Es la expresión que condiciona la iteración del ciclo.

* **cuerpoBucle:** Es el conjunto de instrucciones que se ejecutan durante cada iteración.
 

##### Ejemplo N° 1

En este ejemplo existen 2 bucles: uno externo y otro interno. El bucle externo estará referenciado a una etiqueta ( labelBucle ). Cuando dentro del cuerpo del bucle interno se evalué el valor de las variables x y z a 3 al mismo tiempo. Se empleara la etiqueta labelBucle para terminar la ejecución de dicho bucle con la declaración break. Por lo tanto, se terminara la ejecución de ambos bucles (externo e interno) y se continuara con las siguientes instrucciones.

~~~   
let x=0;
let z=0;
labelBucle:while(true){
    console.log("Bucle Externo :" + x);
    x=x+1;
    z=1;
    while(true){
        console.log("Bucle Interno :" + z);
        z=z+1;
        if(z=== 3 && x===3){
            console.log('Salir Bucle labelBucle');
            break labelBucle;
        }else if(z===3){
            break;
        }
    }
}
~~~

Este ejemplo tiene las siguientes partes:

* **Declaración y Referencia Bucle Externo a Etiqueta ( labelBucle:while(true) ):** Consiste en la declaración de una etiqueta semejante a una variable. Para luego emplearla para terminar el bucle.

* **Actualización de la Variable del Bucle Externo ( x= x+1 ):** Esta expresión actualiza la valor de la variable x del bucle externo a más 1 por cada iteración del bucle externo.

* **Declaración de Bucle Interno (while(true) ):** Consiste en la declaración del bucle interno. Donde la condicional es true, igual al bucle externo. Con la expresión condicional de ambos bucles siendo true, serian bucles infinitos. Para más detalle de este tipo de bucles, revisar su respectiva explicación en este mismo post.

* **Actualización de la Variable del Bucle Interno (z=z+1):** Esta expresión actualiza el valor de la variable del bucle interno a 1 por cada iteración del bucle interno.

* **Sentencia Condicional (if(z=== 3 && x===3) ):** Esta sentencia if evalúa una expresión como verdadero (true) o falso (false). En este caso, evalúa si las variables z y x tiene el valor 3. De cumplir con esa condición se ejecuta la instrucción (break labelBucle ) para que termine el bucle externo con el cual esta referenciado la etiqueta labelBucle. Por lo tanto, se termina la ejecución de los bucles externo e interno.

* **Sentencia Condicional Si Cumple (lse if(z===3){ ):** En caso de no cumplir la condición de la sentencia If; se evalúa esta sentencia ( else if … ). Donde solo se verifica el valor de la variable z y de tener el valor 3, se terminara la ejecución solo del bucle interno con la declaración break explicada anteriormente y continuara iterando el bucle externo. Por consiguiente, se volverá a ejecutar el bucle interno. Hasta que las variables x y z tengan el valor 3 cada una y se ejecute la instrucción break labelBucle y termine ambos bucles (interno y externo).

Resultado
![](https://estilow3b.com/wp-content/uploads/2021/05/11-JavaScript-Bucles-Declaracion-labeled.png)

### 1.9 Conclusiones

Si el cuerpo del bucle es de una solo línea de código, no es obligatorio colocarlo entre llaves ({…}). Pero, si dicho cuerpo de bucle es de más de una línea de código es obligatorio colocarlo entre llaves.
El for es el bucle más utilizado en los lenguajes de programación.
Se puede referenciar un bucle a una etiqueta. Luego emplearla para terminar solo una iteración de dicho bucle ( \[etiquetaBucle] continue ) o todo el ciclo completo del bucle ( \[etiquetaBucle] break ).
El bucle for y do while son similares, pues ambas se ejecutaran hasta que su condición sea falsa.

# 2.¿Cuáles son las diferencias entre const, let y var?

Las tres se utilizan como declaracion de variables. vamos a ver que diferencia unas de otras.

La declaración var es similar a let. Casi siempre podemos reemplazar let por var o viceversa y esperar que las cosas funcionen:

~~~
var message = "Hola";
alert(message); // Hola
~~~

Pero internamente var es una bestia diferente, originaria de muy viejas épocas. Generalmente no se usa en código moderno, pero aún habita en el antiguo.

var permite reasignar un valor a una variable. Si tengo algo como

~~~
var nombre = 'Jose'
~~~

puedo reasignarlo y decir:

~~~
var nombre = 'Juan'
~~~

Y al imprimir en consola obtendría 'Juan'. Esto resulta útil en algunos casos, pero suele considerarse una mala práctica porque al reasignar variables estamos reescribiéndolas. Es mejor usar let o const.

Let y const son otra cosa, ya que una vez declaradas no pueden declararse de nuevo y si tecleara el ejemplo anterior me daría error. ¿Cuál es la diferencia entonces? Let puede modificarse dentro de su ámbito. Esto sería correcto,
~~~
    saludar = "dice Hola tambien";
~~~
pero esto otro no:
~~~
let saludar = "dice Hola";
let saludar = "dice Hola tambien"; // error: Identifier 'saludar' has already been declared
~~~
En cuanto a const, no puede ni redeclararse ni modificarse. Esto resulta útil cuando hablamos de cosas que no van a cambiar nunca, como por ejemplo:
~~~
const pi = 3,14
~~~
Si intento cambiarlo dará error.

# 3.¿Qué es una función de flecha?

Una expresión de función flecha es una alternativa compacta a una expresión de función tradicional, pero es limitada y no se puede utilizar en todas las situaciones. Del inglés arrow function, las funciones de flcha son una forma de escribir código más conciso e intuitivo.

El símbolo => no es un operador, es una definición de función.

Realmente se trata de una forma concisa de escribir funciones en JavaScript y tienen varias ventajas sobre las funciones tradicionales. Aunque hay quien las rechaza por su aspecto algo críptico y tan diferente al resto de los lenguajes

Una de las principales ventajas de las funciones de flecha es su sintaxis concisa. En lugar de tener que escribir "function" cada vez que quieres declarar una función, puedes utilizar la sintaxis "=>" para declarar una función de flecha.

Por ejemplo, aquí está cómo se vería una función tradicional que toma dos números y los suma:

~~~                      
function sumar(a, b){
	return a + b;                       
}                      
console.log(sumar(3,4));  //daría 7
~~~                      
Mientras que con una función de flecha se podría escribir:

~~~
let sumar = (a, b) => a + b;                      
console.log(sumar(3,4));  //daría 7
~~~
                      
Como se puede observar, la función de flecha se ve mucho más limpia y concisa, ocupa menos espacio y hace lo mismo. Observa que no se ha usado return para devolver el resultado, esto puede hacerse por ser una función en una sola línea. Por supuesto que puede usarse return y el código puede ser más complejo como puedes ver en los ejemplos de abajo.

Otra caracterísitca de las funciones de flecha es el uso que hacen del objeto "this" diferente al de las funciones tradicionales.

En las funciones de flecha, "this" se refiere al contexto en el que se declaró la función, en lugar de al objeto que llama la función, como en las funciones habituales. Puede ser el objeto window, un botón, un evento... Esto puede ser especialmente útil al trabajar con objetos y eventos en JavaScript.

Además, las funciones de flecha son una excelente opción cuando se trata de funciones de callback.

Una función de callback es una función que se pasa como argumento a otra función para que se ejecute en algún momento en el futuro.

Con las funciones de flecha, podemos escribir código de callback mucho más conciso y legible.

Resumiento, las funciones de flecha son una característica valiosa de JavaScript que puede mejorar significativamente la legibilidad y simplicidad de tu código.

A medida que sigue evolucionando el lenguaje, las funciones de flecha se vuelven cada vez más populares entre los desarrolladores. Es una característica importante a tener en cuenta al escribir código JavaScript moderno.

### 3.1 Ejemplos de notación de flecha

##### 3.1.1 Funciones de retorno simple:

Una de las formas más comunes de utilizar las funciones de flecha es cuando quieres crear una función que devuelve un valor simple. Por ejemplo, aquí hay una función que toma un número y lo multiplica por 2:
~~~            
let duplicar = numero => numero * 2; 
                          
console.log( duplicar(5) ); // Salida: 10 
~~~
                        
##### 3.1.2 Funciones con varios argumentos:

Si una función de flecha tiene más de un argumento, debes encerrarlos entre paréntesis. Por ejemplo, aquí hay una función que toma dos números y calcula el resto de dividir el primeor por el segundo

~~~                     
let resto = (a, b) => a % b;                           
console.log(resto(5, 2)); // Salida: 1
~~~
                        
##### 3.1.3 Funciones con un cuerpo de varias líneas:

Si una función de flecha tiene un cuerpo de varias líneas, debes ponerlo entre llaves y usar la palabra clave return para devolver el valor deseado. Por ejemplo, aquí hay una función que toma un número y devuelve su valor absoluto:

~~~                   
let valorAbsoluto = numero => {
	if (numero < 0) { 
		return -numero; 
	} 
return numero; }; 
                         
console.log( valorAbsoluto(-5) ); // Salida: 5 
~~~

                        
##### 3.1.4 Funciones como argumentos de otras funciones (callback):

Las funciones de flecha también son útiles cuando se utilizan como argumentos de otras funciones, especialmente cuando se trata de funciones de orden superior como "map", "filter" y "reduce". Por ejemplo, aquí hay un ejemplo de cómo se puede utilizar una función de flecha con el método "map" para duplicar todos los elementos en un array:


~~~                          
let numeros = [1, 2, 3, 4]; 
let duplicados = numeros.map(numero => numero * 2);                   
console.log(duplicados); // Salida : [2, 4, 6, 8] 
~~~

                    
##### 3.1.5 Uso del objeto this

En este ejemplo se muestra la diferencia en cuando al uso de this en las funciones tradicionales y las funciones flecha

~~~
let persona = { 
 nombre: 'Juan',
 edad : 40,
 getEdad : ()=>{
     console.log("this es: ", this); 
     consile.log( this.edad);
     }
 }
persona.getEdad()   // This es {Window ... y undefined, no existe wndows.edad
~~~
                        
En este ejemplo verás que el objeto this es window, el mismo donde se define el objeto persona
~~~
let persona = { 
  nombre: 'Juan',                          
  edad : 40,                       
  getEdad : function(){                   
     console.log("this es: ", this);                      
     console.log( this.edad);                    
     }                        
 }                         
persona.getEdad()   // This es: {persona ... y 40, no existe wndows.edad
~~~
                        
Espero que estos ejemplos te ayuden a entender mejor cómo se utilizan las funciones de flecha en JavaScript y te ayuden a escribir código más limpio y conciso.

# 4.¿Qué es la deconstrucción de variables?

La sintaxis de desestructuración es una funcionalidad fascinante que vino junto con ES6. Es una expresión de JavaScript que permite desempacar valores de arrays o propiedades de objetos en distintas variables. Es decir, podemos extraer datos de arrays y objectos y asignarlos a variables.

### 4.1 ¿Por qué es esto necesario?

Imagina que queremos extraer datos de un array. Anteriormente, ¿cómo se haría esto?

let introduccion = ["Hola", "Yo" , "soy", "Sarah"];
let saludo = introduccion[0];
let nombre = introduccion[3];

console.log(saludo); // "Hola"
console.log(nombre); // "Sarah"

Podemos ver que cuando queremos extraer datos de un array, tenemos que hacer lo mismo una y otra vez.

La desestructuración de ES6 facilita la extracción de estos datos. ¿De qué forma? Primero, discutiremos sobre la desestructuración con array. Luego pasaremos a la desestructuración de objetos.

### 4.2 Desestructuración Básica de array

Si queremos extraer datos de un array, es bastante sencillo usando la sintaxis de desestructuración.

Tomando como referencia el primer ejemplo. En lugar de pasar por ese proceso repetitivo, haríamos esto:

~~~
let introduccion = ["Hola", "Yo" , "soy", "Sarah"];;
let [saludo, pronombre] = introduccion;

console.log(saludo); // "Hola"
console.log(pronombre); // "Yo"
~~~

También podemos lo siguiente, y conseguir el mismo resultado:

~~~
let [saludo, pronombre] = ["Hola", "Yo" , "soy", "Sarah"];

console.log(saludo); // "Hola"
console.log(pronombre); // "Yo"
~~~

##### 4.2.1 Declarando Variables antes de la Asignación

Las variables se pueden declarar antes de ser asignadas de esta manera:
~~~
let saludo, pronombre;
[saludo, pronombre] = ["Hola", "Yo" , "soy", "Sarah"];

console.log(saludo); // "Hola"
console.log(pronombre); // "Yo"
~~~

Observa que las variables se establecen de izquierda a derecha. Así que la primera variable obtiene el primer elemento del array, la segunda variable obtiene el segundo elemento, y así sucesivamente.

##### 4.2.2 Omitiendo elementos en un array

¿Qué pasa si queremos obtener el primer y último elemento de nuestro array en lugar del primero y el segundo, y queremos asignar solo dos variables? Esto también se puede hacer. Fíjate en el siguiente ejemplo:
~~~
let [saludo,,,nombre] = ["Hola", "Yo" , "soy", "Sarah"];

console.log(saludo); // "Hola"
console.log(nombre); // "Sarah"
~~~

¿Qué acaba de suceder?

Pon atención al lado izquierdo de la asignación de variables del array. Observa que en lugar de tener solo una coma, tenemos tres. El separador de coma se utiliza para omitir valores en un array. Por lo que, si deseas omitir un elemento en un array, usa comas.

Veamos otro ejemplo. Si queremos saltar el primer y tercer elemento de la lista. ¿Cómo lo haríamos?
~~~
let [,pronombre,,nombre] = ["Hola", "Yo" , "soy", "Sarah"];

console.log(pronombre); // "Yo"
console.log(nombre); // "Sarah"
~~~
Como ves, el separador de comas es el que hace la magia. Entonces, si queremos omitir todos los elementos, simplemente hacemos esto:
~~~
let [,,,,] = ["Hola", "Yo" , "soy", "Sarah"];
~~~

##### 4.2.3 Asignando el resto de un array

¿Qué sucede si queremos asignar parte del array a variables y el resto de elementos de dicho array a otra variable en particular? En ese caso, haríamos esto:
~~~
let [saludo, ...introduccion] = ["Hola", "Yo" , "soy", "Sarah"];

console.log(saludo); // "Hola"
console.log(introduccion); // ["Yo", "soy", "Sarah"]
~~~
Utilizando este patrón, puedes desempacar y asignar la parte restante de un array a una variable.

### 4.3 Desestructuración con Funciones

También podemos extraer datos de un array devuelto por una función. Digamos que tenemos una función que devuelve un array como el del siguiente ejemplo:
~~~
function obtenerArray() {
    return ["Hola", "Yo" , "soy", "Sarah"];
} 

let [saludo, pronombre] = obtenerArray();

console.log(saludo); // "Hello"
console.log(pronombre); // "I"
~~~
Como puedes observar, obtenemos los mismos resultados.

##### 4.3.1 Usando Valores Predeterminados

Los valores predeterminados se pueden asignar a las variables en caso de que el valor extraído del array sea undefined:
~~~
let [saludo = "hey", nombre = "Sarah"] = ["Hola"];

console.log(greeting); // "Hola"
console.log(name); // "Sarah"
~~~
Por lo tanto, nombre se vuelve "Sarah" porque no está definido en el array.

Intercambiando Valores mediante Desestructuración
Una cosa más. Podemos usar la desestructuración para intercambiar los valores de las variables:
~~~
let a = 3;
let b = 6;

[a, b] = [b, a];

console.log(a); // 6
console.log(b); // 3
~~~

### 4.4 Desestructuración de Objetos

Primero, veamos por qué es necesaria la desestructuración de objetos.

Digamos que queremos extraer datos de un objeto y asignarlos a nuevas variables. Antes de ES6, ¿cómo se haría esto?
~~~
let persona = {
    nombre: "Sarah", 
    pais: "Nigeria", 
    trabajo: "Desarrollador"
};

let nombre = persona.nombre;
let pais = persona.pais;
let trabajo = persona.trabajo;

console.log(nombre); // "Sarah"
console.log(pais); // "Nigeria"
console.log(trabajo); // "Desarrollador"
~~~
Observa lo tedioso que es extraer todos los datos. Tenemos que hacer lo mismo repetidamente. Por suerte, la desestructuración de ES6 provee una solución. Saltemos directamente a ella.

##### 4.4.1 Desestructuración Básica de Objetos

Repitamos el ejemplo anterior con ES6. En lugar de asignar valores uno por uno, podemos usar el objeto de la izquierda para extraer los datos:
~~~
let persona = {
    nombre: "Sarah", 
    pais: "Nigeria", 
    trabajo: "Desarrollador"
};

let {nombre, pais, trabajo} = persona;

console.log(nombre); // "Sarah"
console.log(pais); // "Nigeria"
console.log(trabajo); // "Desarrollador"
~~~
Obtendrás los mismos resultados. También es válido asignar variables a un objeto que no ha sido declarado:
~~~
let {nombre, pais, trabajo} = {
    nombre: "Sarah", 
    pais: "Nigeria", 
    trabajo: "Desarrollador"
};

console.log(nombre); // "Sarah"
console.log(pais); // "Nigeria"
console.log(trabajo); // "Desarrollador"
~~~
##### 4.4.2 Declarando Variables antes de ser asignadas

Las variables en los objetos se pueden declarar antes de asignarlas con desestructuración. Probemos eso:
~~~
let persona = {
    nombre: "Sarah", 
    pais: "Nigeria", 
    trabajo: "Desarrollador"
}; 

let nombre, pais, trabajo;

{nombre, pais, trabajo} = persona;

console.log(nombre); // Error : "Unexpected token ="
~~~
Espera, ¿qué acaba de pasar? Oh, nos olvidamos de agregar () antes de las llaves.

Los paréntesis  ( ) alrededor de la asignación es una sintaxis requerida cuando se usa la desestructuración literal de un objeto sin una declaración. Esto se debe a que {} en el lado izquierdo se considera un bloque y no un objeto literal. Aquí te muestro la forma correcta de hacerlo:
~~~
let persona = {
    nombre: "Sarah", 
    pais: "Nigeria", 
    trabajo: "Desarrollador"
}; 

let nombre, pais, trabajo;

({nombre, pais, trabajo} = persona);

console.log(nombre); // "Sarah"
console.log(trabajo); // "Desarrollador"
~~~
También es importante tener en cuenta que al usar esta sintaxis, los paréntesis () deben ir precedido de un punto y coma. De lo contrario, podría usarse para ejecutar una función de la línea anterior.

Observa como las variables del objeto en el lado izquierdo deben tener el mismo nombre que una clave de propiedad en el objeto persona. Si los nombres son diferentes, obtendremos undefined:
~~~
let persona = {
    nombre: "Sarah", 
    pais: "Nigeria", 
    trabajo: "Desarrollador"
};

let {nombre, amigos, trabajo} = persona;

console.log(nombre); // "Sarah"
console.log(amigos); // undefined
~~~

# 5.¿Qué hace el operador de extensión en JS?

Con el lanzamiento de ECMAScript 6 (ES6), se introdujeron un montón de nuevas funciones y mejoras sintácticas para que JavaScript fuera aún más potente y expresivo. Una de ellas es el operador spread, que ha ganado popularidad rápidamente entre los desarrolladores por su versatilidad y concisión.

En este artículo, examinaremos más de cerca el operador spread de JavaScript y exploraremos cómo puede simplificar tu código y liberar todo su potencial.

### 5.1 ¿Qué es el Operador Spread en JavaScript?

El operador spread en JavaScript es una sintaxis introducida en ECMAScript 6 (ES6) que te permite propagar los elementos de un iterable (como arrays, cadenas u objetos), en otro iterable o llamada a función.

Se denota con tres puntos «...» seguidos de una expresión o un iterable. El operador spread es una potente herramienta que proporciona una forma concisa y flexible de trabajar con datos en JavaScript.

Puede utilizarse para concatenar arrays, crear copias superficiales de arrays, convertir cadenas en arrays de caracteres, fusionar o clonar objetos y pasar dinámicamente valores a funciones o constructores, entre otros casos de uso.

El operador spread simplifica las operaciones complejas y permite un código más expresivo y eficiente. Esto lo convierte en una función muy popular entre los desarrolladores de JavaScript.

### 5.2 Sintaxis y Uso del Operador Spread de JavaScript

Veamos algunos ejemplos de uso del operador spread con arrays, cadenas y objetos para ilustrar su sintaxis y uso.

1. **Concatenar Arrays**

Puedes utilizar el operador spread para distribuir los elementos de un array en otro array. Esto es especialmente útil para concatenar arrays o crear una copia superficial de una array.

Ejemplo:

~~~
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];

// Concatenate arrays using spread operator
const concatenatedArr = [...arr1, ...arr2];
console.log(concatenatedArr); // Output: [1, 2, 3, 4, 5, 6]
~~~

2. **Extendiendo Cadenas de Texto**

Puedes utilizar el operador spread para desglosar los caracteres de una cadena en un array. Esto es útil para convertir una cadena en un array de caracteres, que puede manipularse o combinarse con otros arrays utilizando métodos de array.

Ejemplo:
~~~
const str = "Hello";

// Spread characters of a string into an array
const charArray = [...str];
console.log(charArray); // Output: ['H', 'e', 'l', 'l', 'o']
~~~

3. **Fusionar y Clonar Objetos**

Puedes utilizar el operador spread para propagar las propiedades de un objeto en otro objeto. Esto es útil para fusionar o clonar objetos, crear un nuevo objeto con algunas propiedades anuladas o extraer propiedades específicas de un objeto.

Ejemplo:
~~~
const obj1 = { a: 1, b: 2 };
const obj2 = { b: 3, c: 4 };

// Merge objects using spread operator
const mergedObj = { ...obj1, ...obj2 };
console.log(mergedObj); // Output: { a: 1, b: 3, c: 4 }

// Clone an object using spread operator
const clonedObj = { ...obj1 };
console.log(clonedObj); // Output: { a: 1, b: 2 }
~~~
4. **Extender Argumentos de Función**

El operador spread también puede ser usado en otros contextos, como los argumentos de una función, para pasar valores de manera dinámica a una función o constructor.

Ejemplo:
~~~
// Pass array elements as arguments to a function using the spread operator
const numbers = [1, 2, 3];

const sum = (a, b, c) => a + b + c;

console.log(sum(...numbers)); // Output: 6
~~~

5. **Combinación del Operador Spread con el Parámetro rest**

El operador spread puede utilizarse junto con otras funciones modernas de JavaScript, como la desestructuración de arrays y objetos, para habilitar potentes técnicas de programación funcional. Te permite extraer y manipular elementos de arrays o propiedades de objetos con una sintaxis concisa y expresiva.

Ejemplo:
~~~

const numbers = [1, 2, 3, 4, 5];
const [first, second, ...rest] = numbers;

console.log(first); // Output: 1
console.log(second); // Output: 2
console.log(rest); // Output: [3, 4, 5]
~~~


Los ejemplos anteriores muestran la versatilidad y flexibilidad del operador spread en JavaScript, convirtiéndolo en una herramienta poderosa para manipular y combinar datos de manera concisa y eficiente.

### 5.3 Comprender el Operador Spread y las Copias Superficiales

Es importante tener en cuenta que el operador spread crea copias superficiales de matrices y objetos, y puede tener implicaciones de rendimiento cuando se utiliza con arrays u objetos grandes.

~~~
const originalArray = [[1, 2, 3, 4], 12];
const copiedArray = [...originalArray];

copiedArray[0].push(99);

console.log(originalArray); // Output: [[1, 2, 3, 4, 99], 12]
console.log(copiedArray); // Output: [[1, 2, 3, 4, 99], 12]
~~~

En este código, originalArray es una array con cuatro elementos. Utilizando el operador spread, creamos un nuevo array copiedArray y propagamos en él los elementos de originalArray. A continuación, modificamos el primer elemento de copiedArray añadiendo 99 con el método push.

Cuando obtengas la salida de copiedArray, la salida mostrará que se ha añadido 99 al array del primer elemento, pero hay un problema con la copia superficial que hace el operador spread. El cambio en copiedArray afecta a originalArray.

Esto se debe a que el operador spread no crea copias completamente nuevas de los elementos o propiedades, sino que comparte referencias a los elementos o propiedades originales. Esto puede tener implicaciones de rendimiento cuando se trabaja con arrays u objetos grandes.

Por lo tanto, si trabajas con arrays u objetos grandes, o si necesitas hacer modificaciones profundas en el array u objeto copiado sin afectar al original, quizá debas considerar otros enfoques, como la copia profunda o el uso de bibliotecas diseñadas específicamente para manejar estructuras de datos complejas.

Es esencial utilizar el operador spread con criterio y tener en cuenta las mejores prácticas para un rendimiento y una capacidad de mantenimiento óptimos.

### 5.4 Tres Potentes Consejos para Optimizar el Rendimiento y Evitar Errores Comunes

Para optimizar el rendimiento y evitar errores comunes al utilizar el operador spread, ten en cuenta los siguientes consejos:

1. Evita extender arrayas u objetos grandes, especialmente en rutas de código críticas para el rendimiento.
2. Ten en cuenta los posibles efectos secundarios al extender objetos anidados, y considera la posibilidad de utilizar técnicas de clonación profunda si es necesario.
3. Utiliza el operador spread con criterio y considera enfoques alternativos si el rendimiento es un problema.

### 5.5 Resumen

El operador spread (…) permite concatenar arrays de forma concisa y limpia, clonar arrays y objetos, fusionar objetos, crear argumentos de función de forma dinámica, clonar objetos y arrays anidados complejos, etc.

Debido a su flexibilidad, el operador spread desempeña un papel importante en el futuro del desarrollo de JavaScript, ya que permite a los desarrolladores escribir código más conciso, legible y eficiente.

# 6.¿Qué es la programación orientada a objetos?

La Programación Orientada a Objetos (POO) es un paradigma de programación, es decir, un modelo o un estilo de programación que nos da unas guías sobre cómo trabajar con él. Se basa en el concepto de clases y objetos. Este tipo de programación se utiliza para estructurar un programa de software en piezas simples y reutilizables de planos de código (clases) para crear instancias individuales de objetos. 

A lo largo de la historia, han ido apareciendo diferentes paradigmas de programación. Lenguajes secuenciales como COBOL o procedimentales como Basic o C, se centraban más en la lógica que en los datos. Otros más modernos como Java, C# y Python, utilizan paradigmas para definir los programas, siendo la Programación Orientada a Objetos la más popular. 

Con el paradigma de Programación Orientado a Objetos lo que buscamos es dejar de centrarnos en la lógica pura de los programas, para empezar a pensar en objetos, lo que constituye la base de este paradigma. Esto nos ayuda muchísimo en sistemas grandes, ya que en vez de pensar en funciones, pensamos en las relaciones o interacciones de los diferentes componentes del sistema.

Un programador diseña un programa de software organizando piezas de información y comportamientos relacionados en una plantilla llamada clase. Luego, se crean objetos individuales a partir de la plantilla de clase. Todo el programa de software se ejecuta haciendo que varios objetos interactúen entre sí para crear un programa más grande.

### 6.1 Claves de la Programación Orientada a Objetos

La POO se inspira en la forma en que percibimos y entendemos el mundo que nos rodea. Imagina que estás construyendo un sistema de gestión de una biblioteca. En lugar de pensar en términos de algoritmos y estructuras de datos, la POO te invita a considerar las entidades que existen en el contexto de la biblioteca, como libros, bibliotecarios y usuarios.

En este enfoque, cada una de estas entidades se convierte en un objeto, con propiedades (datos) y comportamientos (funcionalidades). Por ejemplo, un objeto «Libro» puede tener atributos como el título, el autor y el año de publicación, así como métodos para obtener información sobre el libro, prestarlo o devolverlo a la biblioteca.

La clave de la POO radica en la interacción entre estos objetos. Pueden comunicarse entre sí enviándose mensajes y colaborando para lograr un objetivo común. Por ejemplo, un objeto «Usuario» podría enviar un mensaje al objeto «Libro» para solicitar su préstamo, y este último respondería actualizando su estado interno.

### 6.2 Por qué POO?

La Programación Orientada a objetos permite que el código sea reutilizable, organizado y fácil de mantener. Sigue el principio de desarrollo de software utilizado por muchos programadores DRY (Don’t Repeat Yourself), para evitar duplicar el código y crear de esta manera programas eficientes. Además, evita el acceso no deseado a los datos o la exposición de código propietario mediante la encapsulación y la abstracción, de la que hablaremos en detalle más adelante.

##### 6.2.1 Clases, objetos e instancias

¿Cómo se crean los programas orientados a objetos? Resumiendo mucho, consistiría en hacer clases y crear objetos a partir de estas clases. Las clases forman el modelo a partir del que se estructuran los datos y los comportamientos.

El primer y más importante concepto de la POO es la distinción entre clase y objeto.

Una clase es una plantilla. Define de manera genérica cómo van a ser los objetos de un determinado tipo. Por ejemplo, una clase para representar a animales puede llamarse ‘animal’ y tener una serie de atributos, como ‘nombre’ o ‘edad’ (que normalmente son propiedades), y una serie con los comportamientos que estos pueden tener, como caminar o comer, y que a su vez se implementan como métodos de la clase (funciones).

Un ejemplo sencillo de un objeto, como decíamos antes, podría ser un animal. Un animal tiene una edad, por lo que creamos un nuevo atributo de ‘edad’ y, además, puede envejecer, por lo que definimos un nuevo método. Datos y lógica. Esto es lo que se define en muchos programas como la definición de una clase, que es la definición global y genérica de muchos objetos.

![](C:/Users/Alda/Desktop/Dev Camp- Bottega/JavaScript/checkpoint 8/POO.jpg)

Con la clase se pueden crear instancias de un objeto, cada uno de ellos con sus atributos definidos de forma independiente. Con esto podríamos crear un gato llamado Paco, con 3 años de edad, y otro animal, este tipo perro y llamado Pancho, con una de edad de 4 años. Los dos están definidos por la clase animal, pero son dos instancias distintas. Por lo tanto, llamar a sus métodos puede tener resultados diferentes. Los dos comparten la lógica, pero cada uno tiene su estado de forma independiente.

Todo esto, junto con los principios que vamos a ver a continuación, son herramientas que nos pueden ayudar a escribir un código mejor, más limpio y reutilizable.

### 6.3 Principios de la Programación Orientada a Objetos 

##### 6.3.1 La encapsulación

La encapsulación contiene toda la información importante de un objeto dentro del mismo y solo expone la información seleccionada al mundo exterior. 
Esta propiedad permite asegurar que la información de un objeto esté oculta para el mundo exterior, agrupando en una Clase las características o atributos que cuentan con un acceso privado, y los comportamientos o métodos que presentan un acceso público.

La encapsulación de cada objeto es responsable de su propia información y de su propio estado. La única forma en la que este se puede modificar es mediante los propios métodos del objeto. Por lo tanto, los atributos internos de un objeto deberían ser inaccesibles desde fuera, pudiéndose modificar sólo llamando a las funciones correspondientes. Con esto conseguimos mantener el estado a salvo de usos indebidos o que puedan resultar inesperados. 

Usamos de ejemplo un coche para explicar la encapsulación. El coche comparte información pública a través de las luces de freno o intermitentes para indicar los giros (interfaz pública). Por el contrario, tenemos la interfaz interna, que sería el mecanismo propulsor del coche, que está oculto bajo el capó. Cuando se conduce un automóvil es necesario indicar a otros conductores tus movimientos, pero no exponer datos privados sobre el tipo de carburante o la temperatura del motor, ya que son muchos datos, lo que confundiría al resto de conductores.

##### 6.3.2 La abstracción

La abstracción es cuando el usuario interactúa solo con los atributos y métodos seleccionados de un objeto, utilizando herramientas simplificadas de alto nivel para acceder a un objeto complejo.

En la programación orientada a objetos, los programas suelen ser muy grandes y los objetos se comunican mucho entre sí. El concepto de abstracción facilita el mantenimiento de un código de gran tamaño, donde a lo largo del tiempo pueden surgir diferentes cambios.

Así, la abstracción se basa en usar cosas simples para representar la complejidad. Los objetos y las clases representan código subyacente, ocultando los detalles complejos al usuario. Por consiguiente, supone una extensión de la encapsulación. Siguiendo con el ejemplo del coche, no es necesario que conozcas todos los detalles de cómo funciona el motor para poder conducirlo.

##### 6.3.3 La herencia

La herencia define relaciones jerárquicas entre clases, de forma que atributos y métodos comunes puedan ser reutilizados. Las clases principales extienden atributos y comportamientos a las clases secundarias. A través de la definición en una clase de los atributos y comportamientos básicos, se pueden crear clases secundarias, ampliando así la funcionalidad de la clase principal y agregando atributos y comportamientos adicionales.

Volviendo al ejemplo de los animales, se puede usar una sola clase de animal y agregar un atributo de tipo de animal que especifique el tipo de animal. Los diferentes tipos de animales necesitarán diferentes métodos, por ejemplo, las aves deben poder poner huevos y los peces, nadan. Incluso cuando los animales tienen un método en común, como moverse, la implementación necesitaría muchas declaraciones «si» para garantizar el comportamiento de movimiento correcto. Por ejemplo, las ranas saltan, mientras que las serpientes se deslizan. El principio de herencia nos permite solucionar este problema.

##### 6.3.4 El polimorfismo

El polimorfismo consiste en diseñar objetos para compartir comportamientos, lo que nos permite procesar objetos de diferentes maneras. Es la capacidad de presentar la misma interfaz para diferentes formas subyacentes o tipos de datos. Al utilizar la herencia, los objetos pueden anular los comportamientos principales compartidos, con comportamientos secundarios específicos. El polimorfismo permite que el mismo método ejecute diferentes comportamientos de dos formas: anulación de método y sobrecarga de método.

Alrededor de estos principios de la programación orientada a objetos se construyen muchas cosas. Por ejemplo, los Principios SOLID, o los Patrones de diseño, que son recetas que se aplican a problemas recurrentes que se han encontrado y se repiten en varios proyectos.

### 6.4 Beneficios de Programación Orientada a Objetos

Reutilización del código.
Convierte cosas complejas en estructuras simples reproducibles.
Evita la duplicación de código.
Permite trabajar en equipo gracias al encapsulamiento ya que minimiza la posibilidad de duplicar funciones cuando varias personas trabajan sobre un mismo objeto al mismo tiempo.
Al estar la clase bien estructurada permite la corrección de errores en varios lugares del código.
Protege la información a través de la encapsulación, ya que solo se puede acceder a los datos del objeto a través de propiedades y métodos privados.
La abstracción nos permite construir sistemas más complejos y de una forma más sencilla y organizada.

### 6.5 Conclusión

La Programación Orientada a Objetos es actualmente el paradigma que más se utiliza para diseñar aplicaciones y programas informáticos. Son muchas sus ventajas, principalmente cuando necesitas resolver desafíos de programación complejos. Permite una mejor estructura de datos y reutilización del código, lo que facilita el ahorro de tiempo a largo plazo. Eso sí, para ello se requiere pensar bien en la estructura del programa, planificar al comienzo de la codificación, así como analizar los requisitos en clases simples y reutilizables que se pueden usar para diseñar instancias de objetos. 

# 7.¿Qué es una promesa en JS?

Las promesas en JavaScript son un patrón y una característica de manejo asíncrono que se introdujo para facilitar la gestión de operaciones asíncronas en el lenguaje. Una promesa es un objeto que representa un valor que puede estar disponible ahora, en el futuro o nunca. Esta representación encapsula el resultado (éxito o error) de una operación asíncrona.

En otras palabras, proporcionan una forma más estructurada y legible de manejar operaciones asíncronas, permitiendo que el código sea más claro y más fácil de mantener al escribir acciones de JavaScript.

### 7.1 Para qué sirven las promesas en JavaScript

Las promesas en JavaScript sirven para manejar operaciones asíncronas de manera más estructurada y legible. Cuando realizas tareas que no se completan de inmediato, como llamadas a API, lecturas de archivos o consultas a bases de datos, JavaScript necesita una forma de gestionar estas operaciones sin bloquear la ejecución del código.

Las promesas cumplen varias funciones clave:

	*	Manejo del flujo asíncrono óptimo *
	
		Te permiten escribir un código más limpio y comprensible al evitar el anidamiento excesivo de callbacks. En lugar de anidar múltiples callbacks, puedes encadenar métodos .then() de manera más legible.

	*	Gestión de errores *

		Brindan un mecanismo más efectivo para manejar errores en operaciones asíncronas. Puedes usar el método .catch() para capturar errores que ocurren en cualquier parte de la cadena de promesas.

	*	Encadenamiento de operaciones*

		Permiten encadenar múltiples operaciones asíncronas de una manera más intuitiva. El resultado de una promesa puede ser pasado como entrada a la siguiente promesa en la cadena utilizando el método .then().

	*	Manejo de paralelismo *

		Puedes utilizar constructores como Promise.all() y Promise.race() para manejar múltiples promesas al mismo tiempo. El primero espera a que todas las promesas se cumplan antes de continuar, mientras que el segundo se resuelve tan pronto como una de las promesas se cumple.

	*	Legibilidad y mantenibilidad *

		Las promesas hacen que el código asíncrono sea más fácil de leer y mantener, ya que proporcionan una estructura clara para manejar resultados exitosos y errores, en lugar de tener que rastrear flujos de control complejos en callbacks anidados.

	*	Compatibilidad con async/await *

		Asimismo, forman la base de las funciones async y await, una característica introducida en versiones más recientes de JavaScript. async/await simplifica aún más el manejo de código asíncrono al hacer que parezca código síncrono, mejorando la legibilidad.

### 7.2 Estados posibles de una promesa en JavaScript

Una promesa tiene tres estados posibles:

##### 7.2.1 Pendiente (pending)
El estado «Pendiente» (pending) es uno de los tres posibles estados en los que una promesa puede encontrarse en JavaScript. Una promesa está en estado pendiente cuando se crea, pero la operación asíncrona asociada aún no ha sido completada ni ha fallado. En otras palabras, la promesa está en espera de que la operación asíncrona se resuelva o se rechace.

Durante el estado «Pendiente», la promesa está en una especie de limbo. Aunque la operación asincrónica está en curso, la promesa misma no tiene acceso directo al resultado final ni al error que pueda ocurrir. Sin embargo, la promesa se mantiene receptiva a su futuro estado cumplido (fulfilled) o rechazado (rejected).

Cuando la operación asíncrona se completa satisfactoriamente, la promesa pasa del estado «Pendiente» al estado «Cumplido» (fulfilled). En este punto, el valor resultante de la operación se convierte en el resultado de la promesa y puede ser accedido mediante el método .then().

Por otro lado, si la operación asíncrona encuentra un error, la promesa cambia de estado «Pendiente» al estado «Rechazado» (rejected). En este caso, se llama al método reject() en la definición de la promesa o en cualquier lugar donde se rechace explícitamente, y el error proporcionado se convierte en el motivo del rechazo. El manejo de errores se realiza comúnmente usando el método .catch() o utilizando bloques try/catch en combinación con async/await.

##### 7.2.2 Cumplida (fulfilled)

Una promesa entra en el estado «Cumplida» cuando la operación asíncrona asociada se ha completado con éxito y ha producido un valor resultante.

En este estado, la promesa contiene el valor resultante de la operación asíncrona. Esto significa que la promesa ha cumplido su propósito y tiene un resultado con el que trabajar. Este valor puede ser cualquier tipo de dato, como un número, una cadena de texto, un objeto o incluso otra promesa. El valor cumplido se pasa como argumento a la función resolve() cuando se crea la promesa.

Para acceder al valor cumplido de una promesa, se utiliza el método .then() y se proporciona una función que se ejecutará una vez que la promesa esté en el estado «Cumplida».

Es importante destacar que una vez que una promesa está en el estado «Cumplida» no puede cambiar a otro. Esto significa que si una promesa se cumple con un valor, permanecerá en ese estado y no se puede volver a «Pendiente» ni cambiar a «Rechazada».

##### 7.2.3 Rechazada (rejected)

Una promesa entra en el estado «Rechazada» cuando la operación asíncrona asociada ha fallado y se ha producido un error.

En este estado, la promesa contiene información sobre el motivo del fallo, es decir, el error que ocurrió durante la operación asíncrona. El motivo del rechazo se pasa como argumento a la función reject() cuando se crea la promesa.

Para manejar el estado «Rechazada» y el motivo del rechazo, se utiliza el método .catch() o se pueden manejar errores con bloques try/catch en combinación con async/await.

### 7.3 Estructura básica de una promesa en JavaScript

~~~
const myPromise = new Promise((resolve, reject) => {
  // Aquí se realiza la operación asíncrona
  // Si la operación es exitosa, se llama a resolve(valor)
  // Si ocurre un error, se llama a reject(error)
});
~~~
~~~
myPromise
  .then(resultado => {
    // Manejar el resultado si la promesa se cumple
  })
  .catch(error => {
    // Manejar el error si la promesa es rechazada
  });
~~~ 
 
La función resolve se utiliza para cumplir la promesa con un valor, mientras que la función reject se utiliza para rechazar la promesa con un error.

Las promesas también permiten encadenar múltiples operaciones asíncronas usando el método .then(), lo que hace que el código sea más legible y evita el anidamiento excesivo.

Nota: como hemos dicho, en versiones más recientes de JavaScript (a partir de ES6), se introdujeron async/await, que proporcionan una forma aún más cómoda de trabajar con código asíncrono basado en promesas, haciendo que parezca que se está trabajando con código síncrono, pero detrás de escena sigue siendo asincrónico.

##### 7.3.1 Cómo implementar las promesas en JavaScript: ejemplos

**Ejemplo de transacción de pago en línea**

Supongamos que deseamos simular una transacción de pago en línea y queremos asegurarnos de que se manejen correctamente tanto los pagos exitosos como los fallidos, utilizando promesas.

~~~
// Simulación de una función que procesa un pago
function procesarPago(total) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const exito = Math.random() < 0.8; // Simulamos que el 80 % de las veces el pago es exitoso

      if (exito) {
        resolve("Pago exitoso");
      } else {
        reject(new Error("Error en el pago"));
      }
    }, 1500); // Simulamos un retraso de 1.5 segundos para el proceso de pago
  });
}
~~~
~~~
// Ejemplo de uso de la función de procesamiento de pagos
const totalAPagar = 100; // Monto total del pago

procesarPago(totalAPagar)
  .then(resultado => {
    console.log(resultado); // Se ejecutará en caso de pago exitoso
    // Aquí podríamos realizar acciones adicionales, como actualizar la base de datos, enviar un recibo por correo, etc.
  })
  .catch(error => {
    console.error(error.message); // Se ejecutará en caso de pago fallido
    // Aquí podemos ofrecer al usuario la opción de intentar nuevamente o mostrar un mensaje de error
  });
~~~  
  
En este ejemplo, la función procesarPago() simula una transacción de pago en línea. Dependiendo de un valor aleatorio, la función decide si el pago es exitoso o fallido. La promesa que se devuelve se cumple si el pago es exitoso (el 80 % de las veces) y se rechaza si el pago falla.

Luego, utilizamos .then() para manejar el caso de pago exitoso, donde podemos realizar acciones adicionales, como actualizar la base de datos o enviar un recibo por correo electrónico. Empleamos .catch() para manejar el caso de pago fallido, donde es posible ofrecer al usuario opciones para resolver el problema o mostrar un mensaje de error.

**Ejemplo de base de datos**

En este caso, supondremos que estamos trabajando con datos de usuarios y queremos simular la adición de múltiples usuarios a una base de datos, teniendo en cuenta casos exitosos y fallidos.

~~~
// Simulación de una función que agrega usuarios a una base de datos
function agregarUsuarios(usuarios) {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const exito = Math.random() < 0.7; // Simulamos que el 70 % de las veces la operación es exitosa

      if (exito) {
        resolve("Usuarios agregados exitosamente");
      } else {
        reject(new Error("Error al agregar usuarios"));
      }
    }, 2000); // Simulamos un retraso de 2 segundos para la operación de almacenamiento
  });
}
~~~
~~~
// Datos de ejemplo de usuarios a agregar a la base de datos
const nuevosUsuarios = [
  { id: 1, nombre: "Usuario 1" },
  { id: 2, nombre: "Usuario 2" },
  { id: 3, nombre: "Usuario 3" }
];
~~~
~~~
// Uso de la función de agregación de usuarios
agregarUsuarios(nuevosUsuarios)
  .then(resultado => {
    console.log(resultado); // Se ejecutará en caso de operación exitosa
    // Aquí podríamos realizar acciones adicionales, como actualizar la interfaz de usuario o notificar al usuario
  })
  .catch(error => {
    console.error(error.message); // Se ejecutará en caso de operación fallida
    // Aquí podríamos ofrecer al usuario la opción de intentar nuevamente o mostrar un mensaje de error
  });
~~~  
  
Definición de la función agregarUsuarios(): esta función simula el proceso de agregar usuarios a una base de datos. Devuelve una promesa que se cumple si la operación es exitosa (el 70 % de las veces) y se rechaza si la operación falla. La función toma un arreglo de usuarios como argumento.

Simulación de retardo: para simular el tiempo que puede llevar almacenar datos en una base de datos, utilizamos setTimeout() para introducir un retraso de 2 segundos.
Uso de la función de agregación de usuarios: pasamos el arreglo nuevosUsuarios a la función agregarUsuarios(). Luego utilizamos .then() para manejar el caso de éxito, donde podríamos realizar acciones adicionales, y .catch() para manejar el caso de falla, donde podríamos mostrar un mensaje de error.
Datos de ejemplo de usuarios: creamos un arreglo de objetos que representan a los usuarios que deseamos agregar a la base de datos.
Como ves, las promesas en JavaScript son una herramienta esencial para manejar operaciones asíncronas de manera más legible, estructurada y eficiente. Proporcionan una forma de lidiar con el flujo de control en código asíncrono, permitiendo gestionar resultados exitosos y errores de una manera más ordenada. En resumen, han allanado el camino para un manejo más elegante y eficiente de operaciones asíncronas, lo que mejora la calidad del código y la experiencia del desarrollador en la creación de aplicaciones modernas y robustas.

# 8.¿Qué hacen async y await por nosotros?

Async y await en JavaScript son dos palabras clave que nos permiten transformar un código asíncrono para que parezca ser síncrono. Estas palabras clave son muy utilizadas en el contexto de código realizado con promesas.

Nos permite definir situaciones según las que una u otra acción ocurre. Si ninguna de estas acciones sucede, la promesa se rechaza y vemos un error.

![](C:/Users/Alda/Desktop/Dev Camp- Bottega/JavaScript/checkpoint 8/promise.png)

Ten presente que la función de la promesa no cambia cuando utilizamos estas palabras clave. Es decir, el código que la hace posible no se modifica y se mantiene asíncrono. Lo que hacen async y await en JavaScript es añadir transparencia en la forma en la que se ejecuta el código de cara al usuario, simulando ser síncrono para facilitarnos la lectura. A continuación, explicamos exactamente qué hacen las palabras clave async y await en JavaScript.

**async**
	
	La palabra clave async en JavaScript se utiliza en una función para envolver el contenido de la función en una promesa.

**await**

	La palabra clave await en JavaScript nos permite definir una sección de la función a la cual el resto del código debe esperar. Es decir, con await definimos que el código restante de la función debe esperar a que esta sección se resuelva. Por ello, a nuestros ojos, el código se ejecutará de forma síncrona en la terminal. Si no utilizamos await en una función asincrónica, seguramente el código se ejecutará en desorden, pues el programa continuaría leyendo mientras espera al resultado de una función no inmediata.

### 8.1 ¿Cómo utilizar async y await en JavaScript?

Para ejemplificar cómo utilizar async y await en JavaScript, te ponemos un ejemplo. Suponsamos que tenemos la siguiente función doYouLoveMe, que guarda una promesa con el método setTimeout:
~~~
function doYouLoveMe (name) {
	return new Promise (function (resolve, reject) {
		console.log (‘Let me think about it…’)
		setTimeout (() => {
			if (name = ‘Alberto’) {
				resolve (‘Yes!’) {
			} else {
				reject (‘Sorry but no…’)
			}
		}, 1000)
	})
}
~~~

Ahora, queremos gestionar esta promesa utilizando el método then. Esta define qué sucederá cuando la promesa salga bien y cuando la promesa salga mal:

~~~
function loveChecker () {
	doYouLoveMe (‘Alberto’).then (response => {
		console.log (‘Alberto’, response)
	}, error => {
		console.error (‘Alberto’, error)
	})

	doYouLoveMe (‘Frodo’).then (response => {
		console.log (‘Frodo’, response)
	}, error => {
		console.error (‘Frodo’, error)
	})
}
~~~

Entonces, async y await en JavaScript nos permiten reformular nuestro código asíncrono para que parezca ser síncrono a nuestros ojos. Teniendo esto en cuenta, la sintaxis de la función loveChecker se transformaría de la siguiente manera utilizando las keywords async y await:

~~~
async function loveChecker () {
	try {
		let response = await doYouLoveMe (‘Alberto’)
		console.log (‘Alberto’, response)
	} catche (error) {
		console.error (‘Alberto’, error)
	}

	try {
		response = await doYouLoveMe (‘Frodo’)
		console.log (‘Frodo’, response)
	} catch (error) {
		console.error (‘Frodo’, error)
	}
}
~~~

Puedes advertir que lo primero que debemos hacer es insertar la palabra clave async antes de nuestra función asíncrona. Esto hará que la función esté envuelta en una promesa. Luego, hacemos que la respuesta se guarde en una variable. Es allí donde colocamos el await. En este caso, esta palabra clave está haciendo que el código espere a la resolución de la función doYouLoveMe.

Entonces, antes de ejecutar el console.log de la promesa original, debemos insertar algo como lo siguiente:

~~~
let response = await doYouLoveMe (‘Alberto’)
~~~

Esta línea de código reemplaza el método then de la promesa original.

A la práctica de lograr que el lenguaje haga cosas por nosotros usando ciertas palabras se le llama sugar syntax. En este caso, estamos haciendo sugar syntax porque utilizamos la palabra async para hacer que el lenguaje envuelva el contenido en una promesa de manera interna. Esta práctica nos quita muchos dolores de cabeza, pues soluciona los problemas que vienen con la asincronía. Uno de los mayores problemas que nos soluciona es el callback hell, creado por la anidación infinita de promesas o condicionales.