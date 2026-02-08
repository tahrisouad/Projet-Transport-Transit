# 🚌 Transit Ridership Analysis Dashboard (Chicago & Philadelphia)

## 📌 Présentation du Projet
Ce dépôt contient une solution de Business Intelligence complète pour analyser et piloter la performance des transports urbains de **Chicago** et **Philadelphie**. Le projet permet de visualiser la fréquentation (Ridership) par mode de transport et par ligne (Route) pour optimiser la gestion du trafic.

---

## 📂 Structure du Repository
```text
├── data/               # Fichiers CSV nettoyés (Export final de Python)
├── data_raw/           # Fichiers sources bruts (RDF, Excel, CSV)
├── powerbi_model/      # Fichier source Power BI (.pbix)
├── scripts_python/     # Notebooks Jupyter de prétraitement (ETL)
├── docs/               # Screenshots et documentation complémentaire
└── README.md           # Guide du projet
```



## 🛠️ Stack Technique
Langage : Python 3.12+

Bibliothèques : pandas pour la manipulation de données, rdflib pour le parsing des fichiers RDF

BI Tool : Power BI Desktop (Modélisation en Étoile & DAX)

Gestion de Projet : Méthodologie Agile avec Jira & Confluence

## ⚙️ Guide d'Installation et Déploiement
### A. Prérequis
* Python : Installer une version stable (3.10, 3.11 ou 3.12).

* Power BI Desktop : Téléchargeable gratuitement sur le Microsoft Store.

* Bibliothèques : Installez les dépendances via le terminal :

``` Bash
pip install pandas rdflib 
```
### B. Étapes d'exécution
**1. Clonage :**

``` Bash
git clone https://github.com/tahrisouad/Projet-Transport-Transit.git
```
**2. ETL Python :**

Exécutez les notebooks dans **scripts_python/** pour transformer les fichiers de **data_raw/** vers **data/**.

**3. Chargement Power BI :**

Ouvrez **powerbi_model/brief00.pbix**.

⚠️ Mise à jour des sources : Si les graphiques ne s'affichent pas, allez dans Transformer les données > Paramètres de la source de données et modifiez le chemin d'accès.

Cliquez sur Actualiser.

## 📊 Aperçu du Dashboard
Le rapport est structuré en deux axes stratégiques :

**1. Analyse par Mode**
Analyse macro de la fréquentation. On يلاحظ que le Bus représente 57,45% de l'utilisation totale.

**2. Analyse Détaillée des Routes**
Analyse granulaire des 194 lignes de transport.

## 🧠 Intelligence DAX & KPIs
Le projet utilise des mesures DAX avancées pour le pilotage :

**Total Ridership :** SUM(Ridership) (Total de 2,01 Md).

**Growth% :** Analyse comparative mensuelle.

**Max Ridership :** Identification des pics (136K).

## ⚙️ Méthodologie & Gestion de Projet
Pour assurer une organisation optimale et une documentation rigoureuse, ce projet a suivi une approche structurée :

* **Gestion des Tâches (Jira)** : Utilisation de **Jira** pour la planification des sprints و suivi des tâches (To-Do, In Progress, Done).
  * 🔗 [Accéder au Tableau Jira](https://tahrisouad96.atlassian.net/jira/software/projects/TPA/boards/1?atlOrigin=eyJpIjoiNjMwN2IyYTVhNTJhNGQ5YmIxYjZiYmRmMzAwZmMxNTYiLCJwIjoiaiJ9)

* **Documentation (Confluence)** : Rédaction d'une documentation complète incluant le dictionnaire de données و les choix techniques.
  * 🔗 [Consulter la Documentation Confluence](https://tahrisouad96.atlassian.net/wiki/pages/resumedraft.action?draftId=2490369&draftShareId=07b8606b-f62d-4ecb-ad16-3c50c0339535)

Projet réalisé dans le cadre d'une analyse de performance de transport urbain (2025).