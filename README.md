# 🏆 Kaggle Competition – Diabetes Prediction (AUC ROC)

## 📌 Project Overview (English)

This project was developed for a Kaggle-style machine learning competition focused on predicting whether a patient has been diagnosed with diabetes.

The evaluation metric used in this competition is **Area Under the ROC Curve (AUC ROC)**, which measures the model’s ability to rank positive cases higher than negative ones.

The final solution relies on an **optimized CatBoost model**, chosen for its strong performance on tabular data and its native handling of categorical features.

---

## 🚀 Model & Methodology

* Algorithm: **CatBoostClassifier**
* Objective: Binary classification (`diagnosed_diabetes`)
* Evaluation metric: **AUC ROC**
* Validation strategy: **Stratified K-Fold Cross-Validation (5 folds)**
* Key techniques:

  * Ordered Boosting to prevent target leakage
  * Bayesian Bootstrap for regularization
  * Early stopping to avoid overfitting
  * Test-time averaging across folds

This configuration provides an excellent trade-off between **performance** and **training time**, while remaining competition-safe.

---

## 📈 Results

* **Public leaderboard rank:** 🏅 **258/2276**
* The model achieves a strong AUC score while remaining computationally efficient.

---

## 📂 Files

* `train.csv` – Training dataset
* `test.csv` – Test dataset
* `sample_submission.csv` – Submission format example
* `notebook2.py` – Training and inference script
* `submission6.csv` – Final submission file

---

# 🇫🇷 Compétition Kaggle – Prédiction du Diabète (AUC ROC)

## 📌 Présentation du projet

Ce projet a été réalisé dans le cadre d’une compétition Kaggle visant à prédire si un patient a été diagnostiqué diabétique.

La métrique d’évaluation utilisée est l’**AUC ROC (Area Under the Receiver Operating Characteristic Curve)**, qui mesure la capacité du modèle à bien classer les individus positifs par rapport aux négatifs.

La solution finale repose sur un **modèle CatBoost optimisé**, particulièrement adapté aux données tabulaires contenant des variables catégorielles.

---

## 🚀 Modèle et méthodologie

* Algorithme : **CatBoostClassifier**
* Problème : Classification binaire (`diagnosed_diabetes`)
* Métrique : **AUC ROC**
* Validation : **Validation croisée stratifiée (5 folds)**
* Techniques utilisées :

  * Ordered Boosting pour éviter la fuite d’information
  * Bootstrap bayésien pour la régularisation
  * Early stopping pour limiter l’overfitting
  * Moyennage des prédictions sur les folds

Cette approche permet d’obtenir un excellent compromis entre **performance**, **robustesse** et **temps de calcul**.

---

## 📈 Résultats

* **Classement sur le leaderboard public :** 🏅 **258ᵉ place/2276**
* Modèle performant et stable sur les données de test

---

## 📂 Fichiers du projet

* `train.csv` – Données d’entraînement
* `test.csv` – Données de test
* `sample_submission.csv` – Exemple de fichier de soumission
* `notebook2.py` – Script d’entraînement et de prédiction
* `submission6.csv` – Fichier de soumission finale

---
