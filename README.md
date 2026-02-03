# Projet_Data_Anime
# 🌸 Anime Analytics : De la Hype à la Data

> **"Un chef-d'œuvre se définit-il par ses sommets ou par sa régularité ?"**

[![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-7db0bc?style=for-the-badge&logo=seaborn&logoColor=white)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Plotting-11557c?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org/)

---

## 📖 À propos du projet

Ce projet de Data Science explore une base de données d'animes pour dépasser le simple classement par popularité. L'objectif est d'utiliser Python pour révéler des tendances cachées sur la qualité, la source d'adaptation et la constance des studios d'animation.

L'analyse se concentre sur une métrique personnalisée : **La Régularité**.

---

## ⚙️ Méthodologie & Feature Engineering

Le jeu de données a été traité avec **Pandas**. Au-delà du nettoyage classique, j'ai créé de nouvelles variables pour affiner l'analyse :

* **`Ecart`** : La différence entre la note du *meilleur épisode* et celle du *pire épisode*.
* **`Regularite`** (Score sur 10) : Une formule inversée pour récompenser la constance.
    $$Regularite = 10 - (Note_{Meilleur} - Note_{Pire})$$
* **`Longueur`** (Log scale) : Utilisation du logarithme du nombre d'épisodes pour visualiser efficacement les séries courtes (12 épisodes) face aux séries fleuves (Naruto, DBZ) sur le même graphique.

---

## 📊 Visualisations Clés

### 1. Le Top 10 : La Crème de la Crème 🏆
Analyse des notes globales. On remarque la domination des titres récents comme *Frieren* aux côtés de classiques indétrônables comme *Fullmetal Alchemist: Brotherhood*.

![Top 10 Animes]

### 2. L'impact de la Source Originale 📚
D'où viennent les meilleures histoires ? L'analyse révèle que les adaptations de **Visual Novels** et les œuvres **Originales** ont souvent une moyenne supérieure aux adaptations de Mangas classiques.

![Source Analysis]

### 3. L'Analyse Finale : Qualité vs Régularité vs Longueur 🎯
C'est le cœur du projet. Ce scatterplot multidimensionnel permet de segmenter les animes :

* **Axe X (Régularité)** : Plus on va à droite, plus l'anime est constant.
* **Axe Y (Note Globale)** : La qualité générale.
* **Taille des bulles** : La longueur de la série.
* **Couleur** : L'intensité de l'écart type.

![Scatter Plot Final]

> **Insight :** Les "Chefs-d'œuvre absolus" se trouvent dans le coin supérieur droit (Haute Note + Haute Régularité). On remarque aussi que maintenir une régularité parfaite est un défi majeur pour les animes longs (grosses bulles).

---

## 🚀 Comment utiliser ce notebook

1.  **Cloner le repo**
    ```bash
    git clone [https://github.com/votre-username/anime-analytics.git](https://github.com/votre-username/anime-analytics.git)
    ```
2.  **Installer les dépendances**
    ```bash
    pip install pandas seaborn matplotlib numpy
    ```
3.  **Lancer Jupyter**
    ```bash
    jupyter notebook
    ```

---

## 📝 Auteur

Projet réalisé par Louis Nourry
Passionné par la Data Visualization et la Pop-culture.

*N'hésitez pas à étoiler ⭐ ce repo si l'analyse vous a plu !*
