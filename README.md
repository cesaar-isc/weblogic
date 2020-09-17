# Como levantar un proyecto en weblogic con spring 5 
Uno de los principales problemas al desarrollar para un servidor de aplicaciones de weblogic es el la configuración si bien es cierto no causa problemas cuando estas trabajando con una version antigua de spring (3 o menos), pero el problema viene cuando estamos trabajando con una versión actual.

Si notamos al momento de intentar levantar nuestro proyecto marcan demasiados errores y muchas veces los foros no dicen la respuesta muy clara,

## ¿Qué es lo que pasa?
Internamente weblogic tiene sus propias dependencias, estas son las que encuentra primero al momento del despliegue, y por lo tanto toma esas e ignora las que definimos en nuestro jar o war.

## ¿Como solucionarlo?
La solución es muy sencilla, basta con crear un archivo xml de configuración de weblogic y excluir las dependencias propias del servidor.
