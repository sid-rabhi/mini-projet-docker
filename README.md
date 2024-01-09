# Mini-projet Docker 

Les instructions pour le projet **student_list** se trouvent [ici](https://github.com/diranetafen/student-list.git "ici")

!["Crédit image : eazytraining.fr"](https://eazytraining.fr/wp-content/uploads/2020/04/pozos-logo.png) ![projet](https://user-images.githubusercontent.com/18481009/84582395-ba230b00-adeb-11ea-9453-22ed1be7e268.jpg)

---

Auteur : Sid Ahmed Rabhi

Contexte : formation Bootcamp DevOps promotion 16

Centre de formation : Eazytraining

Période : novembre-décembre-janvier

Date : 06 janvier 2024

LinkedIn : https://www.linkedin.com/in/sid-ahmed-rabhi/

---

## L'objectif

Déployer une application nommée **" student_list "**, très basique, qui permet à POZOS d'afficher la liste de certains étudiants avec leur âge, et par la suite offrir un registre privé pour stocker les images.

L'application student_list comporte deux modules :

- Le premier module est une API REST (nécessitant une authentification de base) qui envoie la liste souhaitée des étudiants basée sur un fichier JSON
- Le deuxième module est une application web écrite en HTML + PHP qui permet à l'utilisateur final d'obtenir une liste d'étudiants

## Le besoin

- Élaborer un conteneur dédié à chaque module.
- Établir des interactions entre ces différents conteneurs.
- Offrir un registre privé pour stocker les images Docker.

## Le Plan

- Créer un **Dockerfile** pour construire l'image du conteneur api.
- Créer un **docker-compose.yml** pour lancer l'application (API et application web), le registre local et son interface utilisateur.

---

## Étapes de réalistion du projet

1. **Construire l'image de l'API**

- Aller répertoire *simple_api* 

```bash
cd ./simple_api/
```
- Construitr l'image *student-list*

```bash
docker build -t student-list .
```

![docker images](images/image-api.png "image de l'API")
