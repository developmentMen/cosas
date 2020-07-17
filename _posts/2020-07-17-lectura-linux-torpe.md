---
layout: post
title: Lectura|> linux para torpes 01
date: 2020-07-17 02:30
author: developmentMen
tags: curso linux novatos brutos extremadamente torpes pdf
---
<hr>
Este post es lo que me resulto interesante de la lectura del siguiente libro:
<br>
[curso de Linux para novatos, brutos y extremadamente torpes](https://educasitio.com/files/Curso%20de%20Linux%20para%20novatos%2C%20brutos%20y%20extremadamente%20torpes.pdf)
<br>
<hr>
<div style="text-align: center;">
<img src="https://bbvaopen4u.com/sites/default/files/styles/big-image/public/img/new/bbva-open4u-herramientas-linux_1.jpg?itok=aUf6Y7yg">
</div>
<br>
Luego de explicar mas o menos la historia de linux, algunas distribuciones y valores del software libre empieza diciendo que la mayoria de sistemas `linux` son _Case Sensitivity_, es decir no es lo mismo un comando en mayusculas que uno en minusculas en el libro da el ejemplo del comando **echo hola**:
<br>
<img src="img/echo.png">
<br>
	comando **echo**:
		este comando imprime lo que le demos en pantalla (en este caso le mandamos "hola")
Como se puede ver la salida es diferente si el comando este en mayuscula que en minusculas.
<br>
<h1 style="text-align: center; text-decoration: underline;">Variables</h1>
Dentro de la misma terminal tenemos algo llamado **variables de entorno** que como cualquier lenguaje de programacion una variable almacena informacion y de define de la siguiente manera
<br>
`VARIABLE=valor_de_la_variable`
<br>
y podemos consultarla de la siguiente manera:
<br>
`echo $VARIABLE`
<br>
Ejemplo grafico:
<img src="img/variable.png">
<br>
de momento no se entra en detalle sobre estos comandos pero se señala unas **variables definidas**  y comenta 3 que se consideran importantes :
	$PATH
	$PS1
	$PS2

<h1 style="text-align: center; text-decoration: underline;">Comandos</h1>
Un comando es generalmente un fichero ejecutable que se encuentra en el sistema, la variable $PATH contiene una lista de caminos de busqueda, Para verlo usamos:
<br>
`echo $PATH`
<br>
<img src="img/echoP.png">
<hr>
Bueno eso fue un resumen de lo que me llamo la atencion sobre el libro, les invito a leerlo y aprender mas sobre este comodo sistema operativo, si queres que trate algun tema dejamelo en los comentarios que los voy a estar leyendo, tambien podes dejarme una donacion <3, los quiero nos vemos en otro post
<hr>
<h1 style="text-align: center; size: 200%">~Fin~</h1>