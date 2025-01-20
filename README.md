# Les plus belles images de l'univers avec le JWST

![image](image.png)

## Description du projet :

Ce projet a pour objectif d’explorer les merveilles de l’univers en utilisant les données du James Webb Space Telescope (JWST). À travers des fichiers de données FITS, nous téléchargeons, analysons et affichons des images spectaculaires.

Notre équipe, composée de Louisa, Lina, Kalvin et Baptiste, travaille sous le nom Loupommedeterre pour transformer ces données en visualisations claires et fascinantes. En parallèle, nous développons des outils et des analyses avancées pour explorer les données sous différents angles.

## Structure du projet : 
Le projet est organisé de la manière suivante : 
```bash  
JWST_Project/ 
├── documentations/ # Explications des bibliothèques et outils utilisés
├── Donnes_fits/ # Données FITS utilisées pour générer les images
├── observation/ # Observations et analyses effectuées sur les images
├── compte_rendus/ # Rapports hebdomadaires sur l’avancement du projet
└── README.md # Documentation principale
```

## Installation et Pré-requis : 

Avant de commencer, assurez-vous d’avoir les éléments suivants :

- Python installé sur votre machine (version 3.8 ou supérieure recommandée).
- Les bibliothèques nécessaires :
```python
pip install astropy matplotlib
```
- Clonez ce dépôt pour accéder aux fichiers du projet :
```python
git clone git@gitlab.univ-lr.fr:projets-l2-2024/loupommedeterre/loupommedeterre.git

```


## Utilisation :

Les scripts Python fournis permettent :

- De télécharger et manipuler les fichiers FITS provenant du JWST.
- D’afficher les images générées à partir des données, avec des options de visualisation personnalisées (ex. : zoom, superposition des canaux).
- D'explorer des fonctionnalités avancées, comme l’analyse des données et le traitement d’images.


## Documentation : 

Pour des explications détaillées sur les bibliothèques, outils ou méthodologies utilisées dans le projet, consultez le dossier documentations. Ce dossier contient des guides sur les bibliothèques Python comme Astropy et Matplotlib, ainsi que des astuces pour travailler efficacement avec les fichiers FITS.

# Bibliothèques utilisées :

Voici les bibliothèques principales que nous utilisons dans le projet :

## Astropy : 
- Outils pour manipuler des unités astrophysiques et lire des fichiers FITS.
- Exemples de fonctions utilisées :

```python
from astropy import units as u
from astropy.io import fits
```

## Matplotlib : 
- Génération des visualisations et gestion des couleurs (échelle logarithmique avec LogNorm).
- Exemples :
```python
import matplotlib.pyplot as plt
from matplotlib.colors import LogNorm
```
## Numpy : 
- Manipulation des tableaux de données numériques, calculs scientifiques et manipulation d'images.
- Exemples :
```python
import numpy as np
# Création d'un tableau NumPy à partir de données FITS
image_data = np.array(fits.getdata('image.fits'))

```
## Streamlit : 

- Création d'interfaces interactives pour visualiser et interagir avec les données du projet.
- Exemples :
```python
import streamlit as st
# Affichage de l'image FITS dans l'application Streamlit
st.image(image_data, caption='Image FITS', use_column_width=True)

```

## Équipe : 

- Louisa Ould Bouali
- Lina Abarou
- Chhin Kalvin
- Roblin Baptiste
- Nom du groupe : Loupommedeterre

## Objectifs futurs : 

- Organisation et amélioration du projet : Structurer le projet pour faciliter son utilisation et son développement.
- Développement d’outils avancés : Ajouter des fonctionnalités comme le zoom interactif, la superposition de canaux et l’analyse approfondie des données.
- Documentation : Produire des supports clairs et détaillés pour accompagner les utilisateurs dans leur exploration des données.
- Préparation d’une présentation finale : Partager nos résultats avec la communauté en créant un diaporama et une synthèse du projet.

