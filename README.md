# Multilayer-Perceptron-Python
Multilayer Perceptron with Python on Mnist Data

Data: 
Le fichiermnist_all.csvcontenant les données est fourni au format .csv sans entête et avec la virgule comme séparateur.Il provient d’une extraction de la base MNIST1. Ce fichier comporte 70000 images qu’il faudra répartir dans 3 fichiersafin d’établir les corpus d’apprentissage, de test et de validation. Elles sont constituées d’imagettes normalisées de 28pixels de côté de chiffres manuscrits numérisés en 256 niveaux de gris. La normalisation a été réalisée automatiquementen calculant le centre de masse des pixels, et en translatant l’image de manière à positionner ce point au centre duchamp 28x28.

Objectif :
L’objectif ce devoir est de produire plusieurs modèles des réseaux de neurones exclusivement sur la base surleperceptron multi-couche et sur l’algorithme de rétro-propagationen jouant surles hyper-paramètres, afinde réaliser un apprentissage supervisé. Puis de discuter la qualité de déduction des différents réseaux obtenu grâce à lamise en place d’une expérimentation.


Ce notebook contient plusieurs fonction:
1.une fonction de lecture d’un fichier au format .csv 
2.une fonction de production de l’ensemble des données d’apprentissage, des données de test et des données devalidation. 
3.des fonctions de création dedatasetadaptée à la bibliothèquetensorflow
4.une fonction de mélange et de définition dubatchpour le dataset. Il est essentiel de mélanger l’ensemble dedonnées lors de la phase d’apprentissage et de pouvoir indiquer le nombre d’exemple à fournir pour chaqueretro-propagation (taille dubatch). Une taille debatchà 1 impliquera qu’à chaque présentation d’exemple enentrée du réseau, le résultat sera retro-propagé.
5.ne fonction qui permet de définir le modèle de réseau de neurone que l’on souhaite exécuter :—le modèlesequentialdetensorflowest un empilement linéaire de couches denses, autrement dit unperceptron multicouche.
6.une fonction de sauvegarde au ‘fil de l’eau’. Elle doit permettre de réutiliser un modèle stabilisé après laphase d’apprentissage sans avoir à relancer cette phase. Elle peut également permettre de reprendre l’ap-prentissage là où vous l’avez laissé, au cas où le processus d’apprentissage aurait été interrompu. L’appel àtensorflow.keras.callbacks.ModelCheckpointpermet de sauvegarder en permanence le modèle pendant età la fin de la phase d’apprentissage.

