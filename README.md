 Présentation du projet

Le marché des voitures d’occasion présente une grande diversité de prix selon la marque, le modèle, l’année de fabrication, le kilométrage, la motorisation et l’état du véhicule.

L’objectif de ce projet est de développer un système capable d’estimer le prix d’une voiture d’occasion au Maroc à partir de ses caractéristiques.

Le projet suit un pipeline de Machine Learning comprenant :

Collecte des données : extraction d’informations depuis les annonces de voitures d’occasion sur Avito.ma, sous réserve des autorisations applicables.

Prétraitement des données : nettoyage, conversion des valeurs textuelles en données exploitables et traitement des valeurs manquantes.

Analyse exploratoire (EDA) : étude des distributions, des relations entre variables et des valeurs aberrantes.

Feature Engineering : préparation et transformation des variables pertinentes pour la modélisation.

Modélisation prédictive : entraînement et comparaison de plusieurs algorithmes de régression.

Optimisation des modèles : validation croisée et recherche d’hyperparamètres.

Déploiement : création d’une interface interactive avec Streamlit pour tester des estimations de prix.

Important : le prix estimé par le modèle constitue une indication statistique et non une garantie du prix réel de vente.

🎯 Objectifs

Collecter et exploiter des données réelles d’annonces automobiles.

Mettre en pratique les techniques de nettoyage et de préparation des données.

Identifier les caractéristiques qui influencent le prix d’un véhicule.

Comparer différents algorithmes de régression.

Évaluer la qualité des prédictions avec des métriques adaptées.

Construire une application interactive accessible aux utilisateurs.

Mettre en œuvre les différentes étapes d’un projet de Machine Learning de bout en bout.

🛠️ Technologies utilisées

Catégorie

Technologies

Langage

Python

Collecte des données

Requests, BeautifulSoup

Manipulation des données

Pandas, NumPy

Visualisation

Matplotlib, Seaborn

Machine Learning

Scikit-learn

Modèles avancés

Random Forest, XGBoost, CatBoost, LightGBM

Optimisation

K-Fold Cross-Validation, GridSearchCV

Interface web

Streamlit

Environnement

Jupyter Notebook, Git, GitHub

Les bibliothèques sont à conserver dans cette liste uniquement si elles sont effectivement utilisées dans le code du projet.

🔄 Architecture du pipeline

Collecte des annonces automobiles
              │
              ▼
     Nettoyage des données
              │
              ▼
 Analyse exploratoire (EDA)
              │
              ▼
    Feature Engineering
              │
              ▼
 Préparation des données ML
              │
              ▼
 Entraînement et comparaison
       des modèles
              │
              ▼
 Validation et optimisation
              │
              ▼
   Modèle de régression final
              │
              ▼
   Application interactive
          Streamlit
              │
              ▼
    Estimation du prix

🤖 Modèles de Machine Learning

Plusieurs algorithmes de régression peuvent être évalués afin d’identifier celui qui fournit les meilleures estimations sur des données de test.

Modèle

Principe

Linear Regression

Modèle de référence pour étudier les relations linéaires

Random Forest Regressor

Combinaison de plusieurs arbres de décision

XGBoost Regressor

Boosting d’arbres optimisé pour les données tabulaires

CatBoost Regressor

Boosting conçu notamment pour faciliter la gestion des variables catégorielles

LightGBM Regressor

Boosting efficace sur les jeux de données tabulaires

Le choix du modèle final doit reposer sur les résultats réels de validation et de test, ainsi que sur sa capacité à généraliser à de nouvelles annonces.

Métriques d’évaluation

MAE (Mean Absolute Error) : mesure l’erreur absolue moyenne des prédictions, exprimée en dirhams si la cible est en MAD.

RMSE (Root Mean Squared Error) : pénalise davantage les erreurs importantes.

R² (Coefficient de détermination) : mesure la part de variance expliquée par le modèle.

