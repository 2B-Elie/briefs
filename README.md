#  Projet API – Authentification & Routes Protégées

## Description
Ce projet a pour objectif de mettre en place un système d’authentification avec **JWT** et de sécuriser certaines routes de l’API.  
Il est composé de deux étapes principales :  
1. Implémenter un système **d’inscription et de connexion**.  
2. Protéger certaines routes afin qu’elles soient accessibles uniquement aux utilisateurs connectés.  


##  Table des matières
- [Brief 1 – Système d’Auth](#brief-1--système-dauth)
- [Brief 2 – Routes Protégées](#brief-2--routes-protégées)


## Brief 1 – Système d’Auth
**Objectif :** Créer les routes `register` et `login` permettant aux utilisateurs de s’inscrire et de se connecter.  
- Génération et renvoi d’un **token JWT**.  
- Middleware pour la gestion et la vérification des tokens.  
 Voir le détail ici : [BRIEF1.md](./BRIEF1.md)


## Brief 2 – Routes Protégées
**Objectif :** Sécuriser certaines routes pour que seuls les utilisateurs authentifiés y aient accès.  
- Création d’un **middleware JWT** pour protéger les endpoints sensibles.  
- Exemple : la route `POST /posts` ne doit être accessible qu’aux utilisateurs connectés.  
 Voir le détail ici : [BRIEF2.md](./BRIEF2.md)
