# Projet Big Data et MLOPS

Ce projet permet de récupérer des données depuis l'API GitHub, de les traiter via Kafka, et de proposer une solution de valorisation de ces données grâce à l'IA.

## Prérequis

Il faut ouvrir le fichier projet_ufacik.ipynb
Les dépendances nécessaires sont listées dans le fichier `requirements.txt`.
Génere une clé github et la mettre dans un fichier .env
Exemple : GITHUB_TOKEN=clé

Vous pouvez créer une clé ici : https://github.com/settings/tokens

## Installation et démarrage

### 1. Démarrer Kafka

Ouvrez un premier terminal, déplacez-vous dans le dossier contenant Kafka et exécutez :

```bash
bin/zookeeper-server-start.sh config/zookeeper.properties
```

Dans un second terminal, déplacez-vous dans le même dossier et exécutez :

```bash
bin/kafka-server-start.sh config/server.properties
```

> **Note** : Si le serveur se termine de façon inattendue dans le deuxième terminal, relancez la commande avant d'exécuter les étapes suivantes.

### 2. Exécution du projet

Lancez Jupyter Lab et exécutez les cellules dans l'ordre suivant :

1. "Kafka récupération de données"
2. "Kafka Producer" (permet de récupérer les données depuis l'API GitHub)
3. "Kafka Consumer"
4. Allez à la section "Step 2 : Proposer une solution valorisant les données recueillies, grâce à l'IA, à destination d'entreprises, d'associations ou tout autre type d'organisation ainsi que des particuliers."
5. Exécutez la cellule "Prediction avec interface"

## Fonctionnalités additionnelles

Vous pouvez également exécuter la cellule concernant le "Step 3 : monitoring" pour voir les essais effectués, bien que cette partie ne soit pas encore fonctionnelle.
