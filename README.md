# Practica1
## Práctica 1 da asignatura SRI

**1-Descargar e comprobar que unha imaxe está no teu equipo**
    Para lanzar unha imaxe desde o equipo teremos que usar o comando _docker run [nome da imaxe]_ onde sustituiremos o nome da imaxe polo que temos asignado.

    Para poder visualizar as imaxes que temos no ordenador teremos que lanzar o comando _docker images_ o que nos mostrará un listado das imaxes creadas.

**2-Crear un contenedor sen nome, queda arrincado? Cómo obtés o nome?**
    Para crear un contenedor sen nome simplemente teremos que omitir a opción _--name_ ao executar o comando _docker run_.
    Ao non asignar un nome, o propio **Docker _xerará_ un aleatorio**.

**3-Crea un contenedor co nome 'u1', como accedes a el?**
    Para crear un contenedor co nome 'u1' teremos que lanzar o comando _docker run --name u1_.
    Para poder acceder ao contenedor creado teremos que usar o comando _docker exect -it u1_.

**4-Comproba a sua ip e fai ping a google.com**
    Para comprobar a ip primeiro teremos que lanzar o comando anterior para acceder o contenedor, unha vez dentro teremos que lanzar o coamndo _ifconfig_ o que nos responderá ca ***IP***.
    E para facer ping só teremos que lanzar o comando ***ping google.com***

**5-Crea un contenedor co nome 'bono', podes facer ping entre os contenedores?**
    Para crear o novo contenedor teremos que lanzar o comando de antes pero co nome do novo contenedor, neste caso '_bono_'.
    Para poder facer ping entre eles teremos que crear unha red personalizada co comando _docker network create [nombre da rede]_, unha vez lanzado teremos que iniciar os dous contenedores co comando _run_ e para facer ping entre eles teremos que realizar os comandos vistos no paso anterior.

**6-Se pechas as terminales que pasa co contenedor**
    No caso de pechar a terminal non se pecharían nin detendrían os contenedores iniciados.

**7-Cánta memoria no disco duro ocupaches?**
    Para conocer a memoria usada teremos que ter ao menos un contenedor en funcionamiento e lanzar o comando _docker system df_ o que nos mostrará todas as imaxes e a memoria empregada. Neste caso unha imaxe ocúpame 142 B.

**8-Canta RAM ocupan os contenedores? Crea varios para calculalo**
    Para saber canta memoria ocupan teremos que lanzar varios contenedores e despois lanar o comando _docker stats_ que nos dará diversa información sobre os contenedores.

**9-Como fixeches para clonar o repositorio**
    Para clonar o repositorio tiven que lanzar o comando an terminal _git clone [direccion do repositorio]_ a dirección podemos atoipala no repositorio visto dende un navegador web. 

**10-Como engades o arquivo readme2.md**
    Para añadir o arquivo teremos que usar o coamndo _git add readme2.md_ esto añadirá o arquivo ao reposorio.

**11-Os pasos a seguir para subir o arquivo que estas editando e o readme2.md**
    Para isto teremos que lanzar o comando _commit -m [mensaxe a elección]_ e subiranos os cambios realizados ao repositorio.

**12-Como comprobarías que existe diferencias entre o teu repositorio local e remote?**
    Co comando _git status_ podemos ver que arquivos temos modificados pero non actualizados no repositorio, polo que sería unha forma de ver os cambios.