---
layout: post
title: Lectura|> linux para torpes 02
date: 2020-07-23 20:30
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
	<h1>Musica para leer</h1>
	<iframe width="100%" height="300" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/465546846&color=%23c9bdd3&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true&visual=true"></iframe><div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;"><a href="https://soundcloud.com/lofi-hip-hop-music" title="Hip Hop" target="_blank" style="color: #cccccc; text-decoration: none;">Hip Hop</a> · <a href="https://soundcloud.com/lofi-hip-hop-music/lofi-hip-hop" title="Lofi" target="_blank" style="color: #cccccc; text-decoration: none;">Lofi</a></div>
	<img src="https://bbvaopen4u.com/sites/default/files/styles/big-image/public/img/new/bbva-open4u-herramientas-linux_1.jpg?itok=aUf6Y7yg">
</div>

<h1 style="text-align: center;">Linea de comandos</h1>
Bueno siguiendo con este libro nos habla sobre __el interprete del comandos__, tambien conocido como bash o shell. Existen varios tipos distintos de interpretes que funcionan de manera distinta y cumplen distintas funciones como por ejemplo:
´Korn-Shell (ksh)
Bourne-Shell (sh)
C-Shell (csh)
remote-Shell (rsh)
La Secure Shell (Ssh)
Bourne-Again SHell (bash).´

Para saber que shell está usando usted haga lo siguiente:
<div style="text-align: center;">
	<img src="img/shell.png">
</div>
nos tiene que aparecer "bash" o "shell" aparece otra cosa tecleamos **sh** o **bash**
	`"Una Shell no es solo un interprete de comandos. Una Shell es sobre todo un interprete de un potente
lenguaje."`
<br>
resulta que esto del interprete de comando es todo un mundo pero que es un comando?. Pues un comando es un fichero ejecutable agregado a la variable de entorno PATH, vamos a hablar sobre algunos comando:
<br>
si en algun momento queremos parar un comando en ejecucion apretamos **crtl + c**
<br>
para poder obtener __ayuda__ sobre algun comando tenemos que ejecutar el comando seguido de **-help**
<br>

<h2 style="text-align: center;">concepto importantes</h2><br>
<img src="img/conshell.png">
** Palbras reservadas: **
`case, do, done, elif, else, esac, fi, for, function, if, in, select, then, until, while, time.`<br>
** Comandos internos: **
No necesitan PATH
` cd, exec, arg, eval, exit,... `

<h2 style="text-align: center;">ejemplos</h2>
comando solo: <br> `$ ls`<br>
comando sin opciones con tres argumentos: <br> `$ ls . / ..`<br>
comando con tres opciones distintas todas de equivalentes:<br>
`$ ls -trl`<br>
`$ ls -rtl`<br>
`$ ls -ltr`<br>
`$ ls -l -t -r`<br>
`$ ls -l -t -r`<br>
`$ ls -lt -r`<br>
`$ ls -l -tr`<br>
comando con opciones con '--' :<br>
`$ ls --help`<br>
`$ ls --version`<br>
`$ ls --color=auto` <br>
comando con opciones y argumentos sesibles al orden: <br>
`$ date -d now -R`<br>
`$ date -d -R now` <br>

<h2 style="text-align: center;">flujo de datos</h2>
Los datos que maneja la terminal pueden ser redirigidos a otro programa, fichero o a donde sea que lo querramos usar, y los hacemos de la siguiente manera:<br>
`>`<br>
redirige la salida standar, osea lo que se muestra en la terminal (sobreescribiendo)
<br>`<`<br>
redirige la entrada standar tomandola desde un fichero
<br>`|`<br>
comunica procesos de entrada con salida
<br>`>>`<br>
redirige la salida standar, osea lo que se muestra en la terminal (sin sobreescribir)
<br>
<div style="text-align: center;">
	<img src="img/flujo.png">
</div>