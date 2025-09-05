# Brief 2 – Routes Protégées

## Contexte
Une fois l’authentification en place, il est essentiel de limiter l’accès à certaines ressources.  
Dans notre application, seuls les utilisateurs connectés doivent avoir la possibilité de créer de nouveaux posts.  
Cela implique de mettre en place un système de **routes protégées** grâce à la vérification du token JWT.

## Objectif pédagogique
- Comprendre la logique des middlewares de protection des routes.
- Savoir utiliser un JWT pour autoriser ou refuser l’accès à une ressource.
- Apprendre à sécuriser une API REST avec un système d’authentification.

## Tâches
1. Créer un middleware `authMiddleware` qui :  
   - Récupère le token JWT depuis les headers de la requête.  
   - Vérifie sa validité et extrait les infos de l’utilisateur.  
   - Refuse l’accès si le token est manquant ou invalide.  
2. Protéger la route `POST /posts` afin qu’elle ne soit accessible qu’aux utilisateurs authentifiés.  
3. Tester l’accès à la route via Postman :  
   - Cas avec un token valide (accès autorisé).  
   - Cas sans token ou token invalide (erreur 401).  

## Livrables
- Middleware de protection JWT fonctionnel.  
- Route `POST /posts` accessible uniquement aux utilisateurs connectés.  
- Capture Postman montrant le test d’un accès autorisé et refusé.  

## Ressources utiles
- [jsonwebtoken – Vérification des tokens](https://www.npmjs.com/package/jsonwebtoken)  
- [Express.js – Middleware](https://expressjs.com/en/guide/using-middleware.html)  
- [Postman – Tests API](https://learning.postman.com/docs/writing-scripts/test-scripts/)

