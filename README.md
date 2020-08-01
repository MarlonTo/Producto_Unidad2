# Producto_Unidad2
# Informe 
##  NODE-RED que implemente una interfaz HMI (Interfaz Humano Máquina) y  el Diseño una calculadora científica en Python

## 1.PLANTEAMIENTO DEL PROBLEMA



## 2.OBJETIVOS

### General:



### Específicos:




## 3.ESTADO DEL ARTE

### Tema: 

Investigadores: 

Año: 



Lugar: 

### Tema: 

Investigadores: 

Año:



Lugar: 
 
## 4.MARCO TEÓRICO



### ¿Qué es Python?

Python fue creado a finales de los ochenta por Guido van Rossum en el Centro para las Matemáticas y la Informática (CWI, Centrum Wiskunde & Informatica), en los Países Bajos, como un sucesor del lenguaje de programación ABC, capaz de manejar excepciones e interactuar con el sistema operativo Amoeba. El nombre del lenguaje proviene de la afición de un grupo británico de comediantes conocidos como Monty Python. (Python, n.d.)
Python es un lenguaje de programación interpretado el cual hace hincapié en la legibilidad de su código. Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional.
Este lenguaje está administrado por la Python Software Foundation. es una organización sin fines de lucro creada el 6 de marzo de 2001 dedicada al lenguaje de programación Python. Es responsable de varios procesos dentro de la comunidad, como el desarrollo de Python, la administración de los derechos intelectuales y de obtener fondos.(Operadores Python ➞ Explicamos Todos Los Operadores + Ejemplos Reales, n.d.)

![](IMG/2-25.jpg)

Los pasos para comenzar con Python en la programación de una interface de usuario no son terriblemente complejos, pero requiere que el usuario empiece a tomar algunas decisiones. Por su naturaleza como un lenguaje de programación de propósito general con intérpretes disponibles en todos los sistemas operativos comunes, Python tiene que ser bastante agnóstico en cuanto a las opciones que presenta para crear interfaces gráficas de usuario.
Afortunadamente, hay muchas opciones disponibles para los programadores que buscan crear una manera fácil para que los usuarios interactúen con sus programas. Existen enlaces para varios frameworks de interface de usuario en una variedad de plataformas, incluidas las nativas Windows, Mac y Linux, y muchas que funcionan en las tres.
En este punto, tiene que evaluar bien el hecho de necesitar una interface gráfica. Al momento de desarrollar una aplicación, también debe considerar una interface web, especialmente si cree que los usuarios puedan querer alojar su aplicación de forma remota, y proyectos como Django, Flask o Pyramid hacen que esto sea sencillo. Incluso puede usar una librería como pywebview para colocar una capa delgada alrededor de una aplicación web en una ventana GUI más nativa.



### RASPBERRY PI

Raspberry PI es una placa computadora (SBC) o Pc de placa única, de bajo precio, se podría expresar que es un ordenador de tamaño reducido, del orden de una tarjeta de crédito, desarrollado en el Reino Unido por la Fundación Raspberry PI (Universidad de Cambridge) en 2011, con el objetivo de estimular la enseñanza de la informática en las escuelas, aunque no empezó su comercialización hasta el año 2012. El concepto es el de un ordenador desnudo de todos los accesorios que se pueden eliminar sin que afecte al funcionamiento básico. Está formada por una placa que soporta varios componentes necesarios en un ordenador común y es capaz de comportarse como tal. A la Raspberry Pi la han definido como una maravilla en miniatura, que guarda en su interior un importante poder de cómputo en un tamaño muy reducido. Es capaz de realizar cosas extraordinarias(Yamanoor, Narasimha Saii,Yamanoor, 2013)

Los componentes de la Raspberry Pi son:

●	Un Chipset Broadcom BCM2835, que contiene un procesador central (CPU) ARM1176JZF-S a 700 MHz (el firmware incluye unos modos Turbo para que el usuario pueda hacerle overclock de hasta 1 GHz sin perder la garantía)

●	Un procesador gráfico (GPU) VideoCore IV

●	Un módulo de 512 MB de memoria RAM (aunque originalmente al ser lanzado eran 256 MB).

●	Un conector de RJ45 conectado a un integrado lan9512 -jzx de SMSC que nos proporciona conectividad a 10/100 Mbps

●	2 buses USB 2.0

●	Una Salida analógica de audio estéreo por Jack de 3.5 mm.

●	Salida digital de video + audio HDMI

●	Salida analógica de video RCA

●	Pines de entrada y salida de propósito general

●	Conector de alimentación microUSB

●	Lector de tarjetas SD

(Yamanoor, Narasimha Saii,Yamanoor, 2013)

### Puerto GPIO de la  RASPBERRY PI

La placa Raspberry Pi puede comunicarse con dispositivos externos a través del conector GPIO incorporado. En este conector hay pines de alimentación integrados (+5 y +3.3 V), tierra y pines de entrada / salida capaces de implementar diferentes protocolos.

Dado que existen dos versiones diferentes de hardware Raspberry Pi (rev. 1 y 2), las asignaciones de puertos también pueden variar. Sin entrar, en este momento, en los detalles de los protocolos, las dos posibles versiones de nuestra Raspberry Pi nos llevan a dos posibles escenarios de hardware. Podemos ver aquí un pin de diagrama comparativo de numeración GPIO.

#### Los pines GPIO tienen funciones específicas:

El color amarillo (2): Alimentación a 3.3V.

El color  rojo (2): Alimentación a 5V.

El color naranja (26): Pueden configurarse como entradas o salidas se las conoce tambien como pines de Proposito general.

El color gris (2): Son pines reservados.

El color negro (8): Conexión a GND.

El color azul (2): Comunicación mediante el protocolo I2C (Circuito inter-integrado).

El color verde (2): Destinados a conexión para UART para puerto serie convencional.

El color morado (5): Comunicación mediante el protocolo SPI (Es un protocolo síncrono, el cual sicroniza y la transmite datos  por medio de 4 señales).

 ![](IMG/esquema-pines-gpio.png)
 
 
## 5. LISTA DE COMPONENTES 






### Python 

Es un lenguaje de programación interpretado, que en su filosofía hace un hincapié en que el programador sea capaz de leer el código, compilarlo y comprenderlo de un manera sencilla y comprensible para el mismo, el lenguaje de programación es multiparadigma ya que soporta programación orientada objetos, programación imperativa y un poco de programación funcional. En esta ocasión para nuestra calculadora utilizaremos librerías de programación orientado a objetos. Su creador llamado Guido van Rossum en 1989 decidió crear “un lenguaje que sea fácil, intuitivo, potente y amigable para todos los programadores”, Python permite varios estilos de programación y además otros paradigmas, los cuales están soportados mediante el uso de extensiones.

Una vez obtenido nuestras dos herramientas procedemos a implementar en Visual Code a Python una vez realizado, nos acercamos el icono de extensiones de visual Code y nos descargaremos Magic Python, el cual, Es un paquete que permite resaltar ciertos aspectos en la sintaxis del código de programación por medio de diversos colores  permitiendo al programador identificar que se está realizando ya sean estructuras funciones importaciones entre otros.


 
## 6. MAPA DE VARIABLES


 


## 7. APORTACIONES





 
## 8. CONCLUSIONES



 
## 9. RECOMENDACIONES




 
## 10. CRONOGRAMA



 
## 11. BIBLIOGRAFÍA:


 
 
## 12. ANEXOS
