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
(il met à jour)
### Récuperation du html (version à jour)
```bash
git checkout html
git pull origin html
```




