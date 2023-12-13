# Wipimo.WipADB.API Changelog
## 2023.12.1
### New
- Ajout de la route "../cli/societe" qui retourne une liste des sociétés
### Breaking changes
- Sur la route "../ger/mandant" obligation de renseigner l'IdSociete
## 2023.02.2
### New
- Ajout de la route "../cli/Personne/searchRoles" similaire à la fonctionnalité de recherche globale de Wipimo. Elle permet une recherche parmis les rôles Personnes, PersRelation, Mandants, Baux et Fournisseurs en utilisant un nom complet ou partiel, une adresse email, un numéro de téléphone, tout ou partie d'une d'adresse postale, l'Id d'une personne.
## 2023.02.1
### New
- Ajout de la route "../cli/Personne/{id}/roles" qui retourne une liste de roles par catégories d'une personne :  bail, mandant, fournisseur
### Breaking changes
- Remplacement des enumerations en valeurs numériques
- Les DTO sont formatés en PascalCase comme le modèle de données Wipimo
ex : "MediaPrefere": 10
## 2023.01.2
### New
- Ajout de la route "../cli/Personne/search" avec recherche par nom/prenom, adresse email, téléphone (fixe ou mobile)  
ex : ../cli/personne/search/search?nomprenom=toto
### Breaking changes
- Supression du tri des medias par ordre de préférence dans les réponses des routes "../cli/Personne"
