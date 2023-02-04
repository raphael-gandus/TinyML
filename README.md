# Projet 1 | Raphaël GANDUS

J'ai suivi les mêmes étapes qu'en cours avec les exercices du git suivant : https://github.com/walid213/tinyml-workshop

Sauf qu'au lieu d'enregistrer des mouvements de coups de poings (punch et flex) j'ai effectué des mouvements correspondants aux emojis yes et no.

Cependant pour l'emoji no je n'ai pas fait une croix car cela ressemblait trop au yes donc j'ai fait deux lignes horizontales de gauche à droite puis de droite à gauche.

Vous trouverez dans Projet 1 le fichier "model.h" d'entrainement avec les fichiers "yes.csv" et "no.csv", le code source IMU_Classifier.ino utilisé pour le test et les questions, et le fichier colab utilisé pour créer "model.h".

Résultat obtenu : 
![image](https://user-images.githubusercontent.com/95090973/211158129-adf6e45c-cf85-405b-a54f-a15fd0678732.png)



# Projet 2 | Raphaël GANDUS et Hicham GHANEM

Avec mon camarade Hicham nous avons réussi à entrainer un modèle grâce à la plateforme Edge Impulse qui fonctionne à peu près correctement mais il manque sûrement plusieurs dizaines de minutes d'audio pour l'entrainement que nous n'avons pas eu le temps d'enregistrer. Vous trouverez dans Projet 2 le fichier flash pour l'Arduino produit par Edge Impulse.

Résultat : 
![image](https://user-images.githubusercontent.com/95090973/211208929-a826238c-f601-4252-9b21-e2ba04412582.png)


# Projet final : cancer de la peau | Raphaël GANDUS

La caméra fournie avec le kit Arduino Nano 33 BLE est inutilisable car les images sont de très mauvaise qualité (voici une photo de mon bras) : 
![a](https://user-images.githubusercontent.com/95090973/216775182-01bad802-230f-4f32-a7e0-5311785a4f23.jpg)

J'ai donc choisi de prendre des photos de ma peau avec mon téléphone (peau saine) afin d'entrainer le modèle sur Edge Impulse. J'utilise la base de données suivante pour les peaux cancéreuses : https://www.kaggle.com/datasets/nodoubttome/skin-cancer9-classesisic


![peau cancéreuse](https://user-images.githubusercontent.com/95090973/216775280-d963c51f-7966-4b3d-b948-73c675877da2.jpg)
![peau saine](https://user-images.githubusercontent.com/95090973/216775289-71e8913c-3b4b-4198-90a1-9ec5ccba3f1b.jpg)

Ensuite, voici le traitement appliqué aux données : 
![algorithmes](https://user-images.githubusercontent.com/95090973/216775307-0af7ee88-f3d2-4e08-ada5-77e1f709b63f.jpg)

Et les résultats obtenus avec ce modèle : 
![performance](https://user-images.githubusercontent.com/95090973/216775344-93a0b18b-6ad6-4d16-bd06-2272098e17b4.jpg)

Enfin, voici un exemple de live classification sur une portion de ma peau que le modèle ne connaissait pas :
![Mobile client - Edge Impulse](https://user-images.githubusercontent.com/95090973/216775498-e3302f95-9340-4bd9-ac7b-611708dc1f3b.png)


