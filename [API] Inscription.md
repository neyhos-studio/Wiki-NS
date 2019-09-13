# Utilisation de l'API inscription

  - URL : https://localhost:5001/api/Utilisateurs/Inscription
  - Il faut envoyer un [Object] avec toutes les informations, le Back s'occupe ensuite de scinder l'objet en 2, pour faire les bonnes insertions en DB

JSON SEND

    {
      "account": {
        "emailAccount": "kylian.robba@live.fr",
        "passwordAccount": "bbb"
      },
      "user": {
        "nicknameUser": "Akcess",
        "firstNameUser": "Kylian",
        "lastNameUser": "Robba",
        "birthdayUser": "1994-01-07",
        "genderUser": "m",
        "secretQuestionUser": "Quel est le nom de mon chat ?",
        "secretAnswerUser": "Lequel"
      }
    }
