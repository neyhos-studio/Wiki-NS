# Utilisation de l'API update

  - URL https : https://localhost:5001/api/Update/Upload
  - URL http : http://localhost:5000/api/Update/Upload
  - Il faut envoyer un [Object] upload :

OBJECT SEND

    {
        "versionUpdate": "x.x.x",
        "typeUpdate": "PROD",
        "auteurUpdate": "Exemple",
        "dateUpdate": "yyyy-MM-dd"
    }   

RESPONSE

    true si tout c'est bien passé