Les scores seront ajoutés après l’exécution et l’évaluation des modèles.

Modèle

MAE

RMSE

R²

Linear Regression

À compléter

À compléter

À compléter

Random Forest

À compléter

À compléter

À compléter

XGBoost

À compléter

À compléter

À compléter

CatBoost

À compléter

À compléter

À compléter

LightGBM

À compléter

À compléter

À compléter

📊 Application Streamlit

L’application a pour objectif de permettre à l’utilisateur de renseigner les caractéristiques d’un véhicule et d’obtenir une estimation de son prix.

Fonctionnalités prévues ou à confirmer selon le code disponible :

Sélection de la marque et du modèle.

Saisie de l’année de fabrication.

Indication du kilométrage.

Sélection des caractéristiques techniques disponibles.

Affichage du prix estimé en dirhams marocains.

Présentation des informations utiles à l’interprétation de la prédiction.

Aperçu

Ajouter ici des captures d’écran réelles de l’application Streamlit.

screenshots/
├── home.png
├── prediction.png
└── model_evaluation.png

📁 Structure du projet

moroccan-used-car-price-predictor/
│
├── app.py
├── car_price_prediction.ipynb
├── requirements.txt
├── README.md
│
├── data/
│   └── .gitkeep
│
├── models/
│   └── .gitkeep
│
└── screenshots/
    └── .gitkeep

Cette structure est indicative : elle doit être adaptée aux fichiers réellement présents dans le dépôt. Les modèles entraînés, les données collectées et les captures d’écran ne doivent être ajoutés que lorsqu’ils existent.

⚙️ Installation et exécution

1. Cloner le dépôt

git clone https://github.com/TON-USERNAME/moroccan-used-car-price-predictor.git
cd moroccan-used-car-price-predictor

Remplacer TON-USERNAME par le nom réel du compte GitHub et vérifier l’URL du dépôt.

2. Créer un environnement virtuel

Sous Windows PowerShell :

python -m venv .venv
.\.venv\Scripts\Activate.ps1

3. Installer les dépendances

pip install -r requirements.txt

4. Lancer l’application

streamlit run app.py

L’application s’ouvrira dans le navigateur si Streamlit démarre correctement.

🔍 Points méthodologiques importants

Pour obtenir des résultats fiables, le projet doit notamment prendre en compte :

La suppression ou le traitement des annonces dupliquées et des valeurs incohérentes.

La séparation des données d’entraînement et de test avant toute optimisation.

L’utilisation d’un pipeline de prétraitement afin d’éviter les fuites de données.

La validation croisée réalisée uniquement sur les données d’entraînement.

L’adaptation des transformations aux variables numériques et catégorielles.

L’analyse des erreurs selon les gammes de prix et les catégories de véhicules.

La prise en compte du biais potentiel des annonces disponibles par rapport au marché réel.

Le scraping doit également respecter les conditions d’utilisation du site, les règles applicables et les mesures techniques de protection.

🚀 Améliorations futures

Ajouter une collecte de données automatisée et documentée.

Enrichir le jeu de données avec davantage de marques et de modèles.

Mettre en place une gestion reproductible des expériences ML.

Sauvegarder et versionner le meilleur modèle.

Ajouter des explications de prédiction avec SHAP.

Déployer l’application sur une plateforme accessible en ligne.

Mettre en place des tests automatisés et un pipeline CI/CD.

Surveiller la qualité des données et la dérive des prédictions.

📚 Compétences mises en pratique

Ce projet permet de travailler sur plusieurs compétences recherchées en IA et Data Science :

Python et manipulation de données.

Web scraping et préparation des données.

Analyse exploratoire et visualisation.

Feature Engineering.

Modélisation et évaluation en Machine Learning.

Optimisation d’hyperparamètres.

Développement d’une application avec Streamlit.

Structuration, documentation et versionnement d’un projet.Documentation du projet
```
