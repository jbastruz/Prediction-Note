# Estimation de la note d'un commentaire avec Mistral.ai, XGBoost et TensorFlow

<p align="center">
    <img src="https://vectorseek.com/wp-content/uploads/2023/12/Mistral-AI-Icon-Logo-Vector.svg-.png" alt="Mistral.ai" width="40" style="margin-right: 20px;" align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/2/2d/Tensorflow_logo.svg" alt="TensorFlow" width="35" align="center">
</p>

Ce dépôt contient un notebook Jupyter qui explore la possibilité d'utiliser les embeddings fournies par Mistral.ai pour prédire la note associée à un commentaire. Le notebook utilise XGBoost et TensorFlow comme méthodes d'entraînement du modèle de prédiction.

## Aperçu

Le notebook est divisé en plusieurs sections :

1. **Prétraitement des données** : Cette section prépare les données en effectuant un prétraitement des commentaires et en récupérant les embeddings associées. Les données sont ensuite divisées en un ensemble d'entraînement et un ensemble de test.

2. **Entraînement du modèle avec XGBoost** : Cette section utilise l'algorithme de classification XGBoost pour prédire la note associée à chaque commentaire.

3. **Entraînement du modèle avec TensorFlow** : Cette section crée un réseau de neurones profond avec plusieurs couches cachées et une couche de sortie avec cinq neurones, correspondant aux cinq notes possibles.

4. **Évaluation du modèle** : Cette section évalue les performances du modèle sur l'ensemble de test en utilisant des métriques telles que la précision, le rappel et le score F1. Les performances des deux méthodes sont comparées pour déterminer celle qui convient le mieux au problème.

## Méthodologie

Pour accélérer le traitement des commentaires et de leurs embeddings, nous utilisons la méthode des chunks. Cette approche consiste à diviser les données en plusieurs morceaux, ce qui permet de gérer les données de manière plus efficace et rapide.

Une fois les embeddings récupérées, nous utilisons deux méthodes distinctes pour entraîner notre modèle de prédiction : XGBoost et TensorFlow.

**XGBoost** est un algorithme de gradient boosting qui a fait ses preuves dans de nombreux domaines d'application, notamment pour la classification et la régression.

<p align="center">
    <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdzone.com%2Fstorage%2Ftemp%2F13069527-boosting-algo.png&f=1&nofb=1&ipt=1ac6f470930257e0fb83997b0768a166f0c2b93a8ecd29dfc184c95efd1e786d&ipo=images" alt="XGBoost" width="500">
</p>

**TensorFlow** est une bibliothèque open source pour l'apprentissage automatique qui permet de créer des réseaux de neurones profonds et complexes.

<p align="center">
    <img src="https://s3.amazonaws.com/stackabuse/media/intro-to-neural-networks-scikit-learn-3.png" alt="neural network" width="300">
</p>

## Conclusion

Ce notebook vise à explorer la faisabilité d'utiliser les embeddings fournies par Mistral.ai pour prédire la note associée à un commentaire. En utilisant deux méthodes distinctes, nous cherchons à déterminer la meilleure approche pour résoudre ce problème et à évaluer les performances de notre modèle.
