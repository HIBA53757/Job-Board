
# Jira Project Export: Job Board (JB)

## Overview Table

| Key | Type | Summary | Status | Priority | Parent |
| --- | --- | --- | --- | --- | --- |
| JB-1 | Epic | Consultation et découverte des offres | To Do | High | - |
| JB-2 | Epic | Suivi des offres et dépôt d'offre | To Do | High | - |
| JB-3 | Epic | Dynamisation JavaScript (préparation Brief 2) | To Do | Medium | - |
| JB-4 | Epic | Fullstack Express/EJS/MySQL (préparation Brief 3) | To Do | Medium | - |
| JB-5 | Story | En tant qu'apprenant, je veux voir la liste des offres pour repérer rapidement les opportunités disponibles | To Do | Highest | JB-1 |
| JB-6 | Story | En tant qu'apprenant, je veux ouvrir le détail d'une offre pour connaître toutes les informations avant de postuler | To Do | Highest | JB-1 |
| JB-7 | Story | En tant qu'apprenant, je veux filtrer les offres par ville, technologie et type de contrat pour trouver des offres pertinentes | To Do | Medium | JB-1 |
| JB-8 | Story | En tant qu'apprenant, je veux rechercher une offre par mot-clé pour retrouver rapidement une opportunité précise | To Do | Medium | JB-1 |
| JB-9 | Story | En tant qu'apprenant, je veux trier les offres par date de publication pour voir les plus récentes en premier | To Do | Low | JB-1 |
| JB-10 | Story | En tant qu'apprenant, je veux marquer une offre comme suivie pour la retrouver plus tard | To Do | High | JB-2 |
| JB-11 | Story | En tant qu'apprenant, je veux consulter une page "offres suivies" pour retrouver mes opportunités enregistrées | To Do | High | JB-2 |
| JB-12 | Story | En tant qu'entreprise/recruteur, je veux déposer une offre via un formulaire pour publier une opportunité | To Do | High | JB-2 |
| JB-13 | Story | En tant que visiteur, je veux naviguer entre les pages du portail de façon cohérente | To Do | High | JB-1 |
| JB-14 | Story | En tant qu'utilisateur, je veux une interface responsive pour consulter le portail sur mobile, tablette et desktop | To Do | High | JB-1 |
| JB-15 | Story | En tant qu'administrateur, je veux un aperçu de l'interface d'administration des offres (Figma) pour anticiper la gestion CRUD | To Do | Medium | JB-4 |
| JB-16 | Subtask | Intégrer index.html (liste des offres) avec cartes statiques | To Do | Highest | JB-5 |
| JB-17 | Subtask | Intégrer offre-detail.html | To Do | Highest | JB-6 |
| JB-18 | Subtask | Ajouter zone filtres/recherche/tri statique sur index.html | To Do | Medium | JB-7 |
| JB-19 | Subtask | Créer composant "carte d'offre" réutilisable en CSS | To Do | High | JB-5 |
| JB-20 | Subtask | Intégrer bouton/icône "suivre" (états visuels) sur cartes et fiche détail | To Do | High | JB-10 |
| JB-21 | Subtask | Intégrer offres-suivies.html | To Do | High | JB-11 |
| JB-22 | Subtask | Intégrer deposer-offre.html (formulaire complet) | To Do | High | JB-12 |
| JB-23 | Subtask | Créer header/nav/footer communs et les inclure sur les 4 pages | To Do | High | JB-13 |
| JB-24 | Subtask | Définir variables CSS globales (couleurs, typo, espacements) dans style.css | To Do | Highest | JB-14 |
| JB-25 | Subtask | Tester le responsive sur les 4 pages (mobile, tablette, desktop) | To Do | High | JB-14 |
| JB-26 | Task | Rédiger l'analyse du cahier des charges (docs/analyse-cahier-des-charges.md) | In Progress | Highest | - |
| JB-27 | Task | Concevoir les maquettes Figma (parcours, wireframes, desktop/mobile, design system) | To Do | Highest | - |
| JB-28 | Subtask | Intégrer le champ de recherche mot-clé (HTML/CSS) | To Do | Medium | JB-8 |
| JB-29 | Subtask | Intégrer le contrôle de tri par date (HTML/CSS) | To Do | Low | JB-9 |
| JB-30 | Subtask | Maquetter les écrans back-office (liste + formulaire admin) sur Figma | To Do | Medium | JB-15 |

