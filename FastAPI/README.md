# Public-
API 
Installation
Téléchargez et installez Python 3.7+ sur votre ordinateur si vous ne l'avez pas déjà installé.

Clonez ou téléchargez le fichier ZIP de ce dépôt GitHub.

shell
Copy code
$ git clone https://github.com/<USERNAME>/<REPO_NAME>.git
OU

Téléchargez et extrayez le fichier ZIP du code source de l'API.

Ouvrez un terminal et accédez au répertoire racine de l'API.

shell
Copy code
$ cd <REPO_NAME>
Installez les dépendances nécessaires à l'aide de pip.

ruby
Copy code
$ pip install -r requirements.txt
Exécution
Une fois les dépendances installées, exécutez l'API en exécutant la commande suivante :

css
Copy code
$ uvicorn main:app --reload
L'API sera désormais accessible à l'adresse http://localhost:8000 dans votre navigateur Web.

Utilisation
L'API dispose de plusieurs points de terminaison que vous pouvez utiliser pour interagir avec elle. Voici quelques exemples de requêtes que vous pouvez effectuer :

Pour obtenir la page d'accueil de l'API, accédez à http://localhost:8000/.
Pour obtenir une liste de nombres aléatoires, accédez à http://localhost:8000/val?nb=10 (remplacez 10 par le nombre de nombres aléatoires que vous souhaitez obtenir).
Pour ajouter deux nombres, accédez à http://localhost:8000/calc/add?n1=2&n2=3 (remplacez 2 et 3 par les nombres que vous souhaitez ajouter).
Pour afficher une image, accédez à http://localhost:8000/img?num=1 (remplacez 1 par le numéro de l'image que vous souhaitez afficher).
Pour obtenir des informations sur une station de vélo-partage, accédez à http://localhost:8000/stations_velo?id=1&addr=True&cap=True (remplacez 1 par l'ID de la station que vous souhaitez rechercher). Pour obtenir toutes les informations sur toutes les stations de vélo-partage, accédez à http://localhost:8000/stations_velo?id=toutes&cap=.
C'est tout ce qu'il y a à savoir pour installer et exécuter cette API FastAPI. 
