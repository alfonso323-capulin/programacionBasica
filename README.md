# programacionBasicaTIPOS DE DATOS BASICOS

En python los tipos de datos básicos se dividen en, números, como pueden ser 3 (entero ó integer) 1.75, (punto flotante ó float) 7+5j (complejos ó complex).

Para poder conocer el tipo de dato de una variable susaremos la instrucción "type()".

Otro tipo de dato basico en PYTHON son las cadenas de texto, por ejemplo, "Hola Mundo" (cadena de texto o string ó 'Hola Mundo' ó "Jenny's dog").

Como se puede notar a diferencia de muchos otros lenguajes en PYTHON no se declara el tipo de variable al crearla.

Para resumir en PYTHON se puede reprecentar números enteros, reales, y complejos. Los números enteros son aquellos números positívos o negatívos que no tienen desimales. En la mayor parte de las maquinas las variables enteras ("int") pueden almacrnar números de -2^31 a 2^31. En plataformas de 64 bites el rango es de -2^63 a 2^63.
Operadores:

		suma                    r=3+2
		resta	                r=4-7
            (guión) negación        r=-7
		multiplicación		r=2*6
		exponente		r=2**6
		división		r=3.5/2
		división entera		r=3.5//2
		modulo (residuo)	r=7%2

Un ejemplo de esto puede ser el siguiente:

    a=int(input('Incerta un numero '))   
    b=int(input('Incerta otro numero '))

    s=a+b   
    print('La suma es ' ,s)    
    r=b-a   
    print('La resta es ' ,r)    
    m=a*b   
    print('El producto es ' ,m)   
    d=a/b   
    print('El residuo es ' ,d)   
    dd=b/a
    print('El resultado es ' ,dd)    
    p=a**b   
    print('El resultado de "a" a la "b" es ' ,p)   
    import math    
    print('El logaritmo es ' ,math.log10(a))
###Ciclo For.
En pyhton "for" se utiliza como una forma genérica de interés sobre una secuencia, es decir, recorrer una secuencia.

            variable = secuencia  
            secuencia = ["uno", "dos", "tres"]  //estos son elementos
            for elemento in secuencia:
                print(elemento)                //4 esopacios 

Y los resultados serán:

           uno
           dos
           tres
    
El siclo "for" debe marcarse con un rango como se muestra de la siguiente manera:

    for temperatura in range(0,100,10):    //range es el rango y va el inicio, hasta
                                             donde quiero llegar y en este caso va de 10
    print(temperatura,'gC')                  en 10.

Un ejemplo del ciclo "for" puede ser el siguiente:

    for celcius in range(0,101,10):
        farenheit = (1.8*celcius)+32
        print(celcius,'gC','|',farenheit,'gF')
###Modulo Turlte 
Hay muchos módulos en python que proveen características poderosas que podemos usar en nuestros propios programas. Algunos de estos pueden enviar correos electrónicos y algunos de estos pueden extraer información de paginas de Internet. Para el manejo de gráficos usaremos un modulo que permite crear figuras y patrones. El modulo que se usara permiten desarrollar nuestro pensamiento computacional.

      
    import turtle
    ventana=turtle.Screen()	//Crea una ventana en blanco			
    alex=turtle.Turtle()	//Crear un objeto de la clase turtle lo puedo llamar como yo quiera se llama "alex" y puede tener atributos
    alex.forward(50)	//Avanza 50 unidades
    alex.left(90)		//gira a la izquierda 90°
    alex.forward(30)	//Avanza 30 unidades
    ventana.mainloop()	//Hasta que el usuario cierra la ventana el programa termina

Un ejemplo del modulo Turtle puede ser:

     import turtle
     ventana=turtle.Screen()
     alex=turtle.Turtle()
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     alex.left(90)
     alex.forward(100)
     ventana.mainloop()

Te aparecera una flecha, y no como tal una tortuga, pero si la quisieras ponlo de la siguiente manera:

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor('red')
    ventana.title("Hola")

    alex=turtle.Turtle()
    alex.shape("turtle")
    alex.color("blue")
    alex.pensize(10)
    alex.forward(100)
    alex.left(120)
    alex.forward(100)
    ventana.mainloop() 
###Funciónes 

Una función es un fragmento de código con un nombre asociado que realiza una serie de tareas y devuelve un valor. A demás de ayudarnos a programar y depurar dividiendo el programa en partes, las funciones también permiten reutilizar código.
     
	##definicion de una funcion
	def ladra():
	    print('guau, guau')
	##cuerpo principal del programa
	ladra()
