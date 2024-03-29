# Git

Contenido
- [Git](#git)
    - [¿Qué es Git?](#¿qué-es-git)
    - [Instalación de git en windows y linux](#instalación-de-git-en-windows-y-linux)
    - [Configuración Básica de Usuario](#configuración-básica-de-usuario)
    - [Comandos Básicos en Git](#comandos-básicos-en-git)
        - [init](#init)
        - [clone](#clone)
        - [add](#add)
        - [commit](#commit)
        - [status](#status)
        - [diff](#diff)
        - [pull](#pull)
        - [push](#push)
        - [branch](#branch)
        - [checkout](#checkout)
        - [merge](#merge)
        - [log](#log)
        - [remote](#remote)
        - [fetch](#fetch)
        - [reset](#reset)




        

## ¿Qué es Git? 

Git es un sistema de control de versiones distribuido, diseñado para rastrear cambios en archivos y coordinar el trabajo entre múltiples personas en proyectos de desarrollo de software. Fue creado por Linus Torvalds en 2005, inicialmente para el desarrollo del kernel de Linux, y desde entonces se ha convertido en una de las herramientas más populares en la gestión de código fuente.

En esencia, Git permite a los desarrolladores colaborar de manera eficiente en proyectos de software al proporcionar un historial completo de cambios en el código, así como herramientas para gestionar ramificaciones (branching) y fusiones (merging) de código. Algunas de las características principales de Git incluyen:

1. **Control de Versiones**: Git almacena todos los cambios realizados en un proyecto, lo que permite a los desarrolladores retroceder en el tiempo y recuperar versiones anteriores del código si es necesario.

2. **Gestión de Ramas**: Git permite la creación de ramas independientes del flujo principal de desarrollo, lo que facilita la implementación de nuevas características o la corrección de errores sin afectar el código base.

3. **Fusiones**: Git proporciona herramientas para fusionar ramas, lo que permite combinar cambios de diferentes desarrolladores de manera ordenada y sin conflictos.

4. **Distribuido**: Cada copia de un repositorio Git contiene todo el historial de cambios, lo que significa que los desarrolladores pueden trabajar de manera independiente sin necesidad de una conexión constante a un servidor central.

5. **Velocidad y Eficiencia**: Git está diseñado para ser rápido y eficiente, lo que permite manejar proyectos de cualquier tamaño con facilidad.

En resumen, Git es una herramienta esencial para cualquier equipo de desarrollo de software, ya que facilita la colaboración, el seguimiento de cambios y la gestión del código fuente de manera efectiva.

## Instalación de git en windows y linux 

La instalación de Git en Windows y Linux varía ligeramente, así que aquí tienes una guía básica para cada uno:
Instalación de Git en Windows:

Descarga de Git:
- Ve al sitio web oficial de Git: [Git for Windows.](https://gitforwindows.org/)
- Haz clic en el enlace de descarga para obtener el instalador.
- Ejecutar el Instalador: Una vez descargado, ejecuta el instalador. Sigue las instrucciones del instalador. Puedes mantener la mayoría de las opciones predeterminadas si no estás seguro.

- Configuración: Durante la instalación, se te pedirá que elijas el editor de texto predeterminado para Git. Puedes elegir el que prefieras o dejarlo en el predeterminado (Vim).
- Finalización:Después de la instalación, abre una nueva ventana de línea de comandos (cmd) y ejecuta git --version para verificar que Git se haya instalado correctamente.

Instalación de Git en Linux (Debian/Ubuntu):

- Actualiza el Índice de Paquetes:
```bash
sudo apt update
```
- Instala Git:
```bash
sudo apt install git
```
- Verifica la Instalación: Después de la instalación, verifica que Git se haya instalado correctamente ejecutando:
```bash
$ git --version
```
Después de instalar Git, puedes comenzar a utilizarlo en tu sistema. Recuerda configurar tu nombre de usuario y dirección de correo electrónico utilizando los comandos git config que se mencionaron en la respuesta anterior si aún no lo has hecho.

## Configuración Básica de Usuario

La configuración básica de Git implica establecer tu nombre de usuario y dirección de correo electrónico. Estos detalles se utilizan en los commits para identificar al autor de los cambios. Aquí tienes cómo configurarlos:

Configurar nombre de usuario:


```bash
$ git config --global user.name "Tu Nombre"
```
Reemplaza "Tu Nombre" con tu nombre de usuario de Git.

Configurar dirección de correo electrónico:


```bash
$   git config --global user.email "tu@email.com"
```
Reemplaza "tu@email.com" con tu dirección de correo electrónico asociada a tu cuenta de Git.

Además de esta configuración básica, también puedes establecer otras configuraciones globales, como el editor de texto predeterminado para tus mensajes de commit, la configuración de colores para la salida del terminal, etc. Aquí hay algunos ejemplos:

Establecer el editor de texto para mensajes de commit:


```bash
$ git config --global core.editor "nombre_del_editor"
```
Reemplaza "nombre_del_editor" con el nombre del editor que prefieras, por ejemplo, "nano", "vim", "emacs", etc.

Activar el uso de colores en la salida del terminal:

```bash
$  git config --global color.ui auto
```
Estas son solo algunas de las configuraciones básicas que puedes establecer en Git. Puedes explorar más opciones en la documentación oficial de Git o mediante el comando git help config.

## Comandos Básicos en Git

### init

Inicializa un repositorio Git en un directorio.


```bash
$  git init
```
### clone
Clona un repositorio Git existente desde una URL.

```bash
$  git clone <URL>
```
### add

Agrega un archivo al área de preparación para ser incluido en el próximo commit.

```bash
$ git add <archivo>
```

### commit

Registra los cambios en el repositorio con un mensaje descriptivo.

```bash
$ git commit -m "Mensaje"
```
### status

Muestra el estado actual del repositorio, incluyendo archivos modificados, agregados o pendientes de commit.

```bash
$ git status
```
### diff

Muestra las diferencias entre los archivos modificados y la versión del repositorio.

```bash
$ git diff
```

### pull

Descarga los cambios desde un repositorio remoto y los incorpora a tu rama local.

```bash
$ git pull
```
### push
Sube los cambios locales a un repositorio remoto.

```bash
$ git push
```
### branch

Lista todas las ramas en el repositorio.

```bash
$ git branch 
```

### checkout

Cambia a la rama especificada.

```bash
$ git checkout <rama> 
```

### merge
Fusiona una rama con la rama actual.

```bash
$ git merge <rama> 
```
### log

Muestra un registro de commits en la rama actual.
```bash
$ git log 
```
### remote
Muestra los repositorios remotos configurados junto con sus URLs.
```bash
$ git remote -v 
```
### fetch

Descarga los cambios desde un repositorio remoto sin fusionarlos con tu rama actual.
```bash
$ git fetch 
```

### reset

Deshace los cambios locales en los archivos modificados.
```bash
$ git reset 
```

