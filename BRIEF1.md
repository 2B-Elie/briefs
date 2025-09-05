# Brief 1 – Système d’Auth

## Contexte
L’authentification est une étape incontournable pour sécuriser une API. Elle permet d’identifier les utilisateurs et de leur attribuer un accès personnalisé.  
Dans ce projet, nous devons mettre en place un système simple de **login** et **register** afin que les utilisateurs puissent s’inscrire et se connecter.  
L’utilisation de **JWT (JSON Web Token)** permettra de gérer la persistance de la session côté client et de protéger certaines routes.

## Objectif pédagogique
- Comprendre le fonctionnement de l’authentification par token.
- Savoir créer des routes sécurisées d’inscription et de connexion.
- Apprendre à générer et renvoyer un JWT depuis l’API.

## Tâches
1. Créer la route `POST /auth/register` permettant d’inscrire un utilisateur.  
   - Stocker les informations de l’utilisateur (username, email, mot de passe).  
   - Vérifier les erreurs simples (champs obligatoires, formats).  
2. Créer la route `POST /auth/login` permettant de connecter un utilisateur existant.  
   - Vérifier que l’email et le mot de passe correspondent.  
   - Générer un token JWT et le renvoyer dans la réponse.  
3. Configurer un middleware pour gérer la génération et la vérification des JWT.

## Livrables
- Code des routes `register` et `login`.  
- Middleware JWT fonctionnel.  
- Exemple de tests avec Postman (inscription + connexion).  

## Ressources utiles
- [jsonwebtoken (npm)](https://www.npmjs.com/package/jsonwebtoken)  
- [bcryptjs pour le hachage des mots de passe](https://www.npmjs.com/package/bcryptjs)  
- [Express.js – Middleware](https://expressjs.com/en/guide/using-middleware.html)

