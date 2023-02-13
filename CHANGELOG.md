# Wipimo.WipADB.API Changelog
## 2023.02.1
### New
- Ajout de la route "../cli/Personne/{id}/roles" qui retourne une liste de roles par catégories d'une personne :  bail, mandant, fournisseur
### Breaking changes
- Remplacement des enumerations en valeurs numériques
ex : "MediaPrefere": 10
## 2023.01.2
### New
- Ajout de la route "../cli/Personne/search" avec recherche par nom/prenom, adresse email, téléphone (fixe ou mobile)  
ex : ../cli/personne/search/search?nomprenom=toto
### Breaking changes
- Supression du tri des medias par ordre de préférence dans les réponses des routes "../cli/Personne"
