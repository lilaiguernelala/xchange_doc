# FRONTEND 

- Pour développer avec angular il faut :
Telechager **node.js** et l’installer sachant que **npm** est inclus avec node.js
Pour vérifier : 
Node -v 
Npm -v 

## Prerequisites for Developing with Angular

To develop with Angular, follow these steps:

1. Download and install **Node.js**, which includes **npm**.
2. Verify the installation:
   - Check Node.js version: `Node -v`
   - Check npm version: `Npm -v`

### Troubleshooting npm Installation

If you encounter an error with npm, check the current execution policy:
   - Get-ExecutionPolicy
   - Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

Then, verify that npm is installed correctly:
   - Check npm version: `npm -v`

### Installing Angular

1. Install Angular globally using npm:
   - `npm install -g @angular/cli`
2. Verify the Angular installation:
   - Check Angular version: `ng version`
Si le **npm** nous renvoie une erreur, on va vérifier la politique d'execution actuelle avec : Get-ExecutionPolicy
Ou : Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

Et on reverife si le npm est bien installé : npm -v 
Et maintenant normalement on aura aucune erreur.
- On installe angular : npm install -g @angular/cli
Et on verifie avec : ng version 
