# Compte rendu de commande Exam git
## Pierre Barbary Le Floch 

### Initialisation et Connection 

```bash 
# Sur une VM type kali 
sudo apt install git 
git --version  # verif 

cd documents 
mkdir projetGIGIT 
cd projetGIGIT
git init 
ls -a # verif 
```

### Connexion avec le dépot 

```bash 
git remote add origin https://github.com/Peterblf/projetGIGIT.git

git config user.name "Peterblf"
git config user.email "pierrebrech@icloud.com"
```

### Création et envoi vers le dépot du 1er fichier 
```bash 
git branch html
git checkout html 

nano index.html 
# ajout de html classique 

git add index.html
git commit -m "1er test h1"
git push -u origin html 
```

### MAJ de l'index.html

```bash 
git add index.html 
git commit -m "top/bottom, nav, aside(pub), footer"
git push -u origin html 
```
#### - Répétition de la même action plusieurs fois avec les MAJ suivante 

### Suppression des branches en trop pour le rendu 
```bash 
git branch -a css
git branch -a html # etc pour le reste des branches en trop 
```