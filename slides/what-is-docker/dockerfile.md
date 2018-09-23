## Dockerfile

C'est la recette de construction d'une image docker.

* On part d'une image existante
* On y exécute des commandes qu'on aurait du taper dans un conteneur pour arriver à l'état désiré

```docker
FROM centos:7

RUN  yum install httpd -y
```