---

## Detailed Issues Hierarchy

###  Epic: [JB-1] Consultation et découverte des offres
- **Status:** To Do | **Priority:** High
- **Description:** Permettre à l'utilisateur (apprenant/visiteur) de consulter la liste des offres, d'ouvrir le détail d'une offre, de filtrer et de trier les résultats selon plusieurs critères (ville, technologie, type de contrat, mot-clé, date).

Périmètre brief 1 : intégration statique HTML/CSS (liste, détail). Filtres/tri = structure visuelle prête, logique dynamique en Brief 2.

####  Story: [JB-5] En tant qu'apprenant, je veux voir la liste des offres pour repérer rapidement les opportunités disponibles
- **Status:** To Do | **Priority:** Highest
- **Description:**
*User story*
En tant qu'apprenant, je veux consulter une liste d'offres de stage/alternance afin de voir rapidement ce qui est disponible.

*Critères d'acceptation*

* Étant donné que j'arrive sur la page d'accueil, je vois une liste de cartes d'offres.
* Chaque carte affiche : titre du poste, entreprise, ville, type de contrat, technologies principales, date de publication, description courte.
* Chaque carte permet d'accéder à la fiche détaillée de l'offre.
* La liste reste lisible sur mobile, tablette et desktop.
* Un jeu d'au moins 8 à 10 offres fictives mais réalistes est affiché.

  **Sub-tasks:**
  * **[JB-16]** Intégrer index.html (liste des offres) avec cartes statiques *(To Do | Highest)* - Créer la structure HTML sémantique (header, nav, main, section, article, footer) et le CSS (Flexbox/Grid, variables CSS) pour la page liste des offres, avec 8 à 10 offres fictives en dur.
  * **[JB-19]** Créer composant "carte d'offre" réutilisable en CSS *(To Do | High)* - Définir le composant carte d'offre (structure HTML + classes CSS réutilisables) : image/logo, titre, entreprise, ville, badge technologie, badge type de contrat, date, bouton suivre. Utiliser des variables CSS pour la cohérence visuelle.

####  Story: [JB-6] En tant qu'apprenant, je veux ouvrir le détail d'une offre pour connaître toutes les informations avant de postuler
- **Status:** To Do | **Priority:** Highest
- **Description:**
*User story*
En tant qu'apprenant, je veux consulter la fiche détaillée d'une offre afin de connaître la mission, le profil recherché et les modalités de candidature.

*Critères d'acceptation*

* Depuis une carte offre, un clic ouvre la fiche détail correspondante.
* La fiche affiche : titre, entreprise, localisation, type de contrat, technologies demandées, description complète, profil recherché, infos de candidature, date de publication.
* Un lien ou bouton permet de revenir facilement à la liste des offres.
* La page reste lisible sur mobile, tablette et desktop.

  **Sub-tasks:**
  * **[JB-17]** Intégrer offre-detail.html *(To Do | Highest)* - Créer la structure HTML/CSS de la fiche détail offre (article sémantique, sections mission/profil/candidature) + lien retour vers la liste.

####  Story: [JB-7] En tant qu'apprenant, je veux filtrer les offres par ville, technologie et type de contrat pour trouver des offres pertinentes
- **Status:** To Do | **Priority:** Medium
- **Description:**
*User story*
En tant qu'apprenant, je veux filtrer les offres selon plusieurs critères combinables afin de réduire la liste à ce qui m'intéresse.

*Critères d'acceptation*

