# Soumettre.fr : API pour Webmasters #

## Installation ##
Via Git : git clone git@github.com:soumettre/sdk-api-php.git soumettre-api

Via composer/packagist : composer require soumettre/sdk-api-php

## Getting started ##
1. Crééz un compte client gratuit sur [https://soumettre.fr/](https://soumettre.fr/).
1. Installez le package dans un répertoire de votre site accessible depuis l'extérieur.
1. Editez le fichier config.php à la racine du package.
1. Implémentez les services 


## Acces depuis notre serveur ##

Votre installation doit être accessible depuis notre serveur.
Le package propose un type d'installation : toutes les requêtes vers le répertoire sont routées vers index.php, et SoumettreApi se charge de déterminer le service appelé en fonction de la route.

## Implémentation des services ##

Etendez la classe SoumettreApi pour implémenter les 4 dernières méthodes (les "services") à votre façon.
Ces méthodes, telles qu'implémentées dans la classe, sont des exemples des retours attendus.
 
A l'heure actuelle, ces services sont au nombre de 4 : 

+ check_added : Vérifie si un site est déjà présent sur votre plate-forme
+ categories : Renvoie la liste de vos catégories et sous-catégories, ainsi que leurs liens de parenté
+ post : Ajoute un post sur votre plate-forme
+ delete : Efface un post de votre plate-forme

