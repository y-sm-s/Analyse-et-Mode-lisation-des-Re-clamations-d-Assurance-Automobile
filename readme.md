[# Projet 2 : Modélisation des Résultats des Réclamations d'Assurance Automobile](Analyse et Modélisation des Réclamations d'Assurance Automobile.ipynb)

## Description  
Ce projet utilise l'apprentissage automatique pour prédire si un client de l'assurance automobile fera une réclamation pendant la période de validité de sa police. Travaillant pour On the Road car insurance, l'objectif est d'identifier la caractéristique du jeu de données qui produit le modèle de régression logistique le plus précis pour prédire si une réclamation sera faite contre une police.

## Contexte  
Les compagnies d'assurance investissent beaucoup de temps et d'argent pour optimiser leurs prix et estimer avec précision la probabilité que les clients fassent une réclamation. Dans de nombreux pays, il est légalement obligatoire d'avoir une assurance automobile pour conduire un véhicule sur les routes publiques, ce qui rend le marché très vaste. Conscient de cela, On the Road car insurance a demandé vos services pour construire un modèle afin de prédire si un client fera une réclamation sur son assurance pendant la période de validité de la police. Comme ils ont très peu d'expertise et d'infrastructure pour déployer et surveiller des modèles d'apprentissage automatique, ils ont demandé à identifier la seule caractéristique qui donne le meilleur modèle, mesuré par la précision, afin de pouvoir commencer avec un modèle simple en production.

## Données  
Les données des clients sont fournies sous forme de fichier CSV nommé `car_insurance.csv`, accompagné d'une table détaillant les noms des colonnes et leurs descriptions.

## Méthodologie  
Voici les étapes que nous avons suivies pour réaliser cette analyse :

1. **Lecture et exploration du jeu de données**  
   Chargement des données à partir du fichier CSV `car_insurance.csv` et exploration initiale pour comprendre la structure des données.

2. **Prétraitement des Données**  
   - Conversion des colonnes de type objet en valeurs numériques pour faciliter l'analyse.
   - Traitement des valeurs manquantes en utilisant la médiane pour remplir les colonnes concernées.

3. **Modélisation**  
   Construction de plusieurs modèles de régression logistique en utilisant différentes caractéristiques du jeu de données.

4. **Évaluation de la Performance**  
   Évaluation de la performance des modèles pour déterminer lequel a la meilleure précision.

5. **Identification de la Meilleure Caractéristique**  
   Sélection de la caractéristique qui donne le meilleur modèle basé sur la précision mesurée.

## Résultats  
Le modèle a permis d'identifier la meilleure caractéristique pour prédire les réclamations d'assurance automobile. Les résultats sont stockés dans un DataFrame nommé `best_feature_df`, qui contient :
- `best_feature` : la caractéristique avec la précision la plus élevée.
- `best_accuracy` : le score de précision respectif.
