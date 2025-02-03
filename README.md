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
  

### 2️⃣ **Entraînement des Modèles**

Après le prétraitement, nous avons entraîné et comparé trois architectures de réseaux de neurones :

- **Perceptron Multi-Couches (MLP)** : développé **from scratch** pour servir de baseline et évaluer les performances des modèles plus avancés.
- **Réseau de Neurones Convolutifs (CNN)** : également développé **from scratch**, conçu spécifiquement pour l’analyse d'images.
- **Modèle pré-entraîné VGG16** : exploité via **deux stratégies de transfert d'apprentissage** :  
  - **Transfert pur** : seule la dernière couche est modifiée, tandis que les couches préexistantes de VGG16 sont conservées et gelées.  
  - **Fine-tuning** : certaines couches de VGG16 sont dégelées et réajustées pour mieux s'adapter à notre tâche spécifique.

L’entraînement a été réalisé avec les éléments suivants comme base et d'autres élements selon les besoins spécifiques de chaque modèle :  
- ✅ Optimiseur 
- ✅ Fonction de perte 
- ✅ Taux d’apprentissage



### 3️⃣ **Évaluation des Performances (Entraînement/Validation et sur le Test)**

L’objectif principal de cette étape était de sélectionner le modèle le plus performant et d’évaluer sa capacité à généraliser sur des données non vues.

#### **3.1 Évaluation sur les Ensembles d'Entraînement et de Validation** :
- Sélection du meilleur modèle en fonction de la **combinaison optimale de la perte qui diminue** et de la **précision qui augmente** sur l'ensemble de validation. Cette évolution conjointe assure que le modèle généralise bien, apprenant à prédire correctement tout en évitant le surapprentissage.

#### **3.2 Évaluation sur l’Ensemble de Test** :
- Utilisation de la **matrice de confusion** pour analyser les erreurs de classification (faux positifs, faux négatifs).
- Calcul et analyse de la **courbe ROC** et de l’**AUC** pour mesurer la capacité du modèle à discriminer efficacement entre les classes.


 
## 🛠️ **Outils et Technologies**

- **Langage** : Python
- **Bibliothèques** : TensorFlow, Keras, OpenCV

