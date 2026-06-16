# projet-personnel
# 1 Titre du projet
Dweelo — Application web de mise en relation entre chercheurs de logements et propriétaires au Cameroun.

# 2. Le problème
La recherche de logement au Cameroun, notamment à Douala et Yaoundé, est un parcours du combattant. Les personnes qui cherchent un toit doivent souvent :
→ Se déplacer dans plusieurs quartiers sans garantie de disponibilité
→ Contacter de nombreux propriétaires via le bouche-à-oreille ou des affichages papier
→ Faire face à des informations incomplètes, inexactes ou frauduleuse

# 3. Cible (Utilisateurs)

| Acteur   | Profil cible                                                                                               | 
|----------|------------------------------------------------------------------------------------------------------------|
| Chercheur    |Etudiant , jeune actif , famille , travailleur migrant dans une nouvelle ville (Douala , Yaoundé ,...   |
| Propriétaire | Particulier ou agence souhaitant publier et gérer ses annonces en ligne sans intermédiaire    |
| Administrateur   | Gestionnaire de la plateforme chargé dz validder les annonces et garantir la qualité des données     | 

# 4. Proposition de valeur
Dweelo centralise les annonces immobilières camerounaises en un seul endroit, avec des informations vérifiées, des photos réelles et la possibilité de demander une visite directement en ligne — sans se déplacer à l'aveugle.

# 5. Fonctionnalités MVP
Les fonctionnalités minimales pour que l'application soit utile et utilisable dès le lancement :
Authentification : Inscription et connexion sécurisée pour chercheurs et propriétaires
Gestion des annonces : Création, modification et suppression d'annonces par les propriétaires
Recherche avec filtres : Filtrer par ville, quartier, prix, type de logement et nombre de pièces
Demande de visite : Formulaire pour choisir une date et une heure de visite en ligne
Validation admin : L'administrateur valide ou rejette chaque annonce avant publication

# 6. Fonctionnalités Bonus
→ Gestion des favoris : sauvegarder les annonces intéressantes
→ Notifications de statut : confirmation ou refus de visite
→ Avis sur les logements par les anciens locataires
→ Partage d'annonce via lien ou WhatsApp
→ Mode hors-ligne : consultation des dernières annonces en cache

# 7. Écrans / Pages
Accueil : Barre de recherche rapide + annonces récentes + filtre
Liste des annonces : Grille de logements filtrables avec carte/prix/photo
Détail annonce : Photos, description complète, commodités, bouton « Demander une visite »
Formulaire visite : Sélection de date/heure + message pour le propriétaire
Profil / Tableau de bord : Gestion des annonces (propriétaire) ou favoris (chercheur)
Connexion / Inscription : Formulaires d'authentification par rôle
Admin — Validation : Liste des annonces en attente + boutons valider/rejeter

# 8. Données Manipulées
Objets principaux gérés dans l'application (données simulées en frontend) :
## a)	Logement
Titre     (String)   , Type Logement (string) , Localisation(string), Prix    (number) , Description /nbre pièce (sting) , Photos  (UrL) , Commodités(object) , Disponible   (booléen) , Contact      (string)
b)	Utililisateur
Id (string) , nom(string) ,email(string) , role(string)

# 9. Stack Technique
•	Angular
•	TypeScript
•	Json/localStorage
•	Angular router
•	Material/ailwind

# 10. Contrainte Connexion
L'application doit rester utilisable dans les conditions de connectivité camerounaises (réseau 3G lent, coupures fréquentes) 
→ Données légères : images optimisées, pagination des annonces
→ Stockage local : les annonces consultées récemment sont mises en cache via LocalStorage
→ Pas de dépendance à un serveur externe : toutes les données sont simulées en frontend

