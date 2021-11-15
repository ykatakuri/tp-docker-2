# tp-docker-2

## Question 1

```bash
$ cd tp-docker-2
$ git init
$ touch README.md
```

## Question 2.a

L'option `i` de npm nous permet d'installer toutes les dépendances de notre application contenues dans le fichier `package.json`. On peut l'assimiler a docker build qui créé une nouvelle image à partir du fichier Dockerfile.

## Question 3

```bash
$ docker build -t ma_super_app .
```

Explication de la commande précédente:
- `docker build` - Permet de constuire une image
- `-t ma_super_app` - Donne le nom `ma_super_app` à notre image
- `.` - Signifie que le contexte dans lequel sera build cette image est le repertoire courant. Autrement dit, tout ce qui est copié dans l'image le sera de manière relative au reperoire courant

Pour visualiser le container créé:
```bash
$ docker container ls
```

## Question 4

Le fichier `docker-compose.yml` permet de décrire les conteneurs, appelés service dans le cas de docker-compose, qui définissent une application.

```bash
# Démarre tous les conteneurs tel que spécifié dans le fichier docker-compose.yml
$ docker-compose up -d
``` 

L'option `-d` nous permet d'éxecuter le container en background
