# Clase 06 - Bootcamp

## Repaso GIT

# Creo el repositorio de GIT

```sh
git init
```

# Listo el estado de los archivos


```sh
git status
```

# Haciendo un commit

1.  Agrego al área de staging, los archivos que necesito que formen parte del commit

```sh
git add <nombre-archivo>
git add <nombre-archivo> <nombre-archivo> <nombre-archivo> 
git add . # Agrega todos los archivos que tengo en el working directory (WD)
```

2. Hago el commit

```sh
git commit -m "Mensaje descriptivo"
```

# Cambiar el editor por nano

```sh
git config --global core.editor nano
git config --global core.editor "code --wait"
``` 

# Ver listado de commits que hice en el repo

```sh
git log # versión larga
git log --oneline # versión corta
``` 

# Agregar un remoto a mi repositorio local

```sh
git remote add origin <url-al-repo-remoto>
git remote add origin https://github.com/mleducacion/repaso-ramas.git
```

# Para ver si se agrego el repo remoto

```sh
git remote -v
```

# Subo al remoto el repositorio local

```sh
git push -u origin main # La primera vez
git push
```

# Para recuperar mi código luego de una catastrofe
Ir al repositorio de Gibhut, hacer click sobre el botón code y copiar la url a mi repositorio

```sh
git clone <url-al-repositorio>
git clone git@github.com:mleducacion/repaso-ramas.git ./ # clona en el directorio actual
git clone git@github.com:mleducacion/repaso-ramas.git # crea una carpeta (repaso-ramas) y clona el repositorio remoto al local.
```