# Prédiction des Besoins en Consommation Énergétique des Bâtiments Non Résidentiels

## Contexte du Projet

La ville de Seattle poursuit un objectif ambitieux de devenir neutre en émissions de carbone d'ici 2050. Pour atteindre cet objectif, l'équipe de gestion des bâtiments se concentre sur la réduction des émissions et de la consommation énergétique des bâtiments non résidentiels.

Des relevés détaillés de consommation d'énergie et des émissions de CO2 ont été effectués en 2016, mais ces relevés sont coûteux à obtenir. Le but du projet est de prédire les émissions de CO2 et la consommation totale d'énergie de bâtiments non résidentiels pour lesquels ces données ne sont pas disponibles, en utilisant des informations structurelles telles que la taille du bâtiment, son usage, la date de construction, et sa localisation.

Une autre partie importante du projet est d'évaluer l'utilité de l'ENERGY STAR Score, qui est actuellement difficile à calculer, en l'intégrant dans le modèle de prédiction et en jugeant de sa pertinence.
Objectifs du Projet

Les objectifs principaux de l'analyse et de la modélisation sont les suivants :
- Analyse exploratoire des données : Réaliser une analyse préliminaire pour comprendre les données disponibles, identifier les variables pertinentes, et évaluer la distribution des variables.
- Prédiction des émissions de CO2 et de la consommation énergétique : Construire et tester plusieurs modèles de prédiction pour estimer les émissions de CO2 et la consommation énergétique des bâtiments non résidentiels.
- Évaluation de l'ENERGY STAR Score : Intégrer l'ENERGY STAR Score dans le modèle pour évaluer s’il améliore la précision de la prédiction des émissions et de la consommation.
- Optimisation des performances : Appliquer des techniques de prétraitement des données (normalisation, transformations log) et d'évaluation des performances (validation croisée, optimisation des hyperparamètres) pour améliorer les prédictions.

## Données

Les données utilisées proviennent de relevés effectués en 2016 sur la consommation énergétique et les émissions de CO2 des bâtiments non résidentiels à Seattle. Les informations disponibles incluent des données structurelles sur les bâtiments, telles que :
- Caractéristiques du bâtiment : Taille, usage, année de construction, et situation géographique.
- Consommation d’énergie : Consommation annuelle d’énergie par bâtiment.
- Émissions de CO2 : Quantité de CO2 émise par bâtiment.

Les données des bâtiments pour lesquels les mesures ne sont pas disponibles seront utilisées pour entraîner les modèles de prédiction.

## Méthodologie

Le projet se déroule en plusieurs étapes clés :

Analyse exploratoire des données (EDA) :
- Exploration des variables structurelles des bâtiments pour en comprendre la distribution.
- Recherche de relations entre les variables structurelles et les émissions de CO2 / consommation d’énergie.
- Traitement des valeurs manquantes et des données aberrantes, et application de transformations simples comme la normalisation ou le passage au log des variables pertinentes.

Prédiction des émissions et de la consommation énergétique :
- Test de plusieurs modèles de machine learning pour prédire les émissions de CO2 et la consommation énergétique, en utilisant des algorithmes de différentes familles (ElasticNet, SVM, GradientBoosting, RandomForest, etc.).
- Utilisation d’une validation croisée pour évaluer les performances des modèles et éviter la fuite de données.

Intégration et évaluation de l'ENERGY STAR Score :
- Intégration de l'ENERGY STAR Score dans les modèles et analyse de son impact sur la précision des prédictions.
- Comparaison des performances des modèles avec et sans l'ENERGY STAR Score.

Optimisation des performances :
- Ajustement des hyperparamètres des différents modèles pour maximiser leur précision.
- Évaluation rigoureuse des performances avec des métriques appropriées (RMSE, MAE, etc.).

## Outils et Technologies

L’analyse a été réalisée avec les outils et bibliothèques suivants :
- Pandas pour la manipulation des données.
- Scikit-learn pour la construction et l’évaluation des modèles de machine learning.
- Matplotlib et Seaborn pour la visualisation des données.
- NumPy pour les opérations numériques.
- XGBoost et LightGBM pour les modèles de boosting.

## Résultats et Application

Les résultats de ce projet permettront de prédire la consommation énergétique et les émissions de CO2 des bâtiments non résidentiels de Seattle, en utilisant uniquement les informations structurelles des bâtiments. L'évaluation de l'ENERGY STAR Score permettra également de déterminer si son intégration améliore la qualité des prédictions.

L’application de ces prédictions aidera la ville à mieux cibler ses efforts pour réduire la consommation énergétique et les émissions des bâtiments non résidentiels dans le cadre de son objectif de neutralité carbone pour 2050.
