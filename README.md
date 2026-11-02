# Projet 6 : Audit et fiabilisation des données d'un caviste (Python)

### Contexte
**BottleNeck**, caviste en ligne, gère 825 références (dont 714 actives) avec des données en silos : le stock dans l'ERP, les ventes sur le site web, et la correspondance entre les deux dans un fichier séparé.

**Mon objectif :** réconcilier les trois sources, identifier les erreurs qui faussent le chiffre d'affaires et la marge, puis produire une analyse de performance exploitable par la direction.

### Missions réalisées
* **Rapprochement des données :** fusion ERP, web et fichier de liaison (jointures sur le SKU).
* **Nettoyage :** 9 catégories d'anomalies traitées (prix de vente négatifs, stocks incohérents, identifiants orphelins, doublons...).
* **Trois anomalies critiques isolées :** ventes à perte (prix d'achat supérieur au prix de vente), produits actifs dans l'ERP mais invisibles sur le site, stock dormant.
* **Analyse du chiffre d'affaires :** loi de Pareto, marges, cohérence des prix (boxplot, écart interquartile, Z-score).

### Résultats
* **435 références (61 % du catalogue)** génèrent 80 % du chiffre d'affaires : une « zone cœur » à sécuriser, face à une longue traîne d'environ 280 produits.
* Une marge minimale de **-297 %**, due à une erreur de saisie.
* Trois recommandations : un verrou dans l'ERP contre les prix d'achat supérieurs au prix de vente, la séparation des ventes et des remboursements, un pilotage actif des stocks.

### Compétences & Outils
* **Langage :** Python
* **Librairies :** Pandas, Matplotlib, Seaborn
* **Techniques :** jointures, nettoyage de données, détection d'outliers (IQR, Z-score), analyse de Pareto

### Contenu du dépôt
* `notebooks/` : le notebook d'analyse
* `data-raw/` : exports ERP, web et fichier de liaison
* `reports/` : la présentation
* `images/` : captures d'écran

> **Note :** ce notebook contient deux erreurs d'exécution (une colonne supprimée deux fois, une marge calculée sur le mauvais tableau). Je les ai trouvées et corrigées plus tard, dans le [projet 13](https://github.com/RemyDaura/DA-Projet13-Projet-Data-Augmente-IA), qui reprend ce projet pour en automatiser le contrôle qualité.

<img src="images/Capture d'écran 2025-12-12 133710.png" width="500px"><img src="images/Capture d'écran 2025-12-23 130109.png" width="500px">
<img src="images/Capture d'écran 2025-12-30 130428.png" width="500px">
<img src="images/Capture d'écran 2025-12-30 132603.png" width="500px"><img src="images/Capture d'écran 2025-12-30 132508.png" width="500px">

---
📂 Dossier complet sur mon portfolio : [remydaura.github.io/p6.html](https://remydaura.github.io/p6.html)

*Ce projet fait partie de la formation Data Analyst d'OpenClassrooms.*
