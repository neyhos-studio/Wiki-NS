# Game session and token

### Definition

Une session c'est le maintient de l'état d'une entitée (client) par raport a un réceptacle (serveur, logiciel, machine) sur une periode de temps définie par le réceptacle.

### Le fonctionnement

Une session peut être maintenue dans le temps de différentes façons, 
nous aborderons ici la session maintenue par un système de token.

A l'authentification d'une entitée au réceptacle, ce dernier lui renvoie un token qui fait le lien entre l'entitée et la session ;
Une session est définie par : 

- un compteur décrémental en unitée temporelle ; 
- une durée maximale de temps définie par le réceptacle ;
 
Cette session définit une identitée de confiance à l'entitée envers le réceptacle tant quel est maintenue.
Voici les différents moyens de maintenir un session active en réinitialisant le compteur de temps :

- A l'envoie d'une requête au réceptacle suite à une action de l'utilisateur ;
- A la demande d'un nouvelle état de la par de l'entitée (chargement ou temps d'attente indépendant de l'utilisateur) ;

Voici les différents évènement pouvant interrompre une session active :

- Le réceptacle ne parvient pas à contacter l'entitée (perte de connexion entre l'entitée et le récéptacle) ;
- L'entitée demande au réceptacle d'interrompre la session (demande de déconnexion de l'entitée) ;
- Le réceptacle ne reconnait pas le token de l'entitée et interrompt la session (Tentative de connexion sans token/avec un token non reconnue ou présence d'une session ouverte par l'entitée avec un autre token) ;

