# *************** VERSION, STATUS & LOG ***************
## Git version
$ git --version
## Git status
$ git status

*************** CONFIGURATION UTILISATEUR ***************
## Configuration Utilisateur
$ git config --global user.name "Alain Deloin"
$ git config --global user.email "a.deloin@lol.fr"

*************** INITIALISATION ***************
## Initialisation dépot Git
$ git 

*************** AJOUTER TOUT ***************
## ajouter tous les fichiers à la staging area
$ git add .

*************** COMMIT & PUSH & LOGS ***************
## ajouter un fichier à la stagging area
$ git add <nomFichier>
## Création d'un commit
$ git commit -m "Nom du commit"
## Ajout des nouveau fichiers et Création d'un commit en une commande
$ git commit --all
## Upload commit 
$ git push
## Avoir La liste des commits
$ git log
=> q pour quitter
=> h pour help
## Les arguments git log
$ git log --oneline
$ git log -n "NbCommit"

$ git log -p "fichier"
$ git log --author "auteur" 

*************** BRANCHES ***************
## Lister les branches
$ git branch

## Créer une nouvelle branche
$ git branch "NomBranche"
## Création d'une branche depuis l'actuelle
$ git checkout "NomBranche"

## Création d'une branche et Switch sur nouvelle branche
$ git checkout -b "NomBranche"
## Renommer la branche active
$ git branch -m <nouveauNomDeLaBranche>

## Push d'une branche sur le dépot distant
git push --set-upstream origin dev

## Faire un fetch de la branche active et basculer sur une autre branche
git fetch && git checkout "NomAutreBranche"

## Supprimer une branche
$ git branch -d <nomDeLaBranche>

*************** CONFIGURATION DEPOT DISTANT ***************
## Ajouter un repos distant
$ git remote add origin https://Mon.repos.fr
## Push sur nouveau repos distant
$ push -u origin master
## Clonage d'un repos distant
$ git clone <lien vers le dépôt distant