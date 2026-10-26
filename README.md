# 🚗 Moroccan Used Car Price Predictor (Avito.ma Scraping & ML)

> **Projet de Machine Learning de bout en bout**  
> *Collecte de données (Web Scraping Avito.ma), Feature Engineering, Benchmarking de Modèles & Déploiement Streamlit*

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red.svg)](https://streamlit.io/)
[![LightGBM](https://img.shields.io/badge/Model-LightGBM%20%7C%20XGBoost-orange.svg)](https://lightgbm.readthedocs.io/)
[![Scraping](https://img.shields.io/badge/Scraping-BeautifulSoup-green.svg)](https://www.crummy.com/software/BeautifulSoup/)

---

## 📌 Présentation

Ce projet implémente un pipeline Machine Learning complet pour estimer la valeur marchande d'un véhicule d'occasion au Maroc :
1. **Extraction de données réelles** via web scraping sur [Avito.ma](https://www.avito.ma) (BeautifulSoup).
2. **Nettoyage & Normalisation** : extraction de données numériques depuis des chaînes complexes (kilométrage, devises, puissance fiscale "CV", boîte de vitesses, première main).
3. **Analyse Exploratoire (EDA)** : matrices de corrélation, distributions des prix et détection d'outliers.
4. **Benchmark de Modèles Régresseurs** : Linear Regression, Random Forest, XGBoost, CatBoost et LightGBM.
5. **Optimisation d'hyperparamètres** : K-Fold Cross-Validation et GridSearchCV.
6. **Interface Interactive** : Application web Streamlit prête au déploiement.

---

## 🚀 Lancer l'Application Streamlit

```bash
# 1. Cloner le repository
git clone https://github.com/votre-username/car-price-prediction.git
cd car-price-prediction

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Lancer l'application
streamlit run app.py
```

---

## 📊 Structure du Projet

```
car-price-prediction/
├── app.py                      # Interface web interactive Streamlit
├── car_price_prediction.ipynb   # Notebook de scraping, nettoyage et modélisation
├── requirements.txt            # Dépendances Python
└── README.md                   # Documentation du projet
```
