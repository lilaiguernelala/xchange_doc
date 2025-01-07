# Documentation du Projet

Le projet **Home Exchange** a été développé dans le cadre du programme **CAP Projet** de l'ESIEA, en collaboration avec **Thales Services Numériques**.
Ce projet vise à concevoir et implémenter une plateforme numérique dédiée à l'échange de logements entre particuliers. L'équipe de développement, composée de Alpha Oumar DIALLO, Mohamed Mouad GUESSOUS, Lila IGUERNELALA, Hamza JAMI, Hana HOUSSEIN MOUSSA et Karl NDOBA, est responsable de la conception, du développement et de l'intégration des différents composants techniques de la plateforme.

## Prérequis

* Git : Installé sur votre système pour cloner le projet.
* MySQL : Assurez-vous que MySQL est installé et fonctionnel sur votre PC.
* Workbench ou MySQL Command Line Client : Interface ou terminal pour gérer la base de données.
* Node.js et Angular CLI : Requis pour exécuter le frontend.
* Maven : Requis pour exécuter le backend.
* Postman : Optionnel, pour tester l’API backend.

## Étapes à suivre pour l'installation et la configuration du projet

### 1. Cloner le projet

Exécutez la commande suivante dans un terminal pour cloner le projet :

```js
git clone git@gitlab.esiea.fr:mguessous/xchange.git
```

### 2. Créer une base de données MySQL

#### Option 1 : Avec MySQL Workbench

1. Ouvrez MySQL Workbench.
2. Créez une nouvelle base de données en cliquant sur Create a New Schema.
3. Donnez un nom à la base de données et cliquez sur Apply.

#### Option 2 : Avec MySQL Command Line Client

1. Ouvrez le terminal MySQL.
2. Connectez-vous avec votre nom d’utilisateur et mot de passe.
3. Créez une nouvelle base de données avec la commande :

```js
CREATE DATABASE nom_de_la_base_de_donnees;
```

### 3. Configuration du fichier application.properties

Adaptez les paramètres du fichier application.properties pour correspondre aux informations de votre base de données :

```js
spring.datasource.url=jdbc:mysql://localhost:3306/nom_de_la_base_de_donnees
spring.datasource.username=votre_nom_utilisateur
spring.datasource.password=mot_de_passe
```

### 4. Organisation des dossiers pour le backend et le frontend

1. Cloner deux fois le projet :
   * Dans le premier dossier (par exemple : backend), utilisez la commande :

```js
git clone git@gitlab.esiea.fr:mguessous/xchange.git backend
```

   * Dans le second dossier (par exemple : frontend), utilisez la commande :

```js
git clone git@gitlab.esiea.fr:mguessous/xchange.git frontend
```

2. Ouvrez les deux dossiers dans des IDE différents pour une exécution séparée.

### 5. Exécution du projet

#### Backend

1. Ouvrez le dossier backend dans un IDE comme IntelliJ IDEA ou Eclipse.
2. Positionnez-vous sur la branche backend :

```js
git checkout backend
```

3. Exécutez le backend avec Maven :

```js
mvn spring-boot:run
```

#### Frontend

1. Ouvrez le dossier frontend dans un IDE comme Visual Studio Code.
2. Positionnez-vous sur la branche frontend avec la commande :

```js
git checkout frontend
```

3. Lancez le serveur Angular :

```js
ng serve
```

### 6. Accédez à l’application

Ouvrez votre navigateur et accédez à :

```
http://localhost:4200
```

### 7. Tester le backend avec Postman

1. Ouvrez Postman.
2. Configurez une requête HTTP en spécifiant l’URL du backend (par exemple : http://localhost:8080/api/...).
3. Testez les différents endpoints de l’API.

## Remarques

* Organisation des branches :
  * Branche frontend : Contient le code pour l’interface utilisateur.
  * Branche backend : Contient le code pour le serveur.
* Gestion des erreurs :
  * Si le frontend ou le backend ne fonctionne pas, vérifiez les journaux d’erreurs dans l’IDE ou le terminal.
* Compatibilité : Assurez-vous que les versions de Node.js, Maven, et MySQL sont compatibles avec les configurations du projet.
* Vérifiez l'installation :
  * Version Node.js :

```js
node -v
```

  * Version npm :

```js
npm -v
```

* Si vous rencontrez une erreur avec npm, vérifiez la politique d'exécution actuelle :

```js
Get-ExecutionPolicy
```

* Modifiez la politique si nécessaire :

```js
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

* Re-vérifiez l'installation de npm :

```js
npm -v
```

* Vous pouriez installer Angular CLI globalement avec npm maintenant avec la commande suivante :

```js
npm install -g @angular/cli
```

* Vérifiez l'installation :

```js
ng version
```

*Avec ces étapes, vous serez prêt à développer et exécuter notre application sans rencontrer de problèmes majeurs.*
