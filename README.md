# 🌍 Analyse Stratégique du Marché Airbnb Europe

> **Projet Data Analysis - Janvier 2026**
> Exploration de données et recommandations d'investissement sur le marché locatif européen.

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Validé-success?style=for-the-badge)

---

## 📌 Contexte & Objectif
Dans le cadre de mon cursus Data Analyst, j'ai réalisé une étude approfondie sur le marché Airbnb.
**L'objectif :** Analyser un jeu de données complexe (~50 000 lignes) couvrant **10 grandes villes européennes** (Paris, Londres, Amsterdam, Berlin, etc.) pour identifier les facteurs influençant le prix et la satisfaction client.

---

## 🛠️ Méthodologie Technique
Mon approche s'est déroulée en 3 étapes :

1.  **Data Engineering :** * Agrégation automatisée de 20 fichiers CSV (Week-end vs Semaine).
    * Nettoyage des données (suppression des colonnes inutiles `Unnamed:0`).
    * Création de la variable `day_type` pour analyser l'impact du week-end.
2.  **Analyse Exploratoire (EDA) :**
    * Comparaison des prix moyens par ville.
    * Étude de la corrélation Prix / Distance du centre.
3.  **Visualisation :** Production de graphiques en "Flat Design" pour le rapport.

---

## 🔎 Résultats Visuels & Insights

### 1. Cartographie des Prix : La domination d'Amsterdam
Contrairement aux idées reçues, ce n'est pas Paris ou Londres qui affichent la moyenne la plus haute, mais **Amsterdam**, avec des prix dépassant souvent 500€ pour 2 nuits.

![Carte Europe](images/map_europe.png)

### 2. Classement des Villes (Moyenne 2 nuits)
On observe une fracture Nord/Sud : les villes méditerranéennes (Athènes, Rome, Lisbonne) restent beaucoup plus abordables que les capitales du Nord.

![Graphique Barres](images/barplot_price.png)

### 3. Matrice de Corrélation
L'analyse montre que :
* Le **Prix** est négativement corrélé à la **Distance** (Plus on s'éloigne, moins c'est cher), surtout à Amsterdam (-0.26).
* La **Satisfaction Client** est très fortement liée à la **Propreté**, mais très peu au prix. Payer cher ne garantit pas d'être satisfait !

![Heatmap](images/heatmap.png)

---

## 📂 Structure du Projet

```text
├── data/               # Les 20 fichiers CSV bruts (Amsterdam, Paris, etc.)
├── images/             # Les graphiques générés pour ce rapport
├── notebooks/          # Le code complet (Google Colab .ipynb)
└── README.md           # Ce fichier de présentation
