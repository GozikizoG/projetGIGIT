# EXAM GIT

## 1. Mise en place :

```bash
cd GIT
mkdir projetGIGIT
cd projetGIGIT

git init
git remote add origin https://github.com/GozikizoG/projetGIGIT.git

git config user.name "GozikizoG"
git config user.email "cypriencosta77@gmail.com"
```
## 2. Création CSS

### Mise en place fichier et dossier

```bash
mkdir css
cd css
nano style.css
# ctrl+S // oui, il est vide
# ctrl+X // c'est parce que je vais le faire sur VSC
```
_Moment de devloppement sur ``VisualStudioCode``._

## 3. Upload du CSS

### On prend la dernière version

```bash 
git pull origin master

ls -a # on check les changement
```

### création de branche

```bash
git branch css
git checkout css # oui on peut faire les deux en même temps mais bon
```

### Le premier commit

```bash
cd css
git add style.css
git commit -m "version de base - style.css"
git push -u origin css
```

On attend les premiers html de mon collaborateur

## Mise à jour avec une vu sur l'index

(je faisais ça à l'aveugle avant)

### Récuperation du html (version non à jour)
```bash
git checkout html
git pull origin html
```
(il met à jour, entre temps j'ai créer un dossier registre avec ce registre dedans)
### Récuperation du html (version à jour)
```bash
git checkout html
git pull origin html
```
tout est bon je met en master avec validation team
## Mise en master d'une V1

On ramène le tout en master
```bash
git checkout master
git pull origin html
git pull origin css
```
_Je recheck les dossiers_
```bash
git add *
git commit -m "je me rappelle plus du nom que j'ai mis"
git push origin master
```
Je suprime les vieilles branches
```bash
git branch -d html
git branch -D css 
#on force car j'ai du changer un peu le css et il dit que c'est pas full merged
```
Rendu
```bash
git add *
git commit -m "je me rappelle plus du nom que j'ai mis"
git push origin master
```
## Création page 2

Je refais une branche ou je vais faire du html
```bash
git branch webtest
git checkout webtest
git branch # petit check au cas ou
ls         # petit check au cas ou
```

_Moment de devloppement sur ``VisualStudioCode``._


```bash
git add *
git checkout webtest
git branch # petit check au cas ou
ls         # petit check au cas ou
```