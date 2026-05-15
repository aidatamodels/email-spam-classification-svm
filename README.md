# Classification de spams avec SVM

## Présentation du projet

Ce projet est un notebook pédagogique de science des données consacré à la classification de courriels à l’aide de l’algorithme SVM, Support Vector Machine.

L’objectif est de construire un modèle capable de distinguer un e-mail légitime d’un spam à partir de la fréquence d’apparition des mots contenus dans le message.

Le projet illustre une démarche complète d’apprentissage automatique supervisé appliquée à la classification de texte : chargement des données, exploration, préparation, séparation entraînement/test, modélisation, évaluation et interprétation des résultats.

## Objectif

Le projet répond à la question suivante :

> Peut-on utiliser un modèle SVM pour classifier automatiquement des e-mails comme légitimes ou spams à partir de leurs caractéristiques textuelles ?

Le notebook vise à expliquer :

- comment charger un dataset réel depuis Kaggle ;
- comment préparer un jeu de données textuel déjà vectorisé ;
- comment séparer les variables explicatives et la variable cible ;
- comment entraîner un modèle SVM avec Scikit-learn ;
- comment évaluer un modèle de classification ;
- comment interpréter une matrice de confusion ;
- pourquoi les faux positifs et les faux négatifs n’ont pas le même impact métier.

## Contexte

Le spam est un problème courant dans l’environnement numérique. Chaque jour, des systèmes automatiques doivent analyser des messages afin de distinguer les communications utiles des messages indésirables.

Derrière ce problème quotidien se trouve un cas d’usage classique de l’apprentissage automatique : la classification binaire.

Dans ce projet, chaque e-mail est représenté par des variables numériques indiquant la fréquence d’apparition de certains mots. Le modèle SVM utilise ces informations pour apprendre une frontière de décision entre deux classes :

| Classe | Signification |
|---|---|
| `0` | E-mail légitime |
| `1` | Spam |

Le but n’est pas de construire un système anti-spam opérationnel complet, mais de démontrer de manière claire et pédagogique comment un modèle de classification peut apprendre à reconnaître des motifs dans des données textuelles.

## Source des données

Le projet utilise le dataset Kaggle :

```text
Email Spam Classification Dataset CSV
