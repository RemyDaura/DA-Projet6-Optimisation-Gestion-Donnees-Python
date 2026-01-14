# Projet 6 : Optimisation de la gestion des données (ERP vs Web)

###  Contexte
Je suis intervenu pour **BottleNeck**, un marchand de vin prestigieux. L'entreprise avait un problème critique : ses données étaient cloisonnées. D'un côté un export de l'ERP (gestion des stocks), de l'autre un export du site E-commerce (CMS), et aucun lien fiable entre les deux.

**Mon objectif :** Réconcilier ces deux sources de données pour calculer le Chiffre d'Affaires réel par produit et identifier les erreurs de prix potentielles.

###  Missions réalisées
* **Rapprochement de données (Data Merging) :** Fusion des exports ERP et Web via une clé unique (SKU), en gérant les problèmes de correspondances (Left Join, Inner Join).
* **Nettoyage (Data Cleaning) :** Standardisation des formats, gestion des doublons et des valeurs nulles.
* **Calcul du CA :** Création d'indicateurs pour déterminer le chiffre d'affaires total et par bouteille.
* **Détection d'anomalies (Outliers) :** Analyse statistique des prix pour repérer les valeurs aberrantes (prix trop élevés ou trop bas) en utilisant :
    * La méthode des écarts interquartiles (IQR).
    * La visualisation graphique (Boxplot / Moustache).

###  Compétences & Outils
* **Langage :** Python
* **Librairies :** Pandas (manipulation de DataFrames), Matplotlib & Seaborn (Visualisation).
* **Technique :** Jointures relationnelles, Statistiques descriptives, Z-score.

---


<img src="images/Capture d'écran 2025-12-12 133710.png" width="500px"><img src="images/Capture d'écran 2025-12-23 130109.png" width="500px">
<img src="images/Capture d'écran 2025-12-30 130428.png" width="500px">

<img src="images/Capture d'écran 2025-12-30 132603.png" width="500px"><img src="images/Capture d'écran 2025-12-30 132508.png" width="500px">

---
*Ce projet fait partie de la formation Data Analyst d'OpenClassrooms.*
