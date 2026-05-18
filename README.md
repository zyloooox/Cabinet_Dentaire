# Cabinet Dentaire Bougatef

## Description
Site web pour un cabinet dentaire avec gestion des patients, rendez-vous et services.

## Équipe
- **Bougatef Azza** - Backend (PHP, MySQL)
- **Ajroud Oussema** - Frontend (JavaScript)

## Technologies
- HTML / CSS
- JavaScript
- PHP / MySQL

## Installation

1. Copier le dossier dans `htdocs` (XAMPP)
2. Importer `database.sql` dans phpMyAdmin
3. Copier `db-config.example.php` → `db-config.php`
4. Accéder à `http://localhost/Cabinet_Dentaire/`

## Fonctionnalités

### Patients
- S'inscrire / se connecter
- Réserver une prestation
- Voir historique des soins
- Modifier son profil

### Médecins / Admin
- Gérer les patients
- Gérer les rendez-vous
- Gérer les services
- Gérer les comptes médecins (2 max)
- Voir les statistiques

## Structure du projet

Cabinet_Dentaire/
│
├── 📁 backend/ # PHP (Bougatef Azza)
│ ├── auth.php # Authentification
│ ├── database.php # Connexion BDD
│ ├── patients.php # CRUD patients
│ ├── rdv-api.php # Gestion rendez-vous
│ ├── services-api.php # Gestion services
│ ├── admin-medecins-api.php # Gestion médecins
│ ├── compte-api.php # Espace patient
│ ├── stats.php # Statistiques
│ ├── database.sql # Structure BDD
│ └── db-config.example.php # Configuration exemple
│
├── 📁 frontend/ # JavaScript (Ajroud Oussema)
│ ├── api-base.js # URL base API
│ ├── nav-auth.js # Menu dynamique
│ ├── gestion-patient.js # CRUD patients
│ ├── gestion-rdv.js # Gestion RDV
│ ├── gestion-services.js # Gestion services
│ ├── gestion-medecins.js # Gestion médecins
│ ├── mon-compte.js # Espace patient
│ ├── inscription-connexion.js # Auth
│ ├── reserver-rdv.js # Réservation
│ ├── services-catalog.js # Catalogue
│ └── index.js # Page accueil
│
├── 📁 html-css/ # Pages statiques
│ ├── index.html
│ ├── medecins.html
│ ├── services.html
│ ├── style.css
│ └── ...
│
└── README.md
