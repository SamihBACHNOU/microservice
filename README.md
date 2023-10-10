# microservice
Microservices avec un système de e-commerce


### Analyse et Conception :

1. **Fonctionnalités Principales** :
    - **Produits** : Ajout, suppression, mise à jour et recherche de produits.
    - **Utilisateurs** : Inscription, connexion, mise à jour du profil et suppression.
    - **Commandes** : Création, mise à jour et suppression de commandes.
    - **Paiements** : Simuler le traitement des paiements.

2. **Conception de la Base de Données** :
    - **Produits** : Table avec les détails des produits.
    - **Utilisateurs** : Table avec les détails des utilisateurs.
    - **Commandes** : Table avec les détails des commandes et une référence aux produits et utilisateurs.

### Mise en Œuvre des Services :

1. **Développement des Microservices** :
    - Utilisez Spring Boot (Java) ou Express (Node.js) pour développer chaque microservice.
    - Intégrez MongoDB ou PostgreSQL pour le stockage des données.

2. **Communication entre les Services** :
    - Utilisez des API RESTful ou gRPC pour la communication entre les services.
    - Service de **Commandes** :
        - Communique avec le service **Produits** pour vérifier la disponibilité des produits lors de la création d'une commande.
        - Communique avec le service **Utilisateurs** pour associer une commande à un utilisateur.

### Tests :

1. **Scénarios de Test** :
    - Pour le service **Produits**, testez l'ajout, la suppression, la mise à jour et la recherche de produits.
    - Pour le service **Utilisateurs**, testez l'inscription, la connexion, la mise à jour du profil et la suppression.
    - Pour le service **Commandes**, testez la création, la mise à jour et la suppression de commandes.
    - Testez également les scénarios de communication entre les services.

### Rendu :

1. **Code Source** :
    - Fournissez le code source de chaque microservice dans des répertoires séparés.

2. **Documentation de l'API** :
    - Pour chaque service, documentez les points de terminaison (endpoints) et les méthodes disponibles.

3. **Script de Base de Données** :
    - Fournissez des scripts pour créer les tables nécessaires dans la base de données pour chaque service.

4. **Rapport** :
    - Détaillez les défis rencontrés et les solutions adoptées lors du développement.
    - Expliquez votre choix pour les outils et les technologies.
    - Décrivez les scénarios de test et les résultats obtenus.

### Bonus :

1. **Service d'Authentification basé sur JWT** :
    - Intégrez un service d'authentification basé sur JSON Web Tokens (JWT) pour sécuriser les endpoints des services.

2. **Utilisation de Docker** :
    - Conteneurisez chaque microservice en utilisant Docker.
    - Créez un script Docker-Compose pour démarrer l'ensemble du système avec une seule commande.
