# gtasa:tips
Recomendaciones y sugerencias sobre como armar un GTA Moddeado y no morir en el intento.

**DESCARGO DE RESPONSABILIDAD**: Esta guía de recomendaciones se hizo como traducción en base al post de "primeros pasos" del blog brasilero [MixMods](https://www.mixmods.com.br), **TODOS LOS CRÉDITOS CORRESPONDIENTES RECAEN A SU AUTOR ORIGINAL**: Junior_djjr.

# Introducción
Bienvenidos a GTA SA: Tips, un apartado en donde mostramos recomendaciones y sugerencias para adentrarse en el modding del GTA:SA y que tu juego no crashee en el intento, ¡empezamos!

# 1 - LO QUE NECESITAS.

## 1.1 - Tener un buen GTA, fuera de "Archivos de Programa"

## 1.1.1 - ¿Que es un "buen GTA"?
Empezaremos desde cero, con una instalación **vanilla** (vanilla = sin modificaciones) del GTA:SA, si el GTA será usado *solamente para SA-MP*, es recomendable bajarse una versión RIP del juego debido a que no usaremos gran parte de los audios del mismo, como por ejemplo: diálogos de personajes y las emisoras del juego.

**NO es recomendable** bajarse GTA's pre-modificados (Los famosos GTA's de personajes que están jodidamente sobrevalorados, como Street, Doomer, TutosMarcosIsrael, Th3C3z4r y cualquier otro pelotudo mongólico mexicano de youtube por ejemplo), debido a que pueden existir conflictos o problemas que pueden derivar en crasheos o mal funcionamiento del GTA, por ende, es **mucho mejor** que lo modifiques por tus propios medios, así aprendes y modificas el GTA a tu propio gusto visual.

## 1.1.2 - Fuera de "Archivos de Programa"?
Windows a veces puede bloquear las alteraciones de los archivos encontrados dentro de la carpeta de **"Archivos de Programa"** , por lo tanto, si quieres modificar los archivos del mismo, **nunca** instales el GTA en esta ruta.

Si desactivas el UAC *(Control de cuentas de usuario)* y quitas las restricciones de edición de la carpeta, se puede resolver este inconveniente, pero es menos problemático instalarlo en otra ubicación (en la raíz del disco local por ejemplo).

## 1.1.3 - Backup/Respaldo del GTA.
Un buen consejo es mantener una copia del GTA sin modificaiones, en dado caso de necesitar un respaldo de cualquier cosa, si te quieres ahorrar tu preciado espacios en el disco, borra la carpeta Audio de tu GTA de respaldo *(irónico que lo que más pesa que son los audios es lo que menos se cambia en el juego).*

# 1.2 - Un buen PC para modificar nuestro GTA.

## 1.2.1 - Microsoft Windows *(nuestro sistema operativo)*
Básicamente, cualquier Windows está bien para armar nuestro GTA, excepto Windows XP *(¿quien lo usa en 2020?)*, debido a que como ya dejó de tener soporte, los **.asi** modernos pueden no funcionar en este *(Recordemos que los .asi son librerías, las cuales están escritas en **C++**).*

La gran mayoría de personas usan Windows 10 sin problemas, hay reportes de que hay personas que tienen fallas con el juego, esto se puede resolver colocando el juego en *modo de compatibilidad para Windows 98.*

Además, desactivar el UAC y el DEP es una buena idea, no será un problema si no eres lo suficientemente tonto como para caer con virus. Hay mods para desactivar el DEP para el GTA:SA.

También hay un problema relacionado al Windows en el cual el juego se ejecuta, pero no muestra nada en pantalla ni da mensajes de error, simplemente aparece ejecutandose de fondo y consumiendo del procesador (visible con el administrador de tareas), esto se resuelve usando un mod para desactivar el *rundll32.exe*

