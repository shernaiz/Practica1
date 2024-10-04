# Practica 2

##  Para esta práctica tendremos que ralizar los siguientes pasos

**1-Comoroba se tes a imaxe httpd**

**2-Crea un contenedor de nome 'asir_httpd'**

**3-Mapea o porto do contenedor có 8080 da túa máquina**
    *Utiliza bind mount para que o seu directorio do apache2 'hdocs' estea montado nun directorio da túa elección.*
    _Utiliza -v "$PWD"/htdocs:/usr/local/apache2/htdocs/._

**4-Mostra unha páxina html alozada no apache2 dende o teu navegador.**

**5-Crea un contenedor 'asir_web1' que use este mesmo directorio para 'htdocs' e o porto 8000.**

**6-Crea outro contenedor 'asir_web2' co mesmos directorio e outro porto, como o 8090.**
    _Comproba que os dous servidores mostran a mesma páxina_
    