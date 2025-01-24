# README - Importation et Analyse de Données Automobiles

Ce document est un notebook Jupyter qui démontre l'importation, la manipulation et l'analyse d'un ensemble de données sur les automobiles. Le dataset est téléchargé depuis une URL, nettoyé, et analysé à l'aide de la bibliothèque Pandas en Python.

## Étapes Principales

1. **Importation des Bibliothèques** :
   - Les bibliothèques `pandas` et `numpy` sont importées pour la manipulation des données.

2. **Téléchargement des Données** :
   - Le fichier CSV contenant les données automobiles est téléchargé depuis une URL à l'aide de la fonction `pyfetch` de Pyodide.

3. **Chargement des Données** :
   - Les données sont chargées dans un DataFrame Pandas à l'aide de `pd.read_csv()`.

4. **Inspection des Données** :
   - Les premières et dernières lignes du DataFrame sont affichées avec `df.head()` et `df.tail()`.
   - Les types de données des colonnes sont vérifiés avec `df.dtypes`.

5. **Nettoyage des Données** :
   - Les valeurs manquantes représentées par `?` sont remplacées par `NaN`.
   - Les lignes avec des valeurs manquantes dans la colonne `price` sont supprimées.

6. **Ajout des En-têtes** :
   - Les en-têtes de colonnes sont ajoutés au DataFrame pour une meilleure lisibilité.

7. **Analyse Statistique** :
   - Un résumé statistique des colonnes numériques est généré avec `df.describe()`.
   - Un résumé statistique incluant les colonnes catégorielles est également généré avec `df.describe(include="all")`.

8. **Exportation des Données** :
   - Le DataFrame nettoyé est exporté en fichier CSV avec `df.to_csv()`.

9. **Informations Supplémentaires** :
   - Des informations détaillées sur le DataFrame, y compris les types de données et les valeurs manquantes, sont affichées avec `df.info()`.

## Utilisation

- **Python (Pyodide)** : Ce notebook est conçu pour fonctionner dans un environnement Python utilisant Pyodide, ce qui permet d'exécuter du code Python directement dans le navigateur.

## Fichiers

- **auto.csv** : Le fichier CSV original téléchargé depuis l'URL.
- **automobile.csv** : Le fichier CSV nettoyé et exporté après traitement.

## Conclusion

Ce notebook fournit un exemple complet de la manière dont on peut importer, nettoyer et analyser des données automobiles en utilisant Pandas. Il est idéal pour ceux qui débutent avec la manipulation de données en Python et souhaitent comprendre les étapes de base du traitement des données.