###INTRODUCCIÓN

A raíz de la reciente Bitbitjam que se hizo en Junio y gracias a una de las entradas del concurso, tomé conciencia de que existía 'algo' con el que poder programar la Game Boy (conocida por cierto en su fase prototipo como DMG o Dot Matrix Game). Como el código fuente estaba disponible, me animé a darle un vistazo esperando que fuera en terrible ensamblador pero para mi sorpresa... ¡estaba en el amigable y sencillo C! Buscando información encontré que este juego se había escrito usando el GameBoy Developer's Kit (GBDK) de Michael Hope. 

Este kit se compone de:

    Un compilador ANSI C.
    Un ensamblador.
    Un optimizador.
    Un linker para producir las roms de GameBoy.
    Soporte de multiples bancos de memoria.
    Un juego de librerias en ensamblador, incluido su fuente.
    Ejemplos en C y ensamblador.

La puñeta es que este kit no se actualiza desde el 2001... una pena porque funciona realmente bien y solo se le hecha en falta algunos detallitos para ser perfecto, así que toca conformarse con lo que hay que no es poco. Estos tutoriales se van a centrar en la consola original, pero eso no quita que este kit soporte también la GB COLOR y en algún tutorial se enseñará a darle soporte.

###REQUISITOS

Vamos a distinguir requisitos de hardware, software y de conocimientos.

Evidentemente necesitaremos un ordenador PC, no hace falta que sea moderno. Para probar las roms sería interesante tener una GAMEBOY y un cartucho flash para quemar las roms. Como consola recomiendo la GB COLOR porque es la que mejor pantalla tiene aunque, por otro lado, es fácil de encontrar un clon chino llamado GB BOY COLOR, que además de incluir 66 juegos en memoria, su pantalla en retroiluminada y sale por unos 23 € en casa, en EBAY las tenéis. 

[![GameboyAreAwesome - GB BOY COLOUR Unboxing](https://cloud.githubusercontent.com/assets/48375/11446366/0b6a751c-9536-11e5-83f8-2ed612949758.png)](http://www.youtube.com/watch?v=b7X4LTEchos "GameboyAreAwesome - GB BOY COLOUR Unboxing")


Como flash recomiendo el aparecido este año 2014, [EVERDRIVE de Krizz](http://krikzz.com/index.php?route=product/product&product_id=60), una autentica maravilla de cacharrito y que [lo podeis comprar en España](http://www.videojuegoshoracio.com/).

El kit y herramientas que usaremos en los tutoriales funcionan sobre Windows, yo voy a trabajar sobre XP virtualizado. ¿Eso que es? Pues si sois usuarios de Linux, OSX o cosas más extrañas aún, podéis usar un programa gratuito llamado Virtualbox, que os permitirá 'emular' un sistema operativo sobre otro. Aquí os dejo un video de como instalarlo:

[![Instalar Windows XP paso a paso en VirtualBox](https://cloud.githubusercontent.com/assets/48375/11446365/0b65120c-9536-11e5-9554-be539230d755.png)](http://www.youtube.com/watch?v=-jFU-Zq7G1E "Instalar Windows XP paso a paso en VirtualBox")

###CONOCIMIENTOS 

Tema espinoso, en principio debéis saber lenguaje C. Tampoco es que tengáis un nivel de maestro informático a lo Carmack, con saber lo que es una variable, constante, función, instrucciones lógicas como IF, FOR, WHILE... bastaría. Es de los lenguajes más sencillos que hay y se usa como introducción a la programación, así que nunca está de más aprenderlo. Os dejo [otro tutorial](http://www.elrincondelc.com/cursoc/cursoc.html) para que le deis un vistazo, en serio, no es difícil.

En la carpeta DOC del paquete del kit que os pongo en el siguiente apartado, hay varios textos, incluidos el oficial de Nintendo de 300 páginas, pero en concreto os recomiendo el pandocs.txt que seria interesante que lo imprimieseis para tenerlo a mano.

###ENLACES INTERESANTES

Podemos encontrar más tutoriales sobre GB en varios sitios de la red:

- [Tutoriales de Darkryoga sobre GBDK en C](http://www.elotrolado.net/hilo_desarrollo-software-proyectos-de-darkryoga_1901847_s100)


- [Tutoriales de xzakox en ensamblador](http://wiki.ladecadence.net/doku.php?id=tutorial_de_ensamblador)


- [Ejemplos de GBDK en C de Retroisle](http://www.retroisle.com/others/nintendogameboy/Technical/Firmware/dev.php)



###INDICE DE LOS TUTORIALES

En principio, el plan de capítulos será el siguiente:

1. Hola Mundo
2. Controles
3. Sprites
4. Backgrounds (I)
5. Backgrounds (II)
6. Sonido
7. Juego ejemplo (I)
8. Juego ejemplo (II)


[Vídeo grabado del taller de GB del RetroConsolas Alicante](http://vertice.cpd.ua.es/126068 )

El material en PDF lo tenéis [aquí](http://tinyurl.com/o4eesw6) 