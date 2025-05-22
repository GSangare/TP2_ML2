# Clustering KMeans sur les chiffres manuscrits avec PCA et scalers

Ce projet réalise un clustering non supervisé sur le jeu de données `digits` (chiffres manuscrits 8x8 pixels) en utilisant l’algorithme KMeans. 

## Objectif

- Regrouper les images des chiffres en clusters similaires.
- Tester l’impact de différentes configurations : nombre de clusters, méthodes d’initialisation, mise à l’échelle (scalers), utilisation ou non de la réduction dimensionnelle (PCA).
- Évaluer la qualité des clusters avec plusieurs métriques (inertie, homogénéité, complétude, V-measure, ARI, silhouette).
- Visualiser les images moyennes de chaque cluster dans l’espace original (images 8x8).

## Contenu principal

- Chargement des données `digits` de `sklearn.datasets`.
- Fonction `eval_kmeans` pour entraîner KMeans avec différents hyperparamètres et calculer les métriques.
- Recherche des meilleures configurations en combinant scaler, PCA, nombre de clusters, etc.
- Affichage graphique des scores silhouette des meilleures configurations.
- Calcul et affichage des images moyennes par cluster selon la meilleure configuration.

## Installation

Le code nécessite Python 3 avec les librairies suivantes :

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

Installer avec pip si besoin :

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
