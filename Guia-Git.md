# Guia de Git

## Conceptos básicos

Working directory : Área de trabajo donde se encuentran los archivos que está modificando y creando,pero no están enlazados a Git aún.

Staging area : Área donde los archivos seleccionados están siento trackeados por Git y listos para ser guardados en el repositorio.

Repository : Contiene todos los commit provenientes de Staging area.

## Flujo 1 : Configurar git

### Creación de llave SSH en equipo

`ssh-keygen -t rsa -b 4096 -c youremail@example.com`

Ver llave creada:  
`cd ~/.ssh`  
`cat id_rsa.pub`  
Copiar toda la llave(incluido "ssh-rsa...")

Agregar información del usuario:  
`git config --global user.name "yourname"`  
`git config --global user.email "youremail"`

### Crear repositorio

Situarse en el path deseado y `git init`.

## Flujo 2 : Trabajo local

Crea tus archivos en el path donde creó el repositorio. Comienza a modificarlos y cuando considere que ha llegado a un punto donde debe guardar ese estado,entonces :  
`git add <archivo>` o en su defecto  
`git add .` y añade todos los archivos del working directory

### Flujo 2.1 : Revertir al ultimo guardado

Si ya ha guardado sus archivos con `git add`,y ahora está modificandolos para ver si funciona su próxima tarea,cabe la posibilidad que no lo haga y requiera regresar al estado del archivo cuando se hizo el `git add`. Puede hacerlo con:  
`git checkout -- <archivo>`

### Flujo 2.2 : Guardar un estado de su proyecto

Si ya añadió con `git add` sus archivos,y ahora considera que no solo los quiere guardar,si no almacenar como un estado de su proyecto.Sea una versión 0.1 y compartirla,entonces debería hacer un `git commit`. Esto le abrirá su editor por defecto enlazadao con Git,e insertará la descripción acompañada de su commit.

Si su descripción es corta,o quiere escribir un comando corto,use:
`git commit -m "Descripcion"`

`git log` : te permite ver todos los commit hechos

## Flujo 3 : Creación de ramas locales

A veces,un cambio del directorio al área de staging es muy limitado,ya que se busca modificar por completo algún módulo con grandes cambios e incluso mientras se reaizan los cambios,se requiere ir haciendo commits. Es aquí donde surgen las ramas.
Son una linea que surge del estado actual de la rama principal(master o main,dependiendo de tu configuración en Git). Por estado actual refiere a los commits hechos en `master`. La nueva rama hereda esto,y si se hace un commit en esta,no se ve reflejado en el `master`,hasta que usted decida unir ambas para mezclar el código avanzado.

Puede ver una rama como un entorno para una persona o varias donde se realizan pruebas y avances ajenos o con duda sin comprometer el código principal,ubicado en `master`.
