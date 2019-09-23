# Game session and token

### Definition

Une session c'est le maintient de l'état d'une entitée (client) par raport a un réceptacle (serveur, logiciel, machine) sur une période de temps définit par le réceptacle.

### Le fonctionnement

Une session peut être maintenue dans le temps de différentes façons, 
nous aborderons ici la session maintenue par un système de token.

A l'authentification d'une entitée au réceptacle, ce dernier lui renvoie un token qui fait le lien avec une session ;
Une session est définit par : 

- un compteur décrémental en unité de temps ; 
- une durée maximal de temps défini par le réceptacle ;
 
Cette session définit une identité de confiance à l'entité envers le réceptacle tant quel est maintenue.
Voici les diférents moyens de maintenir un session active en réinitialisant le compteur de temps :

- A l'envoie d'une requête au réceptacle suite à une action de l'utilisateur ;
- A la demande d'un nouveau état de la par de l'entité (chargement ou temps d'attente indépendant de l'utilisateur) ;

Voici les differents evenement pouvant interrompre une session active :

- Le réceptacle ne parvient pas à contacter l'entité (perte de connexion entre l'entité et le récéptacle) ;
- L'entitée demande au réceptacle d'intérompre la session (demande de déconnexion de l'entité) ;
- Le réceptacle ne reconnait pas le token de l'entité et intérrompt la session (Tentative de connexion sans token/avec un token non reconnue ou présence d'une session ouverte par l'entité avec un autre token) ;

