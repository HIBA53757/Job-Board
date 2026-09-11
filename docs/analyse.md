# Analyse du cahier des charges

## 1. Objectif

Créer un portail web permettant de centraliser les offres de stage et d'alternance pour les apprenants de la formation MERN.

## 2. Utilisateurs

* **Visiteur :** consulter les offres publiques.
* **Apprenant :** rechercher, filtrer, consulter et suivre les offres.
* **Administrateur :** créer, modifier et supprimer les offres.

## 3. Fonctionnalités principales

* Consulter la liste des offres.
* Rechercher une offre par mot-clé.
* Filtrer par ville, technologie et type de contrat.
* Trier les offres par date.
* Consulter le détail d'une offre.
* Ajouter ou retirer une offre des offres suivies.
* Déposer une offre.
* Administrer les offres.

## 4. Pages principales

* Liste des offres
* Détail d'une offre
* Déposer une offre
* Offres suivies
* Administration

## 5. Données principales

Le portail repose principalement sur trois entités :

* **Offre**
* **Entreprise**
* **Technologie**

Une entreprise peut publier plusieurs offres et une offre peut être associée à plusieurs technologies.

## 6. Contraintes

L'interface doit être :

* claire et simple ;
* responsive sur mobile, tablette et desktop ;
* cohérente entre les différentes pages ;
* accessible sans authentification.

## 7. Hors périmètre

La première version n'inclut pas :

* authentification ;
* comptes utilisateurs ;
* backend ;
* API ;
* base de données ;
* candidature en ligne ;
* upload de CV ;
* paiement ;
* messagerie.

## 8. Priorités du brief

Pour cette première étape, l'intégration se concentre sur :

1. Liste des offres
2. Détail d'une offre
3. Dépôt d'une offre
4. Offres suivies
5. Navigation cohérente
6. Design responsive
7. Structure HTML prête pour les futures fonctionnalités JavaScript et backend
