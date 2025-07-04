# projet-analyse-de-donnée
Diagnostic du Cancer du Sein par Analyse Morphologique des Noyaux Cellulaires
🎯 Objectif du projet
Ce projet a pour but d’automatiser le diagnostic du cancer du sein à partir de caractéristiques morphologiques des noyaux cellulaires extraites d’images issues de biopsies à l’aiguille fine (BAF).
Nous utilisons plusieurs modèles de Machine Learning pour classifier les tumeurs comme bénignes (0) ou malignes (1) en se basant sur le jeu de données Breast Cancer Wisconsin (Diagnostic).

🗂 Données
 Source : UCI Machine Learning Repository – Dataset #17

 Données : 569 observations – 30 caractéristiques numériques par observation + 1 variable cible (diagnosis)

⚙️ Étapes du projet
Chargement & Nettoyage des données

Suppression de colonnes inutiles (id)

Encodage de la variable diagnosis : B = 0, M = 1

Normalisation des variables numériques (StandardScaler)

Analyse exploratoire

Statistiques descriptives

Visualisations (boxplots, histogrammes, heatmap de corrélation)

PCA et t-SNE pour visualisation 2D

Modélisation

Régression logistique

Arbre de décision

Random Forest

Naive Bayes

Réseau de neurones (Keras)

SVM

Gradient Boosting

Évaluation des modèles

Accuracy, Précision, Rappel, F1-score

Matrices de confusion

Courbes ROC et score AUC

Comparaison et sélection finale

Choix du meilleur modèle selon les performances (Random Forest ou Réseau de neurones)

🔍 Résultats
Modèles les plus performants :regression logistique, Random Forest et Réseau de Neurones (Accuracy ≈ 98%)

Les caractéristiques comme concavity_worst, radius_mean, area_worst sont fortement discriminantes.

Le projet démontre qu’une classification fiable est possible dès la phase de dépistage à partir de données simples.

🧪 Utilisation
bash
Copier
Modifier
# 1. Cloner le repo
git clone <repo_url>
cd cancer-du-sein

# 2. Installer les dépendances
pip install -r requirements.txt

# 3. Lancer le notebook
jupyter notebook breast_cancer_diagnostic.ipynb
📌 Technologies
Python 3

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Keras / TensorFlow

