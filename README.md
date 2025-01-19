# projet-ML
# SARS-CoV-2 Classification Project

# Description

Ce projet vise à prédire les résultats des examens du SARS-CoV-2 (à savoir si un patient est positif ou négatif) à l'aide de variables biologiques et virales issues d'un dataset médical. Le pipeline inclut l'analyse exploratoire, le prétraitement des données, la sélection des caractéristiques, et l'entraînement de modèles de machine learning.

# Données

### Variables clés :

•	SARS-Cov-2 exam result : Variable cible (positive ou negative).

•	Patient age quantile : Catégorie d'âge du patient.

•	Groupes de variables :

•	Variables biologiques (ex. : Hemoglobin, Leukocytes).

•	Variables virales (ex. : Influenza A, Metapneumovirus).


# Pipeline

### 1. Analyse exploratoire des données (EDA)

•	Visualisation des distributions des variables biologiques et virales.

•	Analyse des taux de valeurs manquantes pour identifier les groupes de variables pertinents.

### 2. Prétraitement des données

#### • Encodage : Conversion des variables qualitatives en quantitatives.

#### • Feature Engineering : Identification des patients "malades" à partir des variables virales.

#### • Imputation des données : Suppression des lignes avec trop de valeurs manquantes.

### 3. Modélisation

#### Modèles utilisés :

• Random Forest

• AdaBoost

• SVM

• KNN

# Evaluation :

#### Courbes d'apprentissage.

#### Matrices de confusion.

#### Rapports de classification.

### 4. Optimisation des hyperparamètres

Recherche aléatoire (RandomizedSearchCV) pour affiner les performances des modèles.

Résultats principaux

Meilleur modèle : [indiquer le modèle].

Scores obtenus :

Rappel : 0.6875.

F1-Score : 0.5581395348837209.

Technologies

Langage : Python

Bibliothèques : pandas, numpy, matplotlib, seaborn, scikit-learn

Exécution

Cloner ce dépôt :

git clone [https://github.com/omar9316/projet-ML.git]

Installer les dépendances :

pip install -r requirements.txt

Exécuter les notebooks dans l'ordre :

Analyse exploratoire des données.ipynb

Prétraitement des données.ipynb

Modélisation.ipynb

Structure des fichiers

data/ : Contient le dataset brut.

notebooks/ : Contient les notebooks pour chaque étape du projet.

models/ : Contient les modèles enregistrés.

README.md : Description du projet.
