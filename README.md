# Practica1
## Práctica 1 da asignatura SRI

**Descargar e comprobar que unha imaxe está no teu equipo**
    Para lanzar unha imaxe desde o equipo teremos que usar o comando _docker run [nome da imaxe]_ onde sustituiremos o nome da imaxe polo que temos asignado.

    Para poder visualizar as imaxes que temos no ordenador teremos que lanzar o comando _docker images_ o que nos mostrará un listado das imaxes creadas.

**Crear un contenedor sen nome, queda arrincado? Cómo obtés o nome?**
    Para crear un contenedor sen nome simplemente teremos que omitir a opción _--name_ ao executar o comando _docker run_.
    Ao non asignar un nome, o propio #0969DA Docker xerará un aleatorio.