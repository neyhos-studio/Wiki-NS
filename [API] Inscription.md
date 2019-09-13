# Utilisation de l'API inscription

  - URL : https://localhost:5001/api/Utilisateurs/Inscription
  - Il faut envoyer un [Object] avec toutes les informations, le Back s'occupe ensuite de scinder l'objet en 2, pour faire les bonnes insertions en DB

JSON SEND

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
        "genderUser": "M",
        "secretQuestionUser": "Secret Question",
        "secretAnswerUser": "Secret Answer"
      }
    }
