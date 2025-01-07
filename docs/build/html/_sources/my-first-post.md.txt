# Documentation du Projet

## Prérequis

Git : Installé sur votre système pour cloner le projet.

MySQL : Assurez-vous que MySQL est installé et fonctionnel sur votre PC.

Workbench ou MySQL Command Line Client : Interface ou terminal pour gérer la base de données.

Node.js et Angular CLI : Requis pour exécuter le frontend.

Maven : Requis pour exécuter le backend.

Postman : Optionnel, pour tester l’API backend.

Étapes d'installation et de configuration

1. Cloner le projet

Exécutez la commande suivante dans un terminal pour cloner le projet :

git clone [URL_DU_PROJET]

2. Créer une base de données MySQL

Option 1 : Avec MySQL Workbench

Ouvrez MySQL Workbench.

Créez une nouvelle base de données en cliquant sur Create a New Schema.

Donnez un nom à la base de données et cliquez sur Apply.

Option 2 : Avec MySQL Command Line Client

Ouvrez le terminal MySQL.

Connectez-vous avec votre nom d’utilisateur et mot de passe.

Créez une nouvelle base de données avec la commande :

CREATE DATABASE nom_de_la_base_de_donnees;

3. Configuration du fichier application.properties

Adaptez les paramètres du fichier application.properties pour correspondre aux informations de votre base de données :

spring.datasource.url=jdbc:mysql://localhost:3306/nom_de_la_base_de_donnees
spring.datasource.username=votre_nom_utilisateur
spring.datasource.password=mot_de_passe

4. Organisation des dossiers pour le backend et le frontend

Cloner deux fois le projet :

Dans le premier dossier (par exemple : backend), utilisez la commande :

git clone [URL_DU_PROJET] backend

Dans le second dossier (par exemple : frontend), utilisez la commande :

git clone [URL_DU_PROJET] frontend

Ouvrez les deux dossiers dans des IDE différents pour une exécution séparée.

5. Exécution du projet

### Backend

Ouvrez le dossier backend dans un IDE comme IntelliJ IDEA ou Eclipse.

Positionnez-vous sur la branche backend :

git checkout backend

Exécutez le backend avec Maven :

mvn spring-boot:run

### Frontend

Ouvrez le dossier frontend dans un IDE comme Visual Studio Code.

Positionnez-vous sur la branche frontend :

git checkout frontend

Lancez le serveur Angular :

ng serve

### Accédez à l’application

Ouvrez votre navigateur et accédez à :

http://localhost:4200

6. Tester le backend avec Postman

Ouvrez Postman.

Configurez une requête HTTP en spécifiant l’URL du backend (par exemple : http://localhost:8080/api/...).

Testez les différents endpoints de l’API.

**Remarques**

Organisation des branches :

Branche frontend : Contient le code pour l’interface utilisateur.

Branche backend : Contient le code pour le serveur.

- Gestion des erreurs :

Si le frontend ou le backend ne fonctionne pas, vérifiez les journaux d’erreurs dans l’IDE ou le terminal.

Compatibilité : Assurez-vous que les versions de Node.js, Maven, et MySQL sont compatibles avec les configurations du projet.

Développement avec Angular

Pour développer avec Angular, suivez les étapes suivantes :

Prérequis

Téléchargez et installez Node.js, qui inclut npm.

Vérifiez l'installation :

Version Node.js :

node -v

Version npm :

npm -v

Résolution des problèmes d'installation de npm

Si vous rencontrez une erreur avec npm, vérifiez la politique d'exécution actuelle :

- Vérifiez la politique actuelle :

Get-ExecutionPolicy

Modifiez la politique si nécessaire :

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

Re-vérifiez l'installation de npm :

npm -v

Installation d'Angular CLI

Installez Angular CLI globalement avec npm :

npm install -g @angular/cli

Vérifiez l'installation :

ng version

*Avec ces étapes, vous serez prêt à développer et exécuter des applications Angular sans rencontrer de problèmes majeurs.*
