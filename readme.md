# PROJET FIL ROUGE

## Maquetter une application

### Faire un diagramme USE CASE
![](diagramme_cas_utilisation.png)
		
### Faire un diagramme d'activité
[authentification](https://github.com/rudylps/diagrammes_gedesaft_v2/blob/master/diagrammeActivite_autentification.pdf)  
[creation Arme](https://github.com/rudylps/diagrammes_gedesaft_v2/blob/master/diagrammeActivite_creationArme.pdf)  
[creation Protagoniste](https://github.com/rudylps/diagrammes_gedesaft_v2/blob/master/diagrammeActivite_creationProtagoniste.pdf)  


### Faire un diagramme des classes
![](DiagrammeClasses.PNG)
        
        
### Identifier les acteurs d'un SI
        
        
### Dessiner des wireframe ou mockup (écrans)
        
        
### Modéliser l'enchainement des écrans
        
        
        
## Concevoir une base de données



        ### Epliquer le terme SGBDR
        
        
        ### Utiliser un outil graphique pour créer une base de données
        
        
        ### Créer/Modifier une table avec ses champs
        
        
        ### Matérialiser une relation entre tables
        
        
        ### Modéliser une base de données en 3ème forme normale
        
        
        ### Je sais écrire une requête de création de table
        
        
        ### Je sais définir une clé primaire sur une table
        
        
        ### Je sais définir une clé étrangère sur une table
        
        
        ### Je sais définir une contrainte sur une colonne donnée
        
        
        
## Mettre en place une base de données



        ### Installer un SGBDR
        
        
        ### Créer des rôles et une base
        
        
        ### Exécuter un script de création de tables / données (fichier.sql)
        
        
        ### Ecrire une requête pour insérer des données dans une table
        
        
        ### Exporter une structure de tables (données comprises) et la réintégrer dans une autre base de données
        
        
## Développer une interface utilisateur



        ### Réaliser une interface graphique
        
        
        ### Appliquer une charte graphique
        
        
        ### Analyser une maquette graphique et identifier les différentes parties d'un écran (zoning)
        
        
        ### Faire un menu
        
        
        ### Enchainer les écrans
        
        
        ### Connaitre des composants graphiques qui permettent de créer un écran
        
        
        ### Faire un formulaire de saisie
        
        
        ### Mettre en place des procédures de contrôle de saisie
        
        
        ### Faire un test unitaire manuel
        
        ### Coder avec un langae orienté objet
        
        ### Connaître la programmation événementielle
        
        ### Connaitre la programmation déclrative
        
        ### Utiliser un Environnement de Développement intégré (IDE)
        
        ### Versionner mon travail
        
        ### Mettre des commentaires dans mes programmes
        
        ### Coder selon les règles de l'art
        
        ### Produire un livrable
# GEDESAFT

Afin de pourvoir installer et lancer l'application, il faut savoir utiliser les lignes de commandes
https://windows.developpez.com/cours/ligne-commande/

## CONFIGURATION REQUISE

- JRE installer sur l'ordinateur (v 1.8), attention la v 1.9 est déconseillée
https://www.java.com/fr/download/help/download_options.xml
- MySql-server (v 5.7 +)
https://dev.mysql.com/downloads/mysql/#downloads
https://openclassrooms.com/courses/administrez-vos-bases-de-donnees-avec-mysql/installation-de-mysql (tuto installation)
- git (v2.14 +) 
https://git-scm.com/book/fr/v1/D%C3%A9marrage-rapide-Installation-de-Git
- Node.js 
https://openclassrooms.com/courses/des-applications-ultra-rapides-avec-node-js/installer-node-js (tuto installation)
https://nodejs.org/en/download/ (téléchargement)
- Angular CLI (v1.6.5 +)
lancer la ligne de commande "npm install @angular/cli" (nécéssite node.js)

## IMPORT DU PROJET

Installer les prérequis si nécéssaire
Télécharger le dossier .zip du projet 
ou l'importer (voir ci dessous)
 - Lancer le gitBash à l'emplacement ou vous voulez importez le projet (click Droit "Git Bash Here")
 - Lancer la commande "git clone https://github.com/DethierY/GEDESAFT.git"
 
## CONFIGURATION TECHNIQUE

Allez dans le dossier **resources** (GEDESAFT\src\main\resources) : 

Dedans se trouve fichier **application.properties**, il faut indiquer les informations de connection a votre base de données (url, et identiffiants admins) 

Lancer le server sql, 
importer la base de données (avec le fichier gedesaft.sql présent dans le dossier des diagrammes https://github.com/rudylps/diagrammes_gedesaft_v2.git)

## LANCEMENT DE L'APPLICATION

L'application étant séparée en deux parties, il faut les démarrer toutes les deux pour que l'application fonctionne

### Lancer l'application Springboot
Cloner ou télécharger le dossier back-end https://github.com/DethierY/GEDESAFT.git
  
    Créer un .jar : 
    
      Ouvrez une invite de commande dans le dossier "gedesaft" et lancez les lignes suivantes :
      
      - mvn package -DskipTests
      - cd target
      - java -jar java-springboot-simplecrud-0.0.1-SNAPSHOT.jar"
	  
### Lancer l'application Angular
Ce projet a été généré avec Angular CLI 1.6.5
Cloner ou télécharger le dossier front-end https://github.com/milk42/FilRougeV2Front.git

Dans le dossier du front, lancer une ligne de commande
 - npm install
 - ng serve
 
- Dans un navigateur internet, inscrire l'adresse http://localhost:4200/
	

# L'UML

Dans ce dossier vous pouvez trouver les différents diagrammes et tables qui nous ont servis pour la conception de notre application.
Les diagrammes ont été réalisé pour la première version de GEDESAFT et peuvent ne plus correspondre exactement à l'actuelle application.

## Les mockups

- Pour lire le fichier **mockUp.bmpr**, il faut le programme Balsamiq
https://balsamiq.com/
- Ensuite, ouvrir **mockUp.bmpr**.
Faire **Ctrl + F** afin de lancer le plein écran et les fonctionnalités d'enchainement des écrans matérialisants les hyperliens
