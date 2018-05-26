# Guía de sintaxis Markdown

Markdown es un lenguaje de marcado que tiene como objetivo el hacer más fácil la tarea de dar formato a un texto mediante el uso de algunos caracteres.

## Encabezados ##
Existen hasta seis niveles y para generarlos se agrega # al comienzo de una palabra o frase seguido de un espacio por ejemplo:

# Encabezado 1 (h1 con 1 #) 
## Encabezado 2 (h2 con 2 #) 
### Encabezado 3 (h3 con 3 #)
#### Encabezado 4 (h4 con 4 #)
##### Encabezado 5 (h5 con 5 #)
###### Encabezado 6 (h6 con 6 #)

Se puede encerrar cada encabezado entre almohadillas, por motivos puramente estéticos, porque no es necesario en absoluto, es decir, se puede hacer esto:

### Esto es un encabezado H3 ###

## Citas ##

Para agregar citas a un texto se utiliza el signo > por ejemplo:

> Esto es una cita y tiene
> continuación 

## Listas
### Desordenadas
Para agregar elementos a una lista desordenada se hace uso de un guion (-) seguido de un espacio con el texto. Algunas aplicaciones acpetaran tambien asterisco (*) o un signo de más (+).

- Elemento 1
* Elemento 2
+ Elemento 3

### Numeradas

Para agregar elementos a una lista numerada se agrega un número (1, 2, 3...) seguido de un punto (.) y un espacio por ejemplo:

1. Elemento 1
2. Elemento 2
3. Elemento 3

Se puede anidar una lista con otra usando un espacio y presionando la tecla tabulador:

1. Elemento padre
    - Elemento hijo

## Separaciones
Para agregar una separación basta con usar tres guiones bajos y markdown lo interpretará cómo si fuera una etiqueta HR.
___

## Textos

### Negritas y cursivas

Markdown admite dos maneras de crear estos estilos, mediante asteriscos (*) o mediante guiones bajos (_). Si se agrega un * o _ al inicio y al final del texto éste tendra el estilo cursiva. Si se agrega 2 * o 2 _ al inicio y al final del texto éste se resaltará.
Para agregar ambos estilos se usa tres asteriscos o tres guiones bajos al inicio y fin del texto.
 si se agrega Se recomienda utilizar *.

 Por ejemplo:

***Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas gravida dui at urna facilisis laoreet. Ut vitae magna dui. Cras sollicitudin nisi non mauris imperdiet placerat.***

##Enlaces

Para agregar enlaces basta con agregar entre corchetes un texto que será el ancla seguido de parentesis con la url del enlace, se puede añadir información extra para el title después del enlace con un texto entre comillas("Title").

`[Introducción a python](https://www.python.org/ "Python")`

Tiene como resultado: [Introducción a python](https://www.python.org/ "Python")

Si se requiere que la url sea el propio enlace basta con incluirla entre los signos < y > y el resultado será el siguiente: <https://www.python.org/> 

##Imagenes

Las imagenes se añaden de una manera similar que los enlaces solo que se agrega un signo de exclamación al inicio para que sea interpretado como código de insertar imagene.

`![Markdown](http://www.analiticaweb.es/wp-content/uploads/2017/02/markdown.jpg)`

![Markdown Logo](https://camo.githubusercontent.com/b9381e0c689f1d541ac5179d599739b0f01012db/687474703a2f2f6269742e646f2f686f772d746f2d6d61726b646f776e)


## Código
Permite agregar documentación técnica con fragmentos de código.

Si solo se incluira un frase o palabra basta con iniciarla con cuatro espacios en blanco:

    Esto es código

Pero si se necesita agregar más código basta con hacer uso de tres virgulillas(~) arriba y tres abajo.

~~~
lista = [1, 2, 3]
for m in lista:
    print(m)
~~~

Si se desea resaltar código dentro de una frase se hace uso de dos acentos graves(``), por ejemplo:

También puedo usar `código` aquí.

## Anular Markdown

Para anular los simbolos de markdown se antepone un \ antes del signo que se desea usar o escapar, por ejemplo:

    De esta forma anulas el \*markdown*.

Tiene como resultado:
> De esta forma anulas el \*markdown*.
