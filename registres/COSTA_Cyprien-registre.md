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
_Moment de devloppement sur ``VisualStudioCode`` (le style.css)._

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
git commit -m "Version 1"
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
# je repush pour les oublies pas besoin de changer de commit
git push origin master
```
## Création page Contact

Je refais une branche ou je vais faire du html
```bash
git branch webtest
git checkout webtest
git branch # petit check au cas ou
ls         # petit check au cas ou
```

_Moment de devloppement sur ``VisualStudioCode`` (page contacte et des corrections)._


```bash
git add * # je met tout pour que ce soit fonctionnel à 100% car clément n'a pas tout à jours
git commit -m "page contact"
git push origin webtest
```

## update TOUT css
(le css pour la page 3 et le mobile pour 2 3 trucs)

```bash
git checkout -b stylev2
```
_Moment de devloppement sur ``VisualStudioCode`` (correction mobile et maj css)._

### On upload sur la branche
```bash
git add *
git commit -m "CSS V2 (responsive correcte)"
git push origin stylev2
```

### import de presentation
```bash
git pull origin presentation
```
_quelque corrections_

### import dans master
validation team

```bash
git checkout master
git merge stylev2
git add *
git commit "finale"
git push origin master
```

# FIN 

j'ai pas fait de clone car de base je l'ai créer directement moi.
Et aussi pour la dernnière partie toute les commandes ne sont pas parfaites car j'ai du speed pour l'upload en master de tout.