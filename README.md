# WipADB.API
L'API publique des utilisateurs de Wipimo

## Principe général
Les appels aux différentes ressources de l’API doivent être authentifiés à l’aide d’un token d’accès.

C’est pourquoi, il est nécessaire de s’authentifier à l’API afin d’obtenir un token qui sera utilisé en entrée des appels suivants à l’API.
Le protocole d’authentification utilisé est OAuth 2. Le serveur d’autorisation intercepte la requête de l’utilisateur, vérifie ses droits d’accès, puis renvoie un token d’accès.

Une double vérification de droits est effectuée. 

La première avec votre client_id et votre client_secret. Votre client_id est votre domaine client Wipimo, le client_secret vous sera communiqué lors de la souscription à l’API.

La seconde avec un email et un mot de passe. Ce sont les informations habituelles de connexion à Wipimo.

Le token d’accès (access_token) reçu devra être insérer dans chaque requête d’appel à l’API dans le Header « Authorization » de type « Bearer ».
