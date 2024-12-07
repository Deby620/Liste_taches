# Liste_taches

## Contexte du Projet

Liste de Tâches est une application web simple et efficace permettant de gérer les tâches quotidiennes. Les fonctionnalités principales incluent :
-  Gestion des Tâches: Création, lecture, mise à jour et suppression de tâches
-  Marquage des Tâches: Possibilité de marquer les tâches comme terminées/non-terminées
-  Interface Réactive: Mise à jour en temps réel de l'interface utilisateur
-  Design Moderne: Interface utilisateur intuitive et esthétique

## Contributeurs

Ce projet a été développé par Baran à Dan Débora, stagiaire développeuse.

## Technologies

Frontend: React.js avec Vite
Backend: PHP avec PDO
Base de données: MySQL
Serveur: XAMPP

## Structure du Projet

liste-taches/
├── Backend/
│   ├── api/
│   │   └── taches.php
│   └── config/
│       └── Database.php
└── Frontend/
    └── liste_taches/
        ├── src/
        │   ├── App.jsx
        │   ├── App.css
        │   ├── main.jsx
        │   └── index.css
        └── index.html
        
## Installation

### Prérequis

XAMPP (avec PHP et MySQL)
Node.js 
npm 

### 1. Configuration de la Base de Données

  CREATE DATABASE liste_taches;
  USE liste_taches;
  CREATE TABLE taches (
      id INT PRIMARY KEY AUTO_INCREMENT,
      nom VARCHAR(255) NOT NULL,
      terminee BOOLEAN DEFAULT 0
  );
  
### 2. Installation du Backend

git clone https://github.com/Deby620
cp Backend/* c:/xampp/htdocs/Backend/

### 3. Installation du Frontend

cd Frontend/liste_taches
npm install

### 4. Configuration des Variables d'Environnement

Le backend est configuré pour fonctionner avec les paramètres par défaut de XAMPP :
Host: localhost
User: root
Password: (vide)
Database: liste_taches

### 5. Lancer l'Application

#### Démarrer le Backend

Démarrer XAMPP (Apache et MySQL)

#### Démarrer le Frontend

cd Frontend/liste_taches
npm run dev

L'application sera accessible à http://localhost:5173/

## Utilisation

Ajouter une tâche : Saisir le nom dans le champ et cliquer sur "Ajouter"
Marquer comme terminée : Cocher la case à côté de la tâche
Supprimer : Cliquer sur le bouton "Supprimer" de la tâche