* La structure visuelle des filtres (ville, technologie, type de contrat) est présente sur la page liste.
* Les filtres peuvent visuellement être combinés (zone dédiée, formulaire).
* La logique de filtrage dynamique n'est pas requise en Brief 1 (JS ajouté en Brief 2) : le HTML/CSS doit être prêt à recevoir cette logique.
* Un message "aucun résultat" est prévu visuellement pour le cas où aucune offre ne correspond.

  **Sub-tasks:**
  * **[JB-18]** Ajouter zone filtres/recherche/tri statique sur index.html *(To Do | Medium)* - Intégrer visuellement la zone de filtres (ville, technologie, type de contrat), le champ de recherche et le contrôle de tri, avec structure form et attributs prêts pour le JS du Brief 2. Prévoir un état "aucun résultat".

####  Story: [JB-8] En tant qu'apprenant, je veux rechercher une offre par mot-clé pour retrouver rapidement une opportunité précise
- **Status:** To Do | **Priority:** Medium
- **Description:**
*User story*
En tant qu'apprenant, je veux rechercher une offre par mot-clé (titre, entreprise, description) afin de gagner du temps.

*Critères d'acceptation*

* Un champ de recherche est visuellement présent sur la page liste.
* Le champ est stylé et positionné de façon cohérente avec les filtres.
* La logique de recherche dynamique sera ajoutée en Brief 2 ; le HTML doit être prêt (attribut name, id, structure form).

  **Sub-tasks:**
  * **[JB-28]** Intégrer le champ de recherche mot-clé (HTML/CSS) *(To Do | Medium)* - Intégrer le champ de recherche (input type="search", label associé, icône loupe) dans la zone filtres de index.html. Ajouter un attribut name/id clair pour la future logique JS (Brief 2). Style cohérent avec le reste des filtres.

####  Story: [JB-9] En tant qu'apprenant, je veux trier les offres par date de publication pour voir les plus récentes en premier
- **Status:** To Do | **Priority:** Low
- **Description:**
*User story*
En tant qu'apprenant, je veux trier les offres par date de publication afin de prioriser les opportunités les plus récentes.

*Critères d'acceptation*

* Un contrôle de tri (select ou boutons) est visuellement présent sur la page liste.
* La date de publication est affichée sur chaque carte offre.
* La logique de tri dynamique sera ajoutée en Brief 2 ; le HTML est prêt pour recevoir cette interaction.

  **Sub-tasks:**
  * **[JB-29]** Intégrer le contrôle de tri par date (HTML/CSS) *(To Do | Low)* - Intégrer un contrôle de tri (select avec options "plus récent / plus ancien") dans la zone filtres de index.html. Ajouter un id clair pour la future logique JS (Brief 2). Style cohérent avec le reste des filtres.

####  Story: [JB-13] En tant que visiteur, je veux naviguer entre les pages du portail de façon cohérente
- **Status:** To Do | **Priority:** High
- **Description:**
*User story*
En tant que visiteur, je veux une navigation claire et cohérente entre les pages afin de comprendre où je me trouve et où aller.

*Critères d'acceptation*

* Un header/nav commun est présent sur toutes les pages (liste, détail, dépôt, offres suivies).
* Les liens de navigation utilisent des balises sémantiques (header, nav, footer).
* L'état actif de la page courante est visuellement indiqué dans la navigation.
* La navigation est responsive (menu adapté sur mobile).

  **Sub-tasks:**
  * **[JB-23]** Créer header/nav/footer communs et les inclure sur les 4 pages *(To Do | High)* - Créer le composant navigation (header, nav, footer) avec logo, liens (accueil, dépôt, offres suivies), état actif, et menu responsive (burger sur mobile). L'intégrer de façon cohérente sur index.html, offre-detail.html, deposer-offre.html, offres-suivies.html.

####  Story: [JB-14] En tant qu'utilisateur, je veux une interface responsive pour consulter le portail sur mobile, tablette et desktop
- **Status:** To Do | **Priority:** High
- **Description:**
*User story*
En tant qu'utilisateur, je veux que toutes les pages du portail s'adaptent à la taille de mon écran afin de consulter les offres confortablement partout.

