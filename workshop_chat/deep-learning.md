# deep-learning

> Infos récupérées

**Saturday 11th June﻿**

loic legoff  [4:23 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1654957424443289)

question sur la video episode 1 video 4 (<https://www.youtube.com/watch?v=2US1r-cYJSg&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=6>): la fonction d'activation heavyside est remplacée par quelque chose de différentiable mais qui ne ressemble pas du tout. Pourquoi ne pas choisir quelque chose de plus sigmoidal? Ca serait plus couteux numériquement sans apporter grand chose sur le résultats?

david.rousseau  [4:25 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1654957523522389)

C'est la fonction de loss qui est remplacée par quelque chose de différentiable. Dans le cas de la détection ces fonctions bornent le heavyside. Donc si on minimise la loss différentiable on minimise aussi le heavyside.

david.rousseau  [5:18 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1654960723799169)

[@loic legoff](https://anfdeepscopie.slack.com/team/U03E0QTDW2D) loic la confusion vient peut être du fait qu'on a deux fonctions non linéaire dans l'affaire. La fonction d'activation est appliquée après chaque convolution et qui n'a pas à être différentiable et  la fonction de loss qui mesure l'écart en la prédiction et la vérité terrain et qui doit être différentiable.



**Monday 13th June﻿**

david.rousseau  [4:16 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655129760082379)

Exercice pour demain : dessine moi un CNN
![](https://seafile.unistra.fr/lib/d20e1a9a-2eb2-4a7f-8aad-0079c88b58c3/file/images/auto-upload/image-1664042091005.png?raw=1)


Marine BREUILLY  [5:31 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655134287462779)

Pour "dessiner" des réseaux, voici un outil en ligne bien sympathique: <http://alexlenail.me/NN-SVG/LeNet.html> (edited) 


![](https://seafile.unistra.fr/lib/d20e1a9a-2eb2-4a7f-8aad-0079c88b58c3/file/images/auto-upload/image-1664042227089.png?raw=1)
**Tuesday 14th June﻿**

Mathieu Fallet  [9:35 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655192145211599)

bonjour, Il y a un point que je n'ai pas bien compris: conv2D(32, (3,3)) signifie que l'on prend 32 features de kernel 3x3, es-ce que les poids de chacun des  9 pixels (compris entre 0 et 1?) sont pris au hasard ou bien  ces features sont determinées par un algo (type ligne vertical, ligne horizontal,...) ? Merci. deuxième question sur le transfer learning, après avoir vu la video où il est discuté de la methode deep features, que signifie billet ? De plus lorsque l'on parle de classifier , on utilise en general la methode de random forest dans le domaine du traitement d'images, d'autres methodes sont utilisées , ou est-ce que c'est indiqué dans le code  ? merci (edited)

Marine BREUILLY  [3 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655193572696779?thread_ts=1655192145.211599&cid=C03DK92G58V)

bonjour, les poids des poids des kernels et du biais sont initialisés par défaut avec les variables :
kernel_initializer="glorot_uniform",

```
[object Object][object Object]
```

 <https://keras.io/api/layers/convolution_layers/convolution2d/>Il existe plusieurs fonction d'initialisation disponibles en boutique: <https://keras.io/api/layers/initializers/> (edited) 



Pierre Hener  [3 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655196920313709?thread_ts=1655192145.211599&cid=C03DK92G58V)


Bonjour, à quel endroit du code d'hier a-t-on fait cela?



Marine BREUILLY  [3 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655205107447839?thread_ts=1655192145.211599&cid=C03DK92G58V)


bonjour [@Pierre Hener](https://anfdeepscopie.slack.com/team/U03DN61U6F4), nous avons dans le modelCNN, nous avons utilisé 3 couches convolutionnelles (Conv2D) en définissant un minimum de paramètres.


> Conv2D(32, (3, 3), activation='relu', input_shape=(28, 28, 1))

Les autres paramètres sont implicites (aléatoires par défaut) donc nous ne les avons explicitement définis.


Marine BREUILLY  [3 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655293782944919?thread_ts=1655192145.211599&cid=C03DK92G58V)


[@Pierre Hener](https://anfdeepscopie.slack.com/team/U03DN61U6F4) et [@Mathieu Fallet](https://anfdeepscopie.slack.com/team/U03E0QT9NGH) dans la definition du resau u net, vous pouvez remarquer que les poids des kernel sont initialisés avec "he_normal" cette fois-ci



david.rousseau  [3:38 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655213885366189)
<https://github.com/stardist/stardist/issues/90>



**Wednesday 15th June﻿**

Mathieu Fallet  [10:00 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655280032563519)
Bonjour, Je me pose la question de pourquoi Cellpose fonctionne si bien, je n'arrive pas à comprendre dans l'article les images de gradient en X et Y et ce qui rend l'algo si puissant. . J'ai vu dans les videos de ce matin que NucleAlzer donne des meilleurs resultats encore. Comment utiliser cet algo, l'avez-vous testé ? Si l'image de depart est un peu bruité, conseillez-vous d'appliquer un median ? Est-ce que la normalisation en intensité des images est également importante ? merci.

david.rousseau  [10:08 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655280533614839)
Pour Cellpose, je crois que la base de donnée y est pour beaucoup notamment par sa diversité. Je n'ai pas testé NucleAlzer. Peut être un nouvel outils à benchmarker pour le Groupe de Travail ([@vernayb](https://anfdeepscopie.slack.com/team/U03EBU9355W)). D'une façon générale tout ce qui peut être compensé sur la base d'a priori physique fort (sûr) doit être fait, possiblement à l'ancienne, avec les outils adaptés (recalage, normalisation, débruitage, homogénéisation spatiale du contraste).


vernayb  [10:13 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655280817166479)
En effet tester avec le GT MAIIA. J'ai aussi compris que la puissance de Cellpose vient de la base de données annotées qui est très diverse

vernayb  [10:16 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655280999789599)
Pour Cellpose: à 1min24 -> 70 000 cells pour l'entraînement <https://www.youtube.com/watch?v=3ydtAhfq6H0>
Specialist Network vs Generalist Network, from 6:55 <https://www.youtube.com/watch?v=7y9d4VIKiS8&t=629s>

Sylvain Prigent  [10:19 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281148338679)
Le dataset d’apprentissage de cellpose est disponible sur leur site: <https://www.cellpose.org/dataset> il est pas si grand en nombre d’images mais très varié

david.rousseau  [10:19 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281148339279)
Dans le domaine des plantes nous avons <https://play.google.com/store/apps/details?id=org.plantnet&hl=fr&gl=US> dont le volume d'image dans la data base dépasse aujourd'hui très largement les bases comme Imagenet... cela permet aux auteurs de commencer à déveloper/imaginer des réseaux pour des applications spécifiques en stratifiant leur base.


loic legoff  [10:20 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281211163569)
un problème pour l'expérimentateur c'est le training. Un jour on veut segmenter des noyaux, le suivant ce sont les contours cellulaires. Dans ce contexte, s'il faut annoter plein de données, on a aussi vite fait de segmenter nos structures par d'autres moyens. Je trouve l'idée des simulations très intéressantes. Quand on voit ce que peut faire Dall.E2 (<https://openai.com/dall-e-2/>) on se dit que ca devrait être possible de créer de très bonnes simulations d'images à partir de coordonnées  de noyaux ou contours cellulaires et d'un logiciel équivalent recréant des textures similaires à nos images. Est-ce que quelque chose dans le style existe dans le cadre de l'analyse d'image?
loic legoff  [3 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281397418859?thread_ts=1655281211.163569&cid=C03DK92G58V)
ou bien la solution est effectivement les datasets partagés comme mentionné dans les messages de ce matin.



vernayb  [10:20 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281227590009)
Et pour Stardist à 33:23 -> 600 images/20k annotations (fluo) et 30 images/22k annotations (H&E) <https://www.youtube.com/watch?v=Amn_eHRGX5M>


david.rousseau  [10:21 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281313339759)
Stardist est juste un U-Net avec une couche de post-traitement basé sur un apriori de convexité des cellules.

Mathieu Fallet  [10:22 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281353025279)
oui alors que Cellpose est un peu plus compliqué non ?
david.rousseau  [3 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281383404309?thread_ts=1655281353.025279&cid=C03DK92G58V)
il n'y a pas d' apriori de convexité dans cellpose.

Mathieu Fallet  [10:28 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281718812839)
Par curiosité comment on rajoute ce genre d'hypothèse au modèle (convexité ou autre) ? Par exemple, est-ce pertinent d'utiliser un modèle et de rajouter un filtre de taille  dans le modèle (pas après) (edited) [10:31](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655281908884999)un objet en forme de haricot n'est pas convexe mais concave ce qui peut être le cas d'un noyau (en fonction du type cellulaire), non ?

Thierry Pécot  [10:56 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655283380207139)
Pour l'efficacité de cellpose, les auteurs l'expliquent par le fait que les cellules présentent une variabilité de formes très grande, ce qui fait que l'algorithme converge rapidement. La segmentation de noyaux nécessitera plus de données car la variabilité de formes entre noyaux est beaucoup moins importante. Par ailleurs, j'ai testé NuclAIzer, mais il y a déjà quelques années. J'avais trouvé à l'époque que c'était un peu une usine à gaz.


Marine BREUILLY  [11:22 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655284940733589)
l'article cité par N Goudin avec les mesures pour la validation des résultats: <https://www.nature.com/articles/s41592-021-01284-3>

Mathieu Fallet  [1:02 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655290927011409)
j'ai une question sur l'application du DL sur le clustering. J'ai une zone plus dense (qui varie en densité d'une image à l'autre) que je voudrais determiner, est-ce que le DL (random forest ?) est capable de m'identifier la population plus dense ou faut t'il mieux utiliser algo type kNN et essayer de détecter deux distances dans l'histo ? je ne sais pas si ça rentre dans le cadre de ce  cours ? merci

[1:05](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655291147979159)les cellules sont déja detectées (position)

david.rousseau  [1:44 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655293493764259)
Présentation Nikon -> VIDEO

[1:49](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655293781064639)Discussion autour de l'EGI -> VIDEO

david.rousseau  [3:12 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1655298722257469)
Biologeek attitude : <https://youtu.be/_U08qRoKof4>

**Thursday 7th July**

loic legoff  [7:10 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1657213832414479)
BOnjour, je ne sais pas si ce canal slack es encore d'actualité. J'ai une question: je souhaite détecter des noyaux cellulaires de différentes tailles dans la meme image (taille liée à la ploïdie des cellules). Je veux avoir la position et la taille des noyaux. C'est Ok s'il y en a des manqués. Il y a des problèmes d'inhomogénéité des intensités (cellules plus brillantes à droite sur l'image). Quel outil recommandez vous ? Cellpose ? stardist? Idéalement j'aimerais que ca marche out of the box sans apprentissage.  Je mets une capture d'écran:
![](https://seafile.unistra.fr/lib/d20e1a9a-2eb2-4a7f-8aad-0079c88b58c3/file/images/auto-upload/image-1664043888271.png?raw=1)

Marine BREUILLY  [2 months ago](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1657528093449349?thread_ts=1657213832.414479&cid=C03DK92G58V)
Bonjour [@loic legoff](https://anfdeepscopie.slack.com/team/U03E0QTDW2D), au vu de l'activité, je me permets de répondre. Je n'ai jamais utilisé Cellpose. Je peux vous recommander "QuPath" (et il y a aussi possibilité d'utiliser StarDist).



**Tuesday 2nd August**

Mathieu Fallet  [5:11 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1659453089347189)
bonjour, je cherche une methode pour traiter les images RGB (trois canaux de fluo). je voudrais identifier des cellules non pas avec un seul canal mais trois canaux. donc des images couleurs. ça devrait marcher avec Pytorch comme pour la reconnaissance d'objets de couleurs (chat,..) , non ? Par exemple, ici je voudrais reconnaitre les noyaux seuls (KI 67), les LT avec et sans noyaux et les LB avec et sans noyaux. comment attaquer le problème ? merci. Bon sujet pour novembre ?
![](https://seafile.unistra.fr/lib/d20e1a9a-2eb2-4a7f-8aad-0079c88b58c3/file/images/auto-upload/image-1664043995952.png?raw=1)

vernayb  [5:21 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1659453667533449)
pas de canal dapi/hoechst pour segmenter tous les noyaux pour commencer?


**Friday 5th August**

Mathieu Fallet  [11:00 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1659690044619869)
Justement dans ce projet on voudrait que les cellules en proliferation (marquage nucleaire KI67) donc on pourrait faire ça (c'est ce qu'on fait, segmentation sur KI67) mais ensuite il faut créer des masques annulaires pour rechercher le marquage membranaire des T et B , faire un scatterplot et identifier les T et B par leur intensité, au passage on perd beaucoup de cellules car certaines cellules ont un marquage annulaire de faible intensité...donc plutôt que de faire ça (c'est ce que je fais déjà), je voudrais essayer directement la detection des LT et LB en prolifération sur les images RGB (KI67=bleu, LT=vert, LB=rouge). Comment attaquer le problème ?

Mathieu Fallet  [1:59 PM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1659700779701089)
ça semble fonctionner avec Ilastik sur des images simulées, en gros les noyaux en bleu sans marquage ne sont pas classifié, en gros il reconnait un anneau vert ou rouge  avec du bleu au centre et en plus en cas de contact ça fonctionne aussi !
![](https://seafile.unistra.fr/lib/d20e1a9a-2eb2-4a7f-8aad-0079c88b58c3/file/images/auto-upload/image-1664044095352.png?raw=1)

**Tuesday 9th August**

Mathieu Fallet  [11:43 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1660038184217829)
<https://www.nature.com/articles/s41598-022-08355-1>

**Thursday 11th August**

Mathieu Fallet  [10:51 AM](https://anfdeepscopie.slack.com/archives/C03DK92G58V/p1660207864683269)
cellpose 2 repond à ma question je crois :  [cellpose 2.0 tutorial: how to train your own cellular segmentation model - YouTube](https://www.youtube.com/watch?v=5qANHWoubZU)












