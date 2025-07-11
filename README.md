# Github dedicado al curso de fundamentos en ciencias de datos

Repositorio fundamentos en ciencia de datos. Realizado por el docente Gustavo Castrillón.

Este material esta basado en el curso de [data 8](http://www.data8.org/). 


Algunas instruccion para que pueda trabajar con ssh desde la maquina local

# Crear una clave SSH RSA con GitHub en Linux y envío automático con un script

### 1. **Generar una clave SSH RSA**

Para generar una clave SSH de tipo RSA, sigue los pasos a continuación:

#### Paso 1: Abrir una terminal y generar la clave SSH

Ejecuta el siguiente comando para generar una nueva clave SSH RSA:

```bash
ssh-keygen -t rsa -b 4096 -C "tu_email@example.com"# 002_InstructorAprendizajeEstadistico-
```

# Paso 2: Definir la ubicación de la clave
Cuando te pregunte dónde guardar la clave, puedes presionar Enter para aceptar la ubicación por defecto (/home/tu_usuario/.ssh/id_rsa), 
o puedes especificar otra ruta si lo prefieres.


# Paso 3: Agregar tu clave SSH a GitHub

- Copiar tu clave pública

Debes copiar el contenido de tu clave pública para agregarla a GitHub. Utiliza el siguiente comando para mostrar la clave pública:

```bash
cat ~/.ssh/id_rsa.pub
```


- Agregar la clave pública en GitHub

Ve a GitHub e inicia sesión.
En la esquina superior derecha, haz clic en tu foto de perfil y selecciona Settings.
En la barra lateral izquierda, selecciona SSH and GPG keys.
Haz clic en New SSH key.
En el campo Title, introduce un nombre para la clave (por ejemplo, "Clave SSH para mi máquina").
En el campo Key, pega tu clave pública (el contenido que copiaste anteriormente).
Haz clic en Add SSH key.



# Envío automático con el script send_github.sh, este esta oculto en el directorio.

Puedes automatizar el proceso de pull, add, commit, y push con el siguiente script en Bash llamado send_github.sh.

Script send_github.sh:

```bash
./.send_github.sh "Tu mensaje de commit"
```



Sincronizar los cambmios depues de que se realiza en local
git fetch --all --prune

git checkout nombre de la rama 

git branch -r 
# Github dedicado al curso de fundamentos en ciencias de datos para los profesores del curso.

Este material esta basado en el curso de [data 8](http://www.data8.org/). 



Algunas instruccion para que pueda trabajar con ssh desde la maquina local

# Crear una clave SSH RSA con GitHub en Linux y envío automático con un script

### 1. **Generar una clave SSH RSA**

Para generar una clave SSH de tipo RSA, sigue los pasos a continuación:

#### Paso 1: Abrir una terminal y generar la clave SSH

Ejecuta el siguiente comando para generar una nueva clave SSH RSA:

```bash
ssh-keygen -t rsa -b 4096 -C "tu_email@example.com"# 002_InstructorAprendizajeEstadistico-
```

# Paso 2: Definir la ubicación de la clave
Cuando te pregunte dónde guardar la clave, puedes presionar Enter para aceptar la ubicación por defecto (/home/tu_usuario/.ssh/id_rsa), 
o puedes especificar otra ruta si lo prefieres.


# Paso 3: Agregar tu clave SSH a GitHub

- Copiar tu clave pública

Debes copiar el contenido de tu clave pública para agregarla a GitHub. Utiliza el siguiente comando para mostrar la clave pública:

```bash
cat ~/.ssh/id_rsa.pub
```


- Agregar la clave pública en GitHub

Ve a GitHub e inicia sesión.
En la esquina superior derecha, haz clic en tu foto de perfil y selecciona Settings.
En la barra lateral izquierda, selecciona SSH and GPG keys.
Haz clic en New SSH key.
En el campo Title, introduce un nombre para la clave (por ejemplo, "Clave SSH para mi máquina").
En el campo Key, pega tu clave pública (el contenido que copiaste anteriormente).
Haz clic en Add SSH key.



# Envío automático con el script send_github.sh, este esta oculto en el directorio.

Puedes automatizar el proceso de pull, add, commit, y push con el siguiente script en Bash llamado send_github.sh.

Script send_github.sh:

```bash
./.send_github.sh "Tu mensaje de commit"
```



Sincronizar los cambmios depues de que se realiza en local
git fetch --all --prune

git checkout nombre de la rama 

git branch -r 
