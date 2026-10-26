# 🚗 Moroccan Used Car Price Predictor (Avito.ma Scraping & Machine Learning)

> **End-to-End Machine Learning Project**  
> *Data Collection, Data Preprocessing, Feature Engineering, Model Evaluation & Streamlit Deployment*

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red.svg)](https://streamlit.io/)
[![LightGBM](https://img.shields.io/badge/Models-LightGBM%20%7C%20XGBoost-orange.svg)](https://lightgbm.readthedocs.io/)
[![Scraping](https://img.shields.io/badge/Data%20Collection-BeautifulSoup-green.svg)](https://www.crummy.com/software/BeautifulSoup/)

---

## 📌 Présentation

Ce projet vise à développer une solution de Machine Learning capable d’estimer les prix des voitures d’occasion sur le marché marocain à partir des informations disponibles dans les annonces publiées sur [Avito.ma](https://www.avito.ma).

Le pipeline comprend plusieurs étapes essentielles :

1. **Collecte des données** : récupération des informations relatives aux véhicules à l’aide de techniques de web scraping avec BeautifulSoup.
2. **Prétraitement des données** : nettoyage, transformation et standardisation des informations, notamment les prix, le kilométrage, la puissance fiscale, le type de transmission et le statut de première main.
3. **Analyse exploratoire (EDA)** : étude des distributions, analyse des corrélations et identification des valeurs atypiques.
4. **Comparaison des modèles** : évaluation de plusieurs algorithmes de régression, notamment Linear Regression, Random Forest, XGBoost, CatBoost et LightGBM.
5. **Optimisation des performances** : utilisation de la validation croisée K-Fold et de GridSearchCV pour rechercher les meilleurs hyperparamètres.
6. **Développement de l’application** : création d’une interface interactive avec Streamlit pour générer des estimations de prix à partir des caractéristiques d’un véhicule.

---

## 🚀 Lancer l'Application Streamlit

```bash
# 1. Cloner le repository
git clone https://github.com/votre-username/car-price-prediction.git
cd car-price-prediction

# 2. Installer les bibliothèques nécessaires
pip install -r requirements.txt

# 3. Démarrer l'application
streamlit run app.py
```

---

## 📊 Structure du Projet

```text
car-price-prediction/
├── app.py                      # Application interactive développée avec Streamlit
├── car_price_prediction.ipynb   # Notebook dédié à la collecte, l'analyse et la modélisation
├── requirements.txt            # Liste des dépendances du projet
└── README.md                   # Documentation du projet
```


Python et manipulation de données.

Web scraping et préparation des données.

Analyse exploratoire et visualisation.

Feature Engineering.

Modélisation et évaluation en Machine Learning.

Optimisation d’hyperparamètres.

Développement d’une application avec Streamlit.

Structuration, documentation et versionnement d’un projet.Documentation du projet
```
