# app
Application Flask : Gestion des utilisateurs
Description
Cette application propose un système de gestion des utilisateurs comprenant des fonctionnalités telles que l'inscription, la connexion, la réinitialisation de mot de passe via OTP, la gestion de profils et une recherche avancée. L'application est conçue pour offrir une interface utilisateur conviviale et responsive, ainsi qu'une architecture robuste côté serveur.

Fonctionnalités principales
Inscription et Connexion : Création et authentification sécurisées des utilisateurs.
Réinitialisation de mot de passe : Utilisation d'un OTP envoyé par email.
Gestion des profils : Modification des informations personnelles et ajout d'images de profil.
Recherche avancée : Recherche par critères, comme le service ou la localisation.
Sécurité : Validation des données et gestion des erreurs utilisateur.
Outils et technologies de développement
Langages et frameworks
Python : Développement de la logique métier et manipulation des données.
Flask : Framework léger pour le développement rapide d'applications web.
JavaScript : Interactivité côté client (par exemple, chronomètres pour les quiz).
HTML & CSS : Structure et mise en forme des pages web pour une expérience utilisateur cohérente.
Bootstrap : Framework front-end pour des interfaces modernes et responsives.
Environnement de développement
Visual Studio : IDE polyvalent utilisé pour écrire, déboguer et gérer le projet.
Outils et technologies de base de données
SQLite : Base de données légère et autonome, parfaite pour les projets nécessitant une solution locale simple et performante.
DB Browser for SQLite : Interface graphique intuitive pour gérer et éditer les bases de données SQLite.
Autres outils utilisés
GitHub : Plateforme pour le versionnement et la collaboration sur le code source.
Lucidchart : Création de diagrammes conceptuels pour la modélisation des données et des processus.
Installation
Étape 1 : Cloner le dépôt

git clone https://github.com/votre-repo.git  
cd votre-repo  
Étape 2 : Créer un environnement virtuel

python -m venv env  
source env/bin/activate   # Sous Linux/macOS  
env\Scripts\activate      # Sous Windows  
Étape 3 : Installer les dépendances

pip install -r requirements.txt  
Étape 4 : Configurer la base de données
Initialisez la base de données SQLite :

python
Copier le code
python -c "from app import create_user_table; create_user_table()"  
Étape 5 : Configurer les paramètres SMTP
Mettez à jour les paramètres dans app.py :


app.config['MAIL_SERVER'] = 'smtp.votre-serveur.com'  
app.config['MAIL_PORT'] = 587  
app.config['MAIL_USERNAME'] = 'votre_email@example.com'  
app.config['MAIL_PASSWORD'] = 'votre_mot_de_passe'  
Lancer l'application
Démarrer le serveur

python app.py  
Accéder à l'application
Rendez-vous sur : http://127.0.0.1:5000.
