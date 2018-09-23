### Construiser votre propre image

Creer le fichier

```bash
vi Dockerfile
```

Le contenu

```docker
# Utilise une version legere de l'image httpd
FROM httpd:alpine

# Copy le dossier public-html de la machine physique vers le conteneur
COPY ./public-html/ /usr/local/apache2/htdocs/
```

Construiser l'image
```bash
mkdir public-html
echo 'FROM DOCKER' > public-html/index.html
docker build -t mib4fun/demo-httpd .
```
