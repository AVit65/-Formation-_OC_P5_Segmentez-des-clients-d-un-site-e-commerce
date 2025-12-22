📊 **Projet**

Le site de vente en ligne brésilien Olist souhaite segmenter ses clients en fonction de leur profil afin de mieux cibler ses campagnes de communication. Cette segmentation a pour objectif de mieux comprendre les comportements d’achat et les caractéristiques des clients, dans le but de proposer des actions marketing plus ciblées, personnalisées et efficaces.

Après une analyse exploratoire des données, les différentes sources d’information (commandes, paiements, livraisons, avis clients, etc.) ont été agrégées et transformées pour construire une table client enrichie, intégrant des indicateurs synthétiques et pertinents décrivant les comportements et les caractéristiques des clients. Puis, plusieurs algorithmes de segmentation ont été testés et comparés afin d’identifier des groupes de clients homogènes et interprétables, en s’appuyant sur des métriques d’évaluation adaptées. Enfin, une analyse de la stabilité temporelle des clusters a été réalisée afin d'établir un contrat de maintenance. 

🎓 **Compétences évaluées**
- Évaluer les performances des modèles d’apprentissage non supervisé
 - Sélectionner et entraîner des modèles d’apprentissage non-supervisé

📂 **Architecture du repository**

*Note*: les données ne sont pas inclues et doivent être téléchargés via le lien ci-dessous

```
OC_P5_Segmentez-des-cliens-d'un-site-e-commerce/
│
├── Data/                       
├── Notebook/                         # Notebook d’analyse                            
├── Ouput/                                    
│   ├── Cluster/                      # Visualisations et descriptions des clusters (Effectifs, profils moyens, etc.)
│   ├── Corrélations/                 # Heatmap illustrant les corrélations entre variables 
│   ├── Dendrogramme/                 # Dendogramme issus de l'algorithme Hierarchichal Clustering
│   ├── Distributions/                # Graphiques de distribution des variables
│   ├── Explicativité/                # Graphiques issus de l'analyses d’explicabilité des modèles 
│   ├── Maintenant   /                # Graphiques issus de l'analyses de la stabilité temporelle de la segmentation retenue
│   ├── Normalisation/                # Graphique illustrant l'impact des méthodes de normalisation 
│   ├── Performances/                 # Évaluations des algorithmes (distorsion, silhouette, Calinski, etc.) 
│   ├── Projection/                   # Projections des données en 2D (TNSE, UMAP)
│   ├── Stabilité_initiation/         # Analyses de stabilité des clusters selon l’initialisation
│   ├── Table/                        # Table de clients enrichie
├── Soutenance/                       # Présentation en pdf
├── README.md                         # Documentation générale du projet
├── Requirements                      # Liste des dépendances nécessaires

```

🗄️ **Données**

La base de données brute  utilisée dans le notebook d’analyse  peuvent être téléchargées via ce [lien](https://course.oc-static.com/projects/olist.db) et contient les tables suivantes:
- sellers
- orders
- customers 
- order_pymts
- order_items
- products
- order_reviews
- translation
- geoloc


