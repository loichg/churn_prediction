
# Étude de l’attrition client en banque

## Description

Ce projet vise à analyser et prédire l’attrition (churn) des clients bancaires.
L’objectif est de mieux comprendre les comportements clients et d’identifier les facteurs qui influencent leur départ.

## Objectifs

* Identifier des profils de clients homogènes
* Comprendre les facteurs liés au churn
* Prédire le départ des clients
* Comparer plusieurs modèles de machine learning

## Dataset

Dataset utilisé :
https://www.kaggle.com/datasets/anwarsan/credit-card-bank-churn

Données contenant :

* Informations clients (âge, genre, revenu, etc.)
* Données bancaires (limite de crédit, solde)
* Comportement (transactions, activité, interactions)

## Analyse exploratoire

* Aucune valeur manquante
* Suppression des variables inutiles
* Étude des distributions et corrélations

### Observations :

* Les clients churnés effectuent moins de transactions
* Ils dépensent moins
* Leur utilisation du crédit est plus faible

---

## Méthodes utilisées

### Analyse factorielle

* ACP (Analyse en Composantes Principales)
* AFC (Analyse Factorielle des Correspondances)

### Classification non supervisée

* Clustering (k = 5)
* Segmentation des clients

### Classification supervisée

* Régression logistique
* Régression Lasso
* Arbre de décision (CART)
* Random Forest
* AdaBoost

## Gestion du déséquilibre

* 84% clients fidèles / 16% churn
* Utilisation de **SMOTE** pour équilibrer les données

## Résultats

| Modèle        | Accuracy  | AUC       |
| ------------- | --------- | --------- |
| Random Forest | **95.8%** | **0.985** |
| AdaBoost      | 93.8%     | 0.974     |
| Lasso         | 86.7%     | 0.927     |

Meilleur modèle : **Random Forest**

## Outils utilisés

Langage : R
