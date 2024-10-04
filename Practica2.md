# Practica 2

##  Para esta práctica tendremos que ralizar los siguientes pasos

**1-Comoproba se tes a imaxe httpd**
    Para comproabr se temors a imaxe httpd teremos que lanzar o comando *docker images*. Esto mostrará unha lista cas imaxes que temos, neste caso sí teremos a imaxe httpd.

**2-Crea un contenedor de nome 'asir_httpd'**
    Para crear un contenedor con este nome teremos que lanzar o comando de creación co nome correspondiente, neste caso lanzaremolo xa co porto mapeado para aforrar este paso.

**3-Mapea o porto do contenedor có 8080 da túa máquina**
    *Utiliza bind mount para que o seu directorio do apache2 'hdocs' estea montado nun directorio da túa elección.*
    *Utiliza -v "$PWD"/htdocs:/usr/local/apache2/htdocs/*

   Para mapear o porto do contenedor creado teremos que lanzar o seguinte comando que crea e mapea o porto do contenedor *sudo docker run --name asir_httpd -d -p 8080:80 -v "$PWD"/htdocs:/usr/local/apache2/htdocs/ httpd*

**4-Mostra unha páxina html aloxada no apache2 dende o teu navegador.**
    Para isto teremos que entrar no noso navegador e na barra de búsqueda teremos que escibir a seguinte dirección _https:/localhost:8080_

**5-Crea un contenedor 'asir_web1' que use este mesmo directorio para 'htdocs' e o porto 8000.**
    Para facer isto volveremos a lanzar os dous comandos de antes nun pero co nome do novo contenedor *sudo docker run --name asir_web2 -d -p 8000:80 -v "$PWD"/htdocs:/usr/local/apache2/htdocs/ httpd*

**6-Crea outro contenedor 'asir_web2' co mesmos directorio e outro porto, como o 8090.**
    _Comproba que os dous servidores mostran a mesma páxina_
    Para comprobar que os dous contenedores mostran a misma imaxe só teremos que repetir o paso anterior e entrar no enlace da páxina, este vez con porto 8000 _http/localhost:8000_
