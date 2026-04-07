# 🌾 Microcrédit Agriculture - Dashboard Power BI

## 📌 Description
Ce projet consiste en la création d'un tableau de bord interactif sur Power BI pour analyser l'attribution et l'impact des microcrédits dans le secteur agricole. L'objectif est de transformer des données brutes de production et de financement en indicateurs visuels pour faciliter la prise de décision.

## 🎯 Objectifs du Projet
* Suivre les performances des fermiers par région et par type de culture.
* Analyser la répartition géographique des crédits.
* Visualiser les rendements agricoles en fonction des financements accordés.

## 📊 Structure des Données
Le projet s'appuie sur un modèle de données en étoile comprenant les fichiers suivants :
* **FaitAgriculture.csv** : Table de faits contenant les indicateurs de production et les montants.
* **DimFermier.csv** : Informations détaillées sur les bénéficiaires des crédits.
* **DimCulture.csv** : Référentiel des types de cultures (Maïs, Riz, etc.).
* **DimRegion.csv** & **DimVille.csv** : Hiérarchie géographique pour l'analyse spatiale.

## ⚙️ Technologies Utilisées
* **Power BI Desktop** : Pour la modélisation des données (Power Query), les calculs (DAX) et la visualisation.
* **DAX (Data Analysis Expressions)** : Pour la création de mesures personnalisées (Total Crédits, Rendement moyen).

## 📈 Contenu du Dashboard
Le fichier `agriculture_dashboard.pbix` inclut :
* Des indicateurs clés de performance (KPIs) sur le financement total.
* Des graphiques de répartition par région et par ville.
* Des analyses croisées entre le type de culture et le succès du microcrédit.

## 🚀 Comment utiliser ce projet
1.  Assurez-vous d'avoir **Power BI Desktop** installé sur votre machine.
2.  Téléchargez le dossier et ouvrez le fichier `agriculture_dashboard.pbix`.
3.  Si nécessaire, mettez à jour le chemin des sources de données vers les fichiers `.csv` fournis dans le dossier via l'éditeur Power Query.

## 👩‍💻 Auteur
**Solange Ilinga**
Étudiante en ingénierie, passionnée par la Data Science et le développement de solutions technologiques pour l'agriculture.