Las Funciones ayudan al programador a dividir un problema en pequeñas piezas que pueden ser re usadas. También ayudan al programador a concentrarse en una pequeña parte del programa a la vez. Como resultado el escribir funciones es una parte importante del desarrollo del sofware. 

En nuestro caso debemos aprender a:

	1. Definir una función para usarla después.
	2. Pasar uno o más valores a una función.
	3. Desarrollar un cálculo complejo en una función.
	4. Regresar uno o más resultados a una función.
	5. Llamar a una función que previamente hayamos definido.

Puede también colocarce el Modulo Turtle con algunos de los ciclos, como se muestra este, con Ciclo For:

    import turtle
    def dibujar_cuadro(tur, d):
        for i in range(4):
            tur.forward(d)
            tur.left(90)
    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')
    rafa = turtle.Turtle()
    dona = turtle.Turtle()
    dibujar_cuadro(rafa, 50)
    dibujar_cuadro(dona, 200)
    ventana.mainloop()
###Programación Ambientada a Objetos.

Al principio del curso comentavamos que Python es un lenguaje multiparadigma en el que se podía trabajar con programación estructurada, como veniamos haciendo ahora o con programación orientada a objetos el cual es un paradigma de programación en el que los conceptos del mundo real relevantes para nuestro problema se modelan a travéz de clases y objetos, y en el que nuestro programa consiste en una serie de interacciones entre objetos.

>OBJETOS:

>Un objetos es una entidad que agrupa un estado y una funcionalidad relacionada. El estado del objeto se define a través de variables llamadas atributos, mientras que la funcionalidad de modela a través de funciones a las que se les conoce con el nombre de MÉTODOS DEL OBJETOS.

>**Diagrama UML sirve para definir un objeto y culales son su métodos y sus atributos**

>Un ejemplo de objeto podría ser un coche en el que tendriamos Atributos como: la marca, el numero de puertas, o el color.

>Y Métodos como: arrancar, parar.

>O bien cualquier otra combinación de Atributos y Métodos según lo que fuera relevante para nuestro programa.

>CLASES:

>Una clase no es más que una plantilla genérica de la cual insancia los objetos; es la plantilla que define que Atributos y Métodos tendrán los objetos de esa clase.

En PYTHON las clases de definen Mediante la palabra clave "CLASS" seguido del nombre de la clase, seguido por dos puntos, y a continicación, inentado el cuerpo de la clase.

Por ejemplo:

    class Coche(object):
        def __init__(self,gasolina):
            self.gasolina = gasolina
        def arrancar(self):
            if self.gasolina > 0:
                print('Arranca')
            else:
                print('No Arranca')
        def conducir(self):
            if self.gasolina > 0:
                self.gasolina = self.gasolina - 1
                print('Quedan ', self.gasolina,' litros')
            else:
                print('No se mueve')
    vocho = Coche(5)
    tsuru = Coche(3)

    vocho.arrancar()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir()
    vocho.conducir() 
>REALIZA UN PROGRAMA QUE LE DIGA AL USUARIO EL NUMERO DE DIAS, HORAS, MINUTOS Y SEGUNDOS, EL PREOGRAMA DEBE CALCULAR Y DESPLEGAR EL NUMERO DE SEGUNDOS TOTALES

    print('Llene los siguientes datos.')

        d=float(input('Cuantos dias '))
        h=float(input('Cuantas horas '))
        m=float(input('Cuantos minutos '))
        s=float(input('Cuantos segundos '))
        t=s+(m*60)+(h*3600)+(d*86400)
        print('El tiempo en segundos es',t)

#Ejercicios:
>**Ejercicio 1:**

    import turtle

    def dibujar_cuadro_seguir(tur, p):
        for i in range(4):
            tur.forward(20)
            tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor('blue')
    ventana.title('funciones')
    gabby=turtle.Turtle()
    gabby.pensize(5)
    gabby.speed(2)

    p=30