*Critères d'acceptation*

* Chaque page (liste, détail, dépôt, offres suivies) est testée et fonctionnelle sur mobile, tablette et desktop.
* Utilisation de Flexbox et/ou Grid pour les mises en page.
* Utilisation de variables CSS pour les couleurs, espacements et typographie.
* Les contrastes texte/fond restent lisibles à toutes les tailles d'écran.

  **Sub-tasks:**
  * **[JB-24]** Définir variables CSS globales (couleurs, typo, espacements) dans style.css *(To Do | Highest)* - Créer le fichier css/style.css avec :root { --variables } pour couleurs primaires/secondaires, typographie, espacements, rayons de bordure. Vérifier les contrastes (WCAG AA minimum) sur tous les textes.
  * **[JB-25]** Tester le responsive sur les 4 pages (mobile, tablette, desktop) *(To Do | High)* - Vérifier via DevTools (breakpoints ~375px, 768px, 1280px) que les 4 pages restent lisibles et fonctionnelles. Corriger les débordements, ajuster les media queries.

###  Epic: [JB-2] Suivi des offres et dépôt d'offre
- **Status:** To Do | **Priority:** High
- **Description:** Permettre à l'utilisateur de marquer/retirer une offre comme suivie (stockage navigateur, sans compte) et de proposer un formulaire de dépôt d'offre (statique en Brief 1, alimente la gestion en version complète).

####  Story: [JB-10] En tant qu'apprenant, je veux marquer une offre comme suivie pour la retrouver plus tard
- **Status:** To Do | **Priority:** High
- **Description:**
*User story*
En tant qu'apprenant, je veux marquer une offre comme "suivie" afin de la retrouver facilement plus tard sans créer de compte.

*Critères d'acceptation*

* Un bouton/icône "suivre" est présent sur chaque carte offre et sur la fiche détail.
* L'état visuel (suivi / non suivi) est visuellement différencié (icône pleine/vide, badge, couleur).
* Aucune authentification n'est requise (règle de gestion : suivi propre au navigateur).
* La persistance réelle (stockage navigateur) sera implémentée en Brief 2 ; le Brief 1 livre la structure HTML/CSS et les états visuels.

  **Sub-tasks:**
  * **[JB-20]** Intégrer bouton/icône "suivre" (états visuels) sur cartes et fiche détail *(To Do | High)* - Ajouter le bouton suivre avec ses deux états visuels (suivi/non suivi) via classes CSS, sur la carte offre et sur la fiche détail. Prévoir data-attributes pour la logique JS du Brief 2.

####  Story: [JB-11] En tant qu'apprenant, je veux consulter une page "offres suivies" pour retrouver mes opportunités enregistrées
- **Status:** To Do | **Priority:** High
- **Description:**
*User story*
En tant qu'apprenant, je veux une page dédiée regroupant les offres que j'ai marquées comme suivies.

*Critères d'acceptation*

* Une page "offres-suivies.html" statique existe et reprend le même format de carte que la liste principale.
* Un bouton permet de retirer une offre de la liste de suivi (structure prévue, logique dynamique en Brief 2).
* Un état vide ("aucune offre suivie") est prévu visuellement.
* La navigation vers cette page est accessible depuis le header/nav sur toutes les pages.

  **Sub-tasks:**
  * **[JB-21]** Intégrer offres-suivies.html *(To Do | High)* - Créer la page statique reprenant le composant carte d'offre, avec état vide "aucune offre suivie" et bouton retirer.

####  Story: [JB-12] En tant qu'entreprise/recruteur, je veux déposer une offre via un formulaire pour publier une opportunité
- **Status:** To Do | **Priority:** High
- **Description:**
*User story*
En tant qu'entreprise, je veux remplir un formulaire de dépôt d'offre afin de proposer une opportunité sur le portail.

*Critères d'acceptation*

