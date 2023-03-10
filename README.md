# samuel-colin.github.io

Site Web de Samuel Colin :)

## Environnement Technique

Le site a été créé en [VueJS 3.2.13](https://vuejs.org/) avec [Materialize 3.0.1](https://materializecss.com/).

## Build du Projet

Téléchargement des librairies
```
npm install
```
Lancement du serveur en local
```
npm run serve
```

### Compilation et minifaction pour la Production
```
npm run build
```
Copie des fichiers de Production dans le répertoire _/docs_
```
cp ./dist ./docs
```
Merge des développements sur la branche _gh-pages_ (permet le déploiement sur le site GitHub)
```
git merge gh-pages
```

## Déploiement sur Docker
Création de l'image Docker (Serveurs NodeJS et Apache)
```
docker build -t vuejs-samuel-colin/samuel-colin-app .
```
Création du conteneur à partir de l'image
```
docker run -it -p 8092:8080 --rm --name samuel-colin-app vuejs-samuel-colin/samuel-colin-app 
```