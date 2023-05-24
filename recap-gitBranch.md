"Git branch" : Gérer différentes versions de votre projet

Bonjour ! 
Aujourd'hui, je vais vous parler de Git, qui est un outil très utilisé par les développeurs pour gérer les versions de leurs projets.
Nous allons nous concentrer sur l'une des fonctionnalités importantes de Git appelée "Git branch".

[ Qu'est-ce que Git ?
Git est un système de contrôle de version qui permet de garder une trace des modifications apportées à un projet.
Il permet à plusieurs personnes de travailler ensemble sur un même projet en même temps. ]

Comprendre les branches :
Une branche dans Git est une version distincte de votre projet.
Cela vous permet de travailler sur différentes fonctionnalités ou modifications sans perturber la version principale.
Imaginez une branche comme une copie de votre projet dans laquelle vous pouvez faire des modifications sans affecter le projet principal.

Création et utilisation des branches :
Lorsque vous créez une branche, vous pouvez vous y déplacer et commencer à travailler dessus, laissant la branche principale (appelée souvent "master" ou "main") intacte.
Cela vous permet de développer des fonctionnalités spécifiques ou de corriger des bogues sans affecter la version principale.

Fusionner les branches :
Une fois que vous avez terminé de travailler sur une branche et que vous êtes satisfait du résultat, vous pouvez fusionner cette branche avec la branche principale.
La fusion combine les modifications de la branche dans la branche principale, vous permettant ainsi de mettre à jour votre projet avec les nouvelles fonctionnalités ou corrections.

Avantages de l'utilisation des branches :
Vous pouvez travailler sur différentes fonctionnalités simultanément, ce qui permet une meilleure organisation du travail en équipe.
Utiliser des branches, permet de revenir facilement en arrière et de corriger les erreurs sans affecter le projet principal.
Les branches permettent également d'expérimenter de nouvelles idées sans risquer de perturber le travail déjà réalisé. (exemple : tester des refactos...)

Conclusion :
La fonction "Git branch" permet de gérer différentes versions de votre projet.
En utilisant les branches, vous pouvez travailler de manière plus efficace, en gardant le contrôle sur les modifications et en facilitant la collaboration.
N'hésitez donc pas à créer, systématiquent vos propres branches pour mieux organiser votre travail.
(Même sur un projet travaillé seul, créer une branche "Dev" permet de préserver le travail déjà effectué et sauvegardé dans le main).

#### Principales fonctionnalités dans "git branch" :
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


