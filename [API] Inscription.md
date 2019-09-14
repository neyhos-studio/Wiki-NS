# Utilisation de l'API inscription

  - URL https : https://localhost:5001/api/Utilisateurs/Inscription
  - URL http : http://localhost:5000/api/Utilisateurs/Inscription
  - Il faut envoyer un [Object] composé de 2 [Object] :
      - Un [Object] account (avec Email / Password)
      - Un [Object] user    (avec les autres informations, le back s'occupe de récupérer l'ID de l'account inséré)

OBJECT SEND

    {
      "account": {
        "emailAccount": "exemple@exemple.com",
        "passwordAccount": "exemple"
      },
      "user": {
        "nicknameUser": "exemple",
        "firstNameUser": "exemple",
        "lastNameUser": "exemple",
        "birthdayUser": "yyyy-MM-dd",
        "genderUser": "M"
      }
    }
