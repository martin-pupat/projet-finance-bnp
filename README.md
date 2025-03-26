# CentraleSupélec - Projet BNP

Auteurs :
- Tom Delande
- Yanis Kaafarani
- Martin Pupat
- Sami Rayan Chemlal

## Sommaire

Dans ce répertoire se trouvent les fichiers suivants :
- `Apreprocess_bnp` est le fichier de preprocessing. Il fusionne les deux bases de données, lave les données intéressantes et supprime les données inutiles. Il renvoie une base de données `dataframe` qui sera utilisée dans les modèles suivants.
- `aggregation_month_arima` implémente le modèle de prédiction `ARIMA` sur la base de données. Une optimisation des hyperparamètres est faite, ainsi qu'une métrique des erreurs.
- `aggregation_month_lstm` implémente le modèle de prédiction `LSTM` sur la base de données.
- `aggregation_month_prophet` implémente le modèle de prédiction `PROPHET` sur la base de données. Une optimisation des hyperparamètres est faite, ainsi qu'une métrique des erreurs.
- `markowitz` implémente le modèle de Markowitz afin de générer le portefeuille d'allocations optimal en fonction des résultats de nos modèles de prédiction.
- `Bpreprocess_bnp` puis `Bpreprocess_bnp(suite)` sont deux autres fichiers de preprocessing. Ils ne servent qu'à générer une matrice de corrélation à partir des données initiales et n'ont pas pu être rassemblés avec les premiers fichiers de preprocessing.