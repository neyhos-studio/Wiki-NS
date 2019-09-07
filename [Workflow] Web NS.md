# Connection

### Index

    Depuis l'index, on veux accéder à l'ecran de connexion.
    Le bouton se trouvera dans la top bar et pourra être : (Connexion)
    Le bouton connexion redirige vers l'écran de connexion si on est pas connecté, si on et connecter, un menu deroulan s'afficher avec :
    Profil/Options/Déconnexion.

### Connexion

    L'écran de connexion est dépourvue de top bar, et composé de :
    Un background / Un formulaire central.
    Le formulaire contient les input pour : 
    Email / Password / Connexion / Inscription
    Quand l'utilisateur clique sur connexion, il retourne sur ça page précédente si il est connecté sinon les inputs non valide sont entourer en rouge. et a droite apparai un logo "i" avec quand on met la souris dessus, un message qui dit email non valide/ mot-de-passe non valide

# Inscription

Index -> btn.connexion -> btn.inscription

### Index 

    Depuis l'index, on veux accéder à l'ecran d'inscription.
    Le bouton se trouvera dans la top bar et pourra être : (Inscription)
    Le bouton connexion redirige vers l'écran de d'inscription si on est pas connecté, si on et connecter le bouton n'est pas affiché.

### Inscription

    La même que "Connexion" sauf que le formulaire est composé de :
    Email / Pass / PassConfirm / Pseudo / Nom / Prénom / DateNaissance / 
    QuestionSecrete.1 / ReponseSecrete.1 / QuestionSecrete.2 / ReponseSecrete.2 


<form style="background: #aaa; padding: 20px; display: flex; flex-direction: column" action="url">
    <input type="text" placeholder="Email">
    <input type="text" placeholder="Password">
    <input type="text" placeholder="PasswordVerif">
    <input type="text" placeholder="Nickname">
    <input type="text" placeholder="Nom">
    <input type="text" placeholder="Prenom">
    <input type="date">
    <div>
        <input type="" placeholder="Question">
        <input placeholder="Repoonse">
    </div>
    <div>
        <input type="" placeholder="Question">
        <input placeholder="Repoonse">
    </div>
    <input type="submit">
</from>