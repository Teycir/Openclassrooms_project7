# Parcours Data Science  Projet n°7: "Implémentez un modèle de scoring"

## Description du projet

L'ENTREPRISE "PRÊT À DÉPENSER"
propose des crédits à la consommation pour des personnes ayant peu ou pas du tout d'historique de prêt.
L’entreprise souhaite développer un modèle de Scoring de la probabilité de défaut de paiement du client
pour étayer la décision d'accorder ou non un prêt
Pour réaliser cette étude on s'appuie sur des sources de données variées (données comportementales,
données provenant d'autres institutions financières, etc.).
On doit fournir un outil de compréhension et d'explication du résultat car les clients sont de plus en plus
demandeurs de transparence vis-à-vis des décisions d’octroi de crédit .
Pour cela nous allons mettre en place un dashboard interactif pour que les chargés de relation client
puissent à la fois expliquer de façon la plus transparente possible les décisions d’octroi de crédit, mais
également permettre à leurs clients de disposer de leurs informations personnelles et de les explorer
facilement. Les data scientists pourront avec ce dashbord calibrer les modèles et les entrainer ainsi qu'explorer les données. 


## Données

 https://www.kaggle.com/c/home-credit-default-risk/data
 
 
## Notebooks

* 1 projet7_kaggle_Feature_Engineering_1 ==> première étape de nettoyage de données: fusion et agrégation des données brutes
* 2 projet7_kaggle_Feature_Engineering_2 ==> deuxième étape de nettoyage de données: traitement des valeurs manquantes, de la colinéarité, conversion de données 
* 3 projet7_kaggle_Feature_Selection ==> réduction du nombre de features aux plus importantes
* 4 projet7_modelisation ==> sélection du meilleur modèle
* 5 projet7_interpretation ==> exploration du modèle sélectionné et application du surrogate model sur celui-ci

## Lien pour l'API
Ceci est notre lien du déploiement de notre API.

https://pretdepenser.herokuapp.com/

* 1 https://pretdepenser.herokuapp.com/api/sk_ids/  ==> Extraire la liste des identifiants des clients

* 2 https://pretdepenser.herokuapp.com/api/personal_data?SK_ID_CURR=384575  ==> Obtenir les données du client

* 3 https://pretdepenser.herokuapp.com/api/features_desc  ==> Description des features

* 4 https://pretdepenser.herokuapp.com/api/features_imp  ==> Classement de l'importance des features 

* 5 https://pretdepenser.herokuapp.com/api/local_interpretation?SK_ID_CURR=384575   ==> Prédiction de solvabilité du client


Github API: https://github.com/Teycir/API 

## Lien pour le Dashboard

Ceci est le lien de notre dashboard qui contient le résultat de scoring d'un client ainsi que l'intréprétabilité du résultat de scoring.
Il permet de visualiser l'ensemble des attributs d'un client et de tous les clients.

https://share.streamlit.io/teycir/dashboard/DashBoard/app.py

Github Dashboard: https://github.com/Teycir/DashBoard


