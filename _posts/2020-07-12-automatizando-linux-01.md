---
layout: post
title: No se pudo bloquear? Ubuntu
date: 2020-07-12 1:30
author: developmentMen
tags: ubuntu linux bloq bloqear recurso no se pudo bloquear
---
<div style="text-align: center;">
	<h1>
		Alguna vez te paso esto?
	</h1>
	E: NO SE PUDO BLOQUEAR /VAR/LIB/DPKG/LOCK – OPEN (11: RECURSO NO 
	DISPONIBLE TEMPORALMENTE) <br>
	E: NO SE PUDO BLOQUEAR EL DIRECTORIO DE ADMINISTRACIÓN (/VAR/LIB/
	DPKG/), ¿QUIZÁS HAYA ALGÚN OTRO PROCESO UTILIZÁNDOLO?
	<img src="https://external-content.duckduckgo.com/
	iu/?u=https%3A%2F%2F1.
	bp.blogspot.com%2F-kPswYc9C_dA%2FXbcP0tLFCaI%2FAAAAAAAADfU%2FXXG1OHT9qj
	I
	3xwu6Ckt3rOJJGnTn7LG0QCLcBGAsYHQ%2Fs1600%2Ferrorvarlibdpkglock.jpg&f=1&
	nofb=1">
	<h2>
		En este post te tengo la solucion
		<hr>
	</h2>
</div>
probado en ubuntu/linux

<h2 style="text-decoration: underline;">Paso 1</h2>
copiamos y pegamos el comando:
<h3 style="text-align: center; color: yellow;">
	sudo fuser -vki nombre/del/proceso
</h3>
fuser es una sencilla pero poderosa utilidad de línea de comandos que
busca localizar procesos basados ​​en los archivos, directorios o zócalos 
a los que accede un proceso en particular. En resumen, ayuda a un 
usuario del sistema a identificar procesos mediante archivos o sockets
con este comando estamos <em>"matando"</em> el proceso ya que la letra -k 
corresponde a -kill

<h2 style="text-decoration: underline;">Paso 2</h2>
copiamos y pegamos el comando:
<h3 style="text-align: center; color: yellow;">
	sudo rm -f nombre/del/proceso
</h3>
rm elimina archivos y con -f le decimos que elimine sin dar vueltas ni mas

<h2 style="text-decoration: underline;">Paso 3</h2>
copiamos y pegamos el comando:
<h3 style="text-align: center; color: yellow;">
	sudo dpkg --configure -a
</h3>
El programa DPKG es la base del sistema de gestión de paquetes de Debian GNU
/Linux

<h2 style="text-decoration: underline;">Paso 4</h2>
copiamos y pegamos el comando:
<h3 style="text-align: center; color: yellow;">
	sudo apt autoremove
</h3>
APT es el administrador de paquetes de ubuntu y con este comando 
basicamente le decimos que elimine los paquetes que no se usan o que fueron 
reemplazados por otra actualizacion

<div style="text-align: center;">
	<h2>
		Solucion a largo plazo
		<hr>
	</h2>
</div>

La realidad es que este problema va a seguir apareciendo a lo largo del 
tiempo y de momento en internet no encontre solucion permanente pero se 
puede simplificar su uso de la siguiente manera

<h3>importante:</h3> asegurate de tener installado [git hub][git-hub] (en 
linux se installa con el commando: <em>sudo apt install git</em>)

<h2 style="text-decoration: underline;">Paso 1</h2>
copiamos y pegamos el comando:
<h3 style="text-align: center;">
	git clone https://github.com/developmentMen/autolinux.git
</h3>
esto va a clonar mi [repositorio de automatizaciones][repo] linux creadas y 
probadas en ubuntu
<img src="img/git-clone.png"><br>
una vez echo esto nos va a crear una carpeta llamada <b>autolinux</b> si
vemos dentro de ella se encuentra lo siguiente:
<br><img src="img/ll.png"><br>
el archivo <b>bloq</b> es el que nos facilita arreglar todo de ahora en mas

<h2 style="text-decoration: underline;">Paso 2</h2>
ahora ya solo tenemos que copiar el archivo <b>bloq</b> a una carpeta que 
nos resulte comoda, yo personalmente lo tengo en la misma ruta donde se 
abre la terminal para hacer lo siguiente

copiamos y pegamos el comando:
<h3 style="text-align: center;">
	./bloq nombre/del/proceso/
</h3>
<img src="img/bloq.png"><br>
de esta manera cuando me aparezca el error "no se pudo bloquear" solo tengo 
q escribir el nombre del proceso a eliminar

[git-hub]: https://git-scm.com/download/
[repo]: https://github.com/developmentMen/autolinux.git
