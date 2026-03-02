# Analyse des Données Économiques avec FRED et Python/Pandas

## Description du Projet

Ce projet présente une exploration approfondie des données économiques américaines en utilisant l'API du *Federal Reserve Economic Data (FRED)* et la bibliothèque `pandas` de Python. Il démontre des techniques d'extraction, de nettoyage, d'analyse et de visualisation de séries temporelles économiques clés, telles que le PIB, l'IPC, le S&P 500 et les taux de chômage par État. L'objectif est de fournir un cadre pour l'analyse macroéconomique et la détection de tendances, avec un accent particulier sur la corrélation entre les indicateurs et la visualisation géographique des données.

## Fonctionnalités Clés

*   **Extraction de Données FRED**: Récupération programmatique de diverses séries économiques via l'API FRED.
*   **Analyse de Séries Temporelles**: Visualisation des tendances historiques d'indicateurs macroéconomiques comme le PIB et l'IPC.
*   **Analyse de Corrélation**: Calcul et visualisation de la corrélation entre des indicateurs clés (ex: S&P 500 et taux de chômage national).
*   **Visualisation Géographique Interactive**: Création de cartes choroplèthes interactives pour représenter les données par État (ex: taux de chômage).
*   **Gestion de Données avec Pandas**: Nettoyage, fusion et manipulation de DataFrames pour l'analyse.

## Sources de Données

Les données sont principalement extraites de l'API [Federal Reserve Economic Data (FRED)](https://fred.stlouisfed.org/).

## Technologies Utilisées

*   Python 3.x
*   `pandas` pour la manipulation et l'analyse des données
*   `matplotlib` et `plotly.express` pour la visualisation des données
*   `fredapi` pour l'accès à l'API FRED

## Installation

Pour configurer l'environnement de développement, suivez les étapes ci-dessous :

1.  **Cloner le dépôt**:
    ```bash
    git clone [URL_DU_DEPOT_GITHUB]
    cd [NOM_DU_DEPOT]
    ```

2.  **Créer un environnement virtuel (recommandé)**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Sur Windows, utilisez `venv\Scripts\activate`
    ```

3.  **Installer les dépendances**:
    ```bash
    pip install pandas matplotlib plotly fredapi
    ```

4.  **Obtenir une Clé API FRED**: Vous aurez besoin d'une clé API FRED. Vous pouvez l'obtenir gratuitement sur le [site web de FRED](https://fred.stlouisfed.org/docs/api/api_key.html).

5.  **Configurer votre Clé API**: Remplacez `fred_key = 'VOTRE_CLE_API_FRED'` dans le notebook par votre clé réelle.

## Utilisation

Le projet est structuré sous forme de notebook Jupyter (`.ipynb`). Pour exécuter les analyses :

1.  **Lancer Jupyter Notebook ou JupyterLab**:
    ```bash
    jupyter notebook
    # ou
    jupyter lab
    ```

2.  **Ouvrir et Exécuter le Notebook**: Naviguez vers le fichier du notebook et exécutez les cellules séquentiellement pour reproduire l'analyse.

## Principales Conclusions

*   **PIB et IPC**: Les visualisations montrent les tendances historiques du PIB et de l'IPC, illustrant des périodes de croissance économique et d'inflation.
*   **S&P 500 vs. Taux de Chômage National**: Une corrélation négative modérée (environ -0.20) a été observée, suggérant qu'une baisse du chômage est souvent associée à une légère hausse du S&P 500, reflétant l'interdépendance entre un marché du travail sain et la performance boursière.
*   **Taux de Chômage par État**: La carte choroplèthe interactive a révélé des disparités significatives dans les taux de chômage entre les États, soulignant l'importance d'une analyse régionale.

## Perspectives d'Amélioration et Travaux Futurs

*   **Modélisation Prédictive**: Appliquer des modèles de séries temporelles pour prévoir les futurs mouvements des indicateurs économiques.
*   **Analyse de Causalité**: Explorer des méthodes pour établir des relations de causalité plutôt que de simple corrélation.
*   **Intégration de Plus de Données**: Ajouter d'autres sources de données (ex: données du marché de l'emploi, données sectorielles) pour une analyse plus riche.
*   **Tableaux de Bord Interactifs**: Développer des tableaux de bord interactifs plus complexes avec `Dash` ou `Streamlit`.

## Licence

Ce projet est distribué sous la licence MIT. Voir le fichier `LICENSE` pour plus de détails.