Descarga: [runDLL32 Fix](http://sharemods.com/3fepnakiq7i2/RunDLL32.exe_Fix__corrigir_jogo_n__o_abrindo_.7z.html)

## 1.2.2 - Prepárate.
Cuando ustéd tenga un PC nuevo recien formateado, tu **NECESITAS** tener los redistributables, especificamente los **Visual C++**, esto corregirá cualquier problema que puedas tener con algún .asi, además de que varios juegos te piden tener instalados los redistributables de C++.

Así como el **DirectX End-User Web Installer**, esto corregirá problemas con varios mods que dependan de apartados gráficos *(DirectX)*, como ENB's, reshaders etc. Windows generalmente viene de fábrica con DirectX antíguos, así que por lo tanto esto también resolverá problemas al jugar juegos antiguos.

Descargas: [Visual C++ y DirectX Web-Installer](https://www.mixmods.com.br/2015/08/download-baixar-dll-microsoft-visual-directx9.html)

# 1.3 - Ejecutable del GTA:SA
El archivo .exe versión **1.0 US Hoodlum** o **1.0 US Compact** son los mas utilizados a la hora de modificar el GTA:SA, básicamente todos los mods fueron creados para estos .exe, en especial para el Hoodlum.

Para saber si tu tienes alguno de estos .exe, vaya a su carpeta de instalación del GTA, y presione click derecho sobre el ejecutable del GTA:SA, presione en propiedades, en "Tamaño", cetifiquese que su .exe tenga exactamente **"14.383.616 bytes" (Hoodlum)** o **"5.189.632 bytes" (Compact)**. Si no tienes alguno de esos .exe, es recomendable que los descargues si quieres tener la máxima compatibilidad posible con mods.

El ejecutable de **Compact** es una recopilación hecha por un modder, el cual deja un .exe muchísimo menor en tamaño. También funciona mejor en windows nuevos, por ejemplo, en Windows 7 no arroja el error relacionado con el Tema Aero, aunque hay algunos pocos mods que no funcionaran con el .exe de Compact.

Esto, con lo que fue explicado en el punto 1.1.2 - "Fuera de Archivos de Programa", corregirá el error **"UNKNOWN GAME"** y **"this game is not supported"** de Modloader (así como otros errores de otros mods que requieran escritura constante de archivos).

Descargas:
[gta_sa.exe US 1.0 Hoodlum](https://miscellaneous-c.blogspot.com/2016/04/crack-gta-sa-v10-us-hoodlum-no-cd-fixed.html)
[gta_sa.exe US 1.0 Compact](https://miscellaneous-c.blogspot.com/2016/04/crack-gta-sa-v10-us-hoodlum-no-cd-fixed.html)

# 1.4 - ASI Loader, CLEO y Moonloader

## 1.4.1 - Silent's ASI Loader
Es el encargado de manejar los archivos .asi, que básicamente son .dll renombrados. Es el primer paso para modificar tu GTA.

Es mejor que existe hasta el día de hoy y viene integrado con el Instalador de la Biblioteca CLEO, pero al sol de hoy, el ASI Loader del instalador CLEO está desactualizado, es recomendado instalar el ASI Loader LUEGO de instalar la Biblioteca CLEO, puedes descargar la versión actualizada del ASI Loader desde los links de abajo.

## 1.4.2 Biblioteca CLEO
La muy famosa Biblioteca CLEO (erroneamente llamada Librería CLEO), es un mod que permite la instalación de archivos cleo, los mods de script/código más comunes del GTA.

## 1.4.3 Moonloader
Moonloader llega como un sustituto para la Biblioteca CLEO, ahora utilizando lenguaje .lua para la creación de mods de script, haciendo que la creación de mods sea más poderosa.

Descargas: [Librería CLEO 4](http://mixmods.com.br/2014/02/Livraria-CLEO.html)
[Silent's ASI Loader](http://mixmods.com.br/2013/02/silent-asi-loader.html)
[MoonLoader](https://www.mixmods.com.br/2017/08/MoonLoader.html) - En fase beta, puede haber problemas y no es necesario por ahora su uso.

# 1.5 - Smart Process
El autor original (Junior_djjr), recomienda el uso de Smart Process cuando estés usando tu GTA, básicamente es un programa con el cual puedes hacer un cierre forzado de cualquier programa con solo pulsar un botón, mas información en el post original sobre el programa: [Smart Process](https://www.mixmods.com.br/2015/05/software-smart-process-20.html).

# 2 - MODS RECOMENDADOS PARA UN BUEN GTA.

## 2.1 - Modloader (En serio, ¿quien no usa esto hoy en día?)
Pues bueno, ya tienes un GTA listo para usar con mods, más que tal un mod que te ayude a instalar/desinstalar los mods?, ¡Eso es **Modloader**!

¿Y eso que es?: Modloader es un .asi creado por LINK/2012, que consiste en un mod que carga otros mods sin sustituir ningún archivo. Todo lo que tienes que hacer es simplemente colocar el mod en la carpeta del Modloader y este automáticamente será cargado a tu GTA, si no lo quieres más, solamente remueve el mod fuera de la carpeta del Modloader (o indicarle al Modloader que no quieres cargar ese mod).

¿Por qué usarlo?: Tu nunca necesitarás hacer backup de cosas, tu GTA núnca se verá afectado por lo que fué instalado, los mods estarán solamente siendo cargados al GTA sin sustituir absolutamente ningún archivo de tu juego, si tu GTA da algún problema, solo basta con sacar los archivos fuera de la carpeta del Modloader y presto!, su mod ha sido desinstalado!. E inclusive puedes instalar mods en caliente (Instalar mods sin necesidad de salir del juego).

Descargas:
[Modloader](http://mixmods.com.br/2015/01/SA-Modloader.html)

**NOTA**: El mismo autor tiene en su blog una [Guía de como usar Modloader](https://www.mixmods.com.br/2015/07/tutorial-dicas-tudo-sobre-mod-loader.html), para que aprendas funciones básicas y avanzadas sobre este mod del GTA. Pues, pasarás meses y años usando Modloader en tu juego, ¿por qué no vas y le echas un vistazo?.

## 2.1 - Silentpatch
Silentpatch es un mod no-oficial que corrige centenares de bugs del juego, cosas que Rockstar no pudo corregir a la hora del lanzamiento del juego, las correcciones de las versiones superiores del GTA, Silentpatch las trae para la 1.0.

Sean bugs grandes o grandes, desde mejoras de rendimiento hasta bugs visuales y correcciones de crasheos.

Es simplemente indispensable, originalmente sin este mod el juego tendrá un performance inferior y pueden haber problemas con el mouse, todo será corregido con este mod. 

Descargas:
[Silentpatch](http://mixmods.com.br/2015/03/SilentPatch.html)

## 2.3 - Open Limit Adjuster
Es común que hayan que aumentar algunos límites del juego para añadir nuevos mods. Normalmente, mods que adicionan nuevos objetos, coches, armas, peatones, luces, o simplemente más tareas para peatones, uso de memoria, etc.

**Open Limit Adjuster** tiene una diferencia, el ajusta los límites automáticamente conforme sea necesario, así que no es necesario configurar, solo instalar y listo!

Uno de los famosos bugs que corrige es el de los objetos parpadeantes y el mapa que no carga como es debido.

Descargas:
[Open Limit Adjuster](https://www.mixmods.com.br/2014/09/iiivcsa-open-limit-adjuster.html)

## 2.4 - MixSets
Este es un mod totalmente programado por el creador original de esta guía en portugues (Junior_djjr), que te da centenas de correcciones y mejoras configurables.

Es muy similar a SilentPatch, más enfocado en tweaks (pequeñas configuraciones para mejorar la experiencia), o sea, un mod enfocado en mejorar el funcionamiento del juego, mientras que SilentPatch se enfoca en reparar bugs.

Posee varias excelentes configuraciones para el gameplay, incluyendo varios ajustes de la distancia de visión, que deja el juego mucho más agradable para PC's modernas (Limitar el juego a 60 FPS, poder colocar más coches y peatones, etc.)

Es tambien excelente para aumentar los FPS del juego, con configuraciones que aumenta la prioridad de su CPU, y disminuir o remover detalles gráficos (Tales como el polvo), que ayudan a corregir el lag de tu GTA.

Es casi un paquete de mods, donde todo es configurable y puedes activar/desactivar funciones mediante el archivo .ini, por lo tanto no existe eso de que "MixSets es incompatible con X mod", si ves alguna incompatibilidad, solo debes desactivar esa función del .ini, no existe motivo aparente para no usar este mod.

Descargas:

[MixSets](https://www.mixmods.com.br/2019/08/mod-mixsets.html)

## 2.5 - Widescreen Fix
GTA SA no fue hecho para nuestras PC de hoy en día, todos lo saben ... Como en el caso de nuestros monitores de pantalla ancha (pantalla ancha, que casi todos usan hoy).

GTA SA en un monitor de pantalla ancha se estira, con el radar ovalado y la luna, etc. Además de toda profundidad 3D se muestra de manera incorrecta, este mod soluciona los problemas de los monitores de pantalla ancha y prácticamente no se puede jugar sin el, el mod hace un cambio increíble en la pantalla y hace que el juego sea mucho más agradable a la hora de jugar.

Descargas:
[Widescreen Fix](https://www.mixmods.com.br/2016/06/widescreen-fix-para-gta-sa-corrigir.html)

## 2.6 - Framerate Vigilante
El GTA:SA originalmente fue hecho para jugar en 30 FPS,en el caso de que tu juegues con FPS altos (o  bajos), como 60 FPS, tu juego presentará varios bugs.

Este mod tiene como objetivo corregir esos problemas!

Descargas:
[Framerate Vigilante](https://www.mixmods.com.br/2019/06/framerate-vigilante.html)

## 2.7 - Mover la carpeta de User Files.
En dados casos puede ser bastante común tener varias instalaciones del mismo juego, como una para modificar, otra para respaldos, otra para una conversión total, etc.

**portablegta.asi** es un mod que altera la carpeta "GTA San Andreas User Files", creando una carpeta "userfiles" dentro del mismo directorio en donde tienes el juego instalado, algo así como una instalación portatil.

Así puedes tener diferentes instalaciones con diverentes partidas guardadas, configuraciones, fotos, replays, etc. Lea la publicación completa a la hora de descargar para entender más usos de este mod.

Descargas:
[portablegta](https://www.mixmods.com.br/2018/07/portablegta-change-saves-folder.html)
