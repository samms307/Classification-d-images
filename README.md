# 🐶🐱 Classification supervisée d'images de chiens et de chats  

## Présentation  
Ce projet se concentre sur la classification supervisée d'images de chiens et de chats.  

Nous avons constitué un ensemble de données comprenant **1 028 images pour chaque classe (chiens et chats)** soit un total de **2 058 images** extraites d'un ensemble plus vaste de **25 000 images**.  

Les données utilisées dans ce projet peuvent être téléchargées à l'adresse suivante : 🔗 [Microsoft Dataset](https://www.microsoft.com/en-us)  


## 🎯 **Objectifs**
L'objectif principal de ce projet est de développer un algorithme capable de classer correctement une nouvelle image en tant que chien ou chat.

Pour cela, nous avons comparé trois architectures de réseaux de neurones :
- Perceptron Multi-Couches (MLP)
- Réseau de Neurones Convolutifs (CNN)
- Modèle pré-entraîné VGG16

L’analyse s’est portée sur la précision, le temps d'entraînement et la complexité afin de déterminer quelle architecture offre les meilleures performances.


# 📈 **Étapes Clés du Projet**

### 1️⃣ **Prétraitement des Données**

Le prétraitement des images a été effectué via un pipeline automatisé, incluant plusieurs étapes essentielles :

- **Séparation des données en trois ensembles** : entraînement, validation et test.
- **Redimensionnement** des images pour assurer une taille uniforme.
- **Normalisation** des pixels afin d'améliorer la convergence du modèle.
- **Nettoyage des données** incluant :
    - Uniformisation des canaux de couleur (conversion en RGB si nécessaire).
    - Gestion des images floues pour garantir la qualité des entrées.
  
L
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


🛠️ Technologies utilisées
Python
TensorFlow / PyTorch
OpenCV
Matplotlib & Seaborn (visualisation)