* La page "deposer-offre.html" contient un formulaire avec : nom entreprise, titre du poste, ville, type de contrat, technologies demandées, description de la mission, profil recherché, contact/lien de candidature.
* Le formulaire utilise des balises sémantiques (form, label, fieldset si pertinent).
* Le formulaire est responsive et lisible sur mobile.
* Le formulaire est uniquement représenté visuellement (aucun traitement/soumission réel n'est requis en Brief 1).

  **Sub-tasks:**
  * **[JB-22]** Intégrer deposer-offre.html (formulaire complet) *(To Do | High)* - Créer le formulaire de dépôt d'offre en HTML sémantique avec tous les champs requis, labels associés, validation HTML native (required, type), style cohérent avec le reste du site.

###  Epic: [JB-3] Dynamisation JavaScript (préparation Brief 2)
- **Status:** To Do | **Priority:** Medium
- **Description:** Préparer la structure HTML/CSS et l'organisation des données pour permettre l'ajout de la logique JavaScript dynamique lors du Brief 2 : filtres, tri, suivi d'offres en JS, manipulation du DOM.

Hors périmètre Brief 1 : le JS dynamique lui-même. Ce qui est attendu ici = préparation (data-attributes, structure sémantique, classes prévues pour les états).

###  Epic: [JB-4] Fullstack Express/EJS/MySQL (préparation Brief 3)
- **Status:** To Do | **Priority:** Medium
- **Description:** Préparer l'architecture de données (schéma Offre/Entreprise/Technologie) et l'arborescence de vues pour la bascule vers un backend Express/EJS/MySQL en Brief 3 : CRUD offres, relations entreprise-technologie, administration.

Hors périmètre Brief 1 : implémentation backend réelle. Ce qui est attendu ici = modélisation conceptuelle des données et anticipation de la structure de vues EJS.

####  Story: [JB-15] En tant qu'administrateur, je veux un aperçu de l'interface d'administration des offres (Figma) pour anticiper la gestion CRUD
- **Status:** To Do | **Priority:** Medium
- **Description:**
*User story*
En tant qu'administrateur, je veux visualiser (en maquette Figma) les écrans permettant de consulter, créer, modifier et supprimer une offre, afin de préparer la gestion des offres en Brief 3.

*Critères d'acceptation*

* Un back-office minimal est représenté dans le fichier Figma (liste des offres avec actions, formulaire création/édition).
* L'écran permet de visualiser l'association d'une ou plusieurs technologies à une offre.
* Hors périmètre Brief 1 : aucune implémentation HTML/CSS ou logique réelle n'est requise, uniquement la maquette.

  **Sub-tasks:**
  * **[JB-30]** Maquetter les écrans back-office (liste + formulaire admin) sur Figma *(To Do | Medium)* - Sur Figma : créer les écrans "liste des offres (vue admin)" avec actions modifier/supprimer, et "formulaire création/édition d'offre" avec sélection des technologies associées. Ceci prépare la vue EJS du Brief 3, pas d'intégration HTML/CSS ici.

###  General Tasks

####  Task: [JB-26] Rédiger l'analyse du cahier des charges (docs/analyse-cahier-des-charges.md)
- **Status:** In Progress | **Priority:** Highest
- **Description:**
Reformuler le besoin produit, identifier les utilisateurs (apprenant, visiteur, administrateur) et leurs parcours, lister les règles de gestion clés, produire l'arborescence de l'application.

####  Task: [JB-27] Concevoir les maquettes Figma (parcours, wireframes, desktop/mobile, design system)
- **Status:** To Do | **Priority:** Highest
- **Description:**
Créer le fichier Figma : parcours utilisateurs, arborescence, wireframes basse fidélité, maquettes desktop/mobile pour les écrans publics, back-office minimal, composants réutilisables (carte offre, bouton, champ, badge techno, navigation), cohérence visuelle (couleurs, typo, espacements, états).
jira-export.md
Displaying jira-export.md.