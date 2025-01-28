# Projet de Classification d'Images

## Présentation 

Ce projet se concentre sur la classification supervisée d'images de chiens et de chats.

Nous avons constitué un ensemble de données comprenant 1028 images pour chaque classe, soit un total de 2058 images sur un ensemble plus vaste de 25 000 images. 
Les données utilisées dans ce projet peuvent être téléchargées à l'adresse suivante : [Microsoft](https://www.microsoft.com/en-us).

## Objectifs

Comparer trois types d'architectures de réseaux de neurones : 
- Perceptron Multi-Couches (MLP)
- Réseau de Neurones Convolutifs (CNN)
- Modèle pré-entraîné VGG16

Ensuite déterminer quelle architecture offre la meilleure performance.

## Méthodologie

### Étapes du Projet

1. **Prétraitement des Données**
   - Redimensionnement des images
   - Nettoyage des données
   - Normalisation
   - Séparation en ensembles d'entraînement, de validation et de test

2. **Modélisation**
   - Développement des différentes architectures : MLP, CNN, VGG16
   - Conception et configuration soigneuses de chaque architecture

3. **Évaluation des Performances**
   - Comparaison des résultats obtenus sur les ensembles d'entraînement et de validation
   - Analyse de la précision et de la fonction de perte pour chaque modèle
   - Sélection du modèle le plus performant, en s'assurant qu'il généralise bien sur de nouvelles données
  
### Outils et Technologies

- **Langage** : Python
- **Bibliothèques** : TensorFlow, Keras