>**Ejercicio 2**

    a=input('Escoje un color de los siguientes para la ventana: brown chocolate coral red pink purple blue green yellow black :  ')

    b=input('Escoje un color de los siguientes para la tortuga 1: brown chocolate coral red pink purple blue green yellow black :  ')

    c=input('Escoje un color de los siguientes para la tortuga 2: brown chocolate coral red pink purple blue green yellow black :  ')

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor(a)
    ventana.title("Hola, Kary bebe")

    gabby=turtle.Turtle()
    gabby.shape("turtle")
    gabby.color(b)
    gabby.pensize(5)

    gabby.forward(100)
    gabby.left(120)
    gabby.forward(100)
    gabby.left(120)
    gabby.forward(100)
    gabby.left(120)
    gabby.forward(100)

    gabs=turtle.Turtle()
    gabs.shape("turtle")
    gabs.color(c)
    gabs.pensize(5)

    gabs.forward(100)
    gabs.left(-120)
    gabs.forward(100)
    gabs.left(-120)
    gabs.forward(100)
    gabs.left(-120)
    gabs.forward(100)

    ventana.mainloop() 

>**Ejercicio 3***

    import turtle
    ventana=turtle.Screen()
    ventana.bgcolor("black")
    ventana.title("Hola, Kary bebe")

    diego=turtle.Turtle()
    xime=turtle.Turtle()

    diego.shape("turtle")
    diego.color("green")
    diego.pensize(2)

    xime.shape("turtle")
    xime.color("red")
    xime.pensize(2)

    xime.speed(9)
    xime.speed(10)

    diego.penup()
    xime.penup()
    diego.setpos(0,-50)
    diego.pendown()
    diego.circle(50)
    xime.setpos(0,-100)
    xime.pendown()
    xime.circle(100)

    ventana.mainloop()

>**Ejercicio 4**

    import turtle
    a=int(input('Introdizca el numero de circulos que desea:'))

    ventana = turtle.Screen ()
    ventana.bgcolor("black")
    ventana.title("Hola Kary bebe")

    kary = turtle.Turtle()
    kary.shape("turtle")
    kary.color ("green")
    kary.pensize (2)

    kary.speed(8)

    for i in range(a):
  
      kary.penup()
      kary.setpos(0,-(i*10))
      kary.pendown()
      kary.circle(i*10)
  
    ventana.mainloop()

>**Ejercicio 5**

    import turtle
    ventana=turtle.Screen()
    ventana.setup(1000, 500)
    ventana.tracer(0)
    ventana.addshape("mario.gif")

    mario=turtle.Turtle()
    mario.speed(0)
    mario.shape("mario.gif")

    mario.penup()
    mario.goto(-500, 0)

    while True:
        ventana.update()
        mario.forward(.5)

>**Ejercicio 6**

    import turtle

    window= turtle.Screen()
    window.addshape("mario.gif")
    border= turtle.Turtle()

    border.speed(0)
    border.up()
    border.hideturtle()
    border.pensize(0)
    border.color('white')
    border.goto(500,500)
    border.down()
    border.goto(500,-500)
    border.goto(-500,-500)
    border.goto(-500,500)
    border.goto(500,500)


    camino=turtle.Turtle()
    camino.speed(0)
    camino.shape("mario.gif")

    camino.up()
    dx=1

    while True:
        x,y= camino.position()
        if x+dx>=500 or x+dx<=-500:
            dx=-dx
   
        camino.goto(x+dx,y)


    window.mainloop()

>**Ejercicio 7**

    class Triangulo(object):
        def __init__(self,angulo1,angulo2,angulo3):
            self.angulo1 = angulo1
            self.angulo2 = angulo2
            self.angulo3 = angulo3

        def ChecarAngulo(self):

            if self.angulo1+self.angulo2+self.angulo3 == 180:
                print('Es un triangulo')

            else:
                print('No es un triangulo')

    miTriangulo=Triangulo(90,30,60)

    miTriangulo.ChecarAngulo()

>**Ejercicio 8**

    class Cancion(object):
        def __init__(self,letra):
            self.letra = letra
    
        def cantame(self):
            print(self.letra)

    micumpleanos=Cancion(["...que cantaba el rey David," " hoy por ser dia de tu santo," " te las cantamos a ti."])

    micumpleanos.cantame()}

>**Ejercicio 9**

    import turtle

    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')

    omar = turtle.Turtle()
    d = 50

    for i in range(4):
        gabby.forward(d)
        gabby.left(90)

    ventana.mainloop()

>**Ejercicio 10**

    import turtle

    def dibujar_cuadro(tur, d):

        for i in range(4):
            tur.forward(d)
            tur.left(90)

    ventana=turtle.Screen()
    ventana.bgcolor('green')
    ventana.title('Funciones')

    diego = turtle.Turtle()
    gabby = turtle.Turtle()
    dibujar_cuadro(gabby, 200)

    ventana.mainloop()
