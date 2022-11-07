### Table des matières
1. [Antisèches](#antiseches)
1. [Base de données](#BDD)
1. [Conseil software](#software)
1. [Conseil hardware](#hardware)
1. [Conseil langage de programmation](#langageprog)
1. [Plugins ImageJ/Fiji](#fiji)
1. [Culture/Applications diverses du Deep Learning](#culture)
1. [Ressources vidéos](#videos)
1. [Ressources biblio](#biblio)
1. [Cours en ligne](#onlinecourse)
1. [Communauté - Forums](#networking)
1. [FAQ Slack](#faq-1)
1. [FAQ Skype](#faq-2)

<hr>

# **Antisèches - Cheat Sheet<a name="antiseches"></a>**
1. [Deep learning Cheat Sheet](https://www.globalsqa.com/deep-learning-cheat-sheet/)
1. [Cheatography about Neural Networks](https://cheatography.com/lwebzem56/cheat-sheets/neural-networks-for-machine-learning/)
1. Glossaire
      * [ZeroCostDL4Mic](https://github.com/HenriquesLab/ZeroCostDL4Mic/wiki/Glossary)
      * [la CNIL](https://www.cnil.fr/fr/intelligence-artificielle/glossaire-ia)
      * [Grand Lexique Francais de l'IA](https://datafranca.org/wiki/Accueil)
      * [Peltarion's AI glossary](https://peltarion.com/knowledge-center/documentation/glossary)
      * [Difference Between a Batch and an Epoch in a Neural Network](https://machinelearningmastery.com/difference-between-a-batch-and-an-epoch/)
      * [Receptive field](https://theaisummer.com/receptive-field/)
1. Représentation visuelle des réseaux neuronaux
      * [Dessine-moi un "CNN"](http://alexlenail.me/NN-SVG/LeNet.html)

<hr>

# **Base de données partagées<a name="BDD"></a>**
1. Images / Données
      * [MNIST](https://fr.wikipedia.org/wiki/Base_de_donn%C3%A9es_MNIST): Modified ou Mixed National Institute of Standards and Technology, est une base de données de chiffres écrits à la main. La [base MNIST](http://yann.lecun.com/exdb/mnist/) est devenue un test standard, constituée de 60,000 images d'apprentissage et 10,000 images de test
      * [Cytomine](https://open.cytomine.com/)
      * [OpenMicroscopy](https://www.openmicroscopy.org/omero/)
      * [Cellpose](https://www.cellpose.org/dataset)
      * [Pl@ntNet: images de plantes](https://www.gbif.org/dataset/search?hosting_org=da86174a-a605-43a4-a5e8-53d484152cd3)
1. Modèles de Deep-Learning pré-entraînés:
      * [BioImage Model Zoo : Advanced AI models in one-click](https://bioimage.io/#/)
      * [Models Keras pré-entrainés](https://keras.io/api/applications/)
1. Gestion de formats d'images
      * [OMERO](https://www.openmicroscopy.org/omero/)
      * [Hierarchical Data Formats - HDF5](https://en.wikipedia.org/wiki/Hierarchical_Data_Format)
<hr>

# **Conseil outils et logiciels par thème<a name="software"></a>**
1. **Annotation**

[Une présentation de différents outils par B. Vernay](https://gitlab.com/igbmc/mic-photon/anf_deepscopie/-/blob/main/documents_ressources/2021_ANF_Labelling_Bioimages_for_Deep_Learning_v03.pdf).

[Une vidéo avec les différents outils](https://www.youtube.com/watch?v=rB6kG3fMNMA&t=530s)

[La compilation des vidéos du groupe ImHorPhen Bio-imaging](https://youtube.com/playlist?list=PLUukCwr0iCefUhA50m8TREn9GpzTwv_fD)

Liste *non exhautive* des outils pour faire de **l'Annotation sémantique / instance = classification de pixels**
* [Cytomine](https://open.cytomine.com/)
* [Fiji (ROI -> Label mask)](https://sites.imagej.net/SCF-MPI-CBG/)
* [Labkit (2D et 3D)](https://imagej.net/plugins/labkit/)
* [QuPath (2D)](https://qupath.readthedocs.io/en/stable/docs/starting/annotating.html)
* [AnnotatorJ](https://github.com/spreka/annotatorj) 
* [GIMP](https://www.gimp.org/) 
* [ITK-SNAP (3D)](http://www.itksnap.org/pmwiki/pmwiki.php): [vidéo](https://docs.google.com/presentation/d/1ff6T2KhrSm1NSI3LQCn5IWcE41GKevNmvlES4KBnfXk/edit?urp=gmail_link)
* [Paintera (3D)](https://github.com/saalfeldlab/paintera)
* [3D Cell Annotator (3D)](http://www.3d-cell-annotator.org)
* [KNOSSOS (3D)](https://knossos.app), [webKnossos (inplementation web de knossos)](https://docs.webknossos.org)
* [Humans in the loop (online - by others - collaboratif)](https://humansintheloop.org/), [presentation](https://docs.google.com/presentation/d/1AFbuWu_EemdF6UqAiOEH7TpFKac0sB9z7wPOcrpQoDI/edit#slide=id.gd0a87e1865_3_66)
* [Zooniverse (online - by others - collaboratif)](https://www.zooniverse.org/), [vidéo](https://www.youtube.com/watch?v=dCPv536TEIw&t=538s)
* [Cytomine (online - by others)](https://open.cytomine.com/), [vidéos](https://www.youtube.com/watch?v=ygdL3VLegEc&t=3s)
* [SLIC superpixels = Simple Linear Iterative Clustering](https://www.epfl.ch/labs/ivrl/research/slic-superpixels/)

Liste *non exhautive* des outils pour faire de **l'Annotation d'objets / classification d'objets**
* [LabelImg (2D+t)](https://github.com/tzutalin/labelImg) 
* [Labelme (2D)](https://github.com/wkentaro/labelme) 
* [Make Sense (online)](https://www.makesense.ai/)


2. **Détection de noyaux et/ou cellules**
      * [ilastik](https://www.ilastik.org/)
      * [Cellpose](http://www.cellpose.org/) et sa [documentation](https://cellpose.readthedocs.io/en/latest/index.html)
      * [StarDist](https://stardist.net/#)
      * [nucleAIzer : outils en ligne](http://www.nucleaizer.org/)

1. *Visualisation des données*
      * [napari](https://napari.org/stable/index.html)
      * [Fiji - avec hyperstack]

1. **Logiciel (?)**
      * TissueAnalyzer, avec intégration possible de Cellpose
      * TissueMiner

1. **Augmentation de données (Librairies (python))**
      * [Augmentation de données pour les images de microscopie the needs of microscopy images analysis by M Weigert](https://github.com/stardist/augmend)
      * [Ensemble très grand de techniques d'augmentation de données](https://imgaug.readthedocs.io/en/latest/)
      * [Augmentation de données pour la 3D](https://torchio.readthedocs.io/index.html)
      * [Augmentation pour images 2D Très large bande + rapide](https://albumentations.ai/)
      * [Augmentation pour images IRM](https://github.com/MathFLDS/MRAugment)

1. [NGROK](https://ngrok.com) Utile pour visualiser les courbes d'apprentissage et de coût (loss) dans Google Colab.
1. [ZeroCostDL4Mic]( https://github.com/HenriquesLab/ZeroCostDL4Mic)
1. Comparaison (Benchmark) de protocoles d'analyse:
      * [BIAflows](https://biaflows-sandbox.neubias.org/#/)

<hr>

# **Conseil hardware / achat matériel<a name="hardware"></a>**
1. [Choix du GPU en 2021: Quadro, Ampere, GeForce Compared](https://www.youtube.com/watch?v=pWzlL51oqRo) 
1. [Panorama des ressources en calcul intensif (GPU externe)](https://www.youtube.com/watch?v=Se3lkb9eWA8&t=259s)
1. [Data centric AI Resource Hub](https://datacentricai.org/)
1. Si pas de moyens pour s'équiper, utiliser les ressources en ligne:
      * [Deep Hybrid Datacloud platform - si pas de moyen pour ach](https://raw.githubusercontent.com/deephdc/deep-docs/master/source/_static/overview.pdf)
      * [Google Colab](https://colab.research.google.com/)
      * [Grille européenne de calcul : EGI](https://www.egi.eu/egi-ace-open-call/)

Conseil pour l'achat d'un GPU:
1) Discussion avec un IT admin 
2) Choisir un GPU déconnecté de l'écran
3) Choisir un GPU avec assez de RAM pour l'imagerie
4) Choisir un GPU adapté à la machine d'accueil
5) Choisir un GPU qui supporte les bonnes versions des logiciels utilisés

<hr>

# **Environnement logiciel pour le deep learning<a name="langageprog"></a>**
1. [Python et ses nombreuses librairies](https://www.unite.ai/10-best-python-libraries-for-deep-learning/) TensorFlow, Pytorch, NumPy,Scikit-Learn, SciPy, Pandas, Microscoft CNTK, Keras, Theano, MXNet
      * TensorFlow
            * [Installation from scratch](https://www.youtube.com/watch?v=bIU9gVoEFXo&t=216s)
            * [Augmentation de données](https://www.tensorflow.org/tutorials/images/data_augmentation)
1. [R]()
1. [Julia](https://deeplearningwithjulia.com/)

<hr>

# **Plugins ImageJ/Fiji<a name="fiji"></a>**
1. Localisation d'objets en microscopie: 
[Multi-Template-Matching: detection d'objets unique ou multiple](https://imagej.net/plugins/multi-template-matching)
1. Tracking d'objets + visualisation + édition + analysis:
[TrackMate](https://imagej.net/plugins/trackmate)
1. Detection de cellules/noyaux avec a priori de convexité:
[StarDist](https://imagej.net/plugins/stardist). Conseil pour convertir un modèle Stardist pour être utilisé dans Fiji [ICI] (https://github.com/stardist/stardist/issues/90). Conseil pour convertir un modèle Stardist pour être utilisé dans [QuPath](https://forum.image.sc/t/unspecified-error-while-loading-self-trained-stardist-model/71626/10?u=marbre2)
1. Méthode de morphologie mathématiques :
[MorphoLibj](https://imagej.net/plugins/morpholibj)
<hr>
1. Génération de ROIs à partir d'images de label, avec option d'erosion et de quantification
[LabelsToROIs](https://labelstorois.github.io/)
1. Utilisation de modèles DL déjà entrainés dans imageJ [deepImageJ](https://deepimagej.github.io/deepimagej/)

# **Culture/Applications diverses du Deep Learning<a name="culture"></a>**
1. Création d'images réalistes et artistiques à partir d'une information textuelle: 
[DALL-E 1](https://openai.com/blog/dall-e/),
[DALL-E 2](https://openai.com/dall-e-2/)
1. Comment programmer des voitures autonomes ? perspectives humaines vs intelligence artificielle:
[Moral Machine](https://www.moralmachine.net/hl/fr)
1. Musique: [a Eurovision song created by Artificial Intelligence: Blue Jeans and Bloody Tears
](https://www.youtube.com/watch?v=4MKAf6YX_7M)
1. Cinéma: [l'excellent Yves qui imaginait justement en 2019 que des robots combattent à l'eurovision. Une des scènes le plus hilarantes est le combat de recettes par des "frigo intelligents" ... l'un étant nourri de données, disons plus riches que l'autre, par son propriétaire](https://www.youtube.com/watch?v=qOULNcVTDvM)
1. Santé: [Santé numérique : peut-on tout prédire ? - Magazine de l'Inserm n°53](https://fr.calameo.com/read/0051544505fe386bdf46b)

<hr>

# **Ressources vidéos<a name="videos"></a>**
1. Chaîne Youtube [ImHorPhen Bio imaging research group - Deep learning full pack](https://youtube.com/playlist?list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F):
      * [Automatic hyperparameter tuning by Pejman](https://www.youtube.com/watch?v=HHlYUdWV4Vk)
      * [Deep learning with real world data sets](https://youtu.be/UIE3PcIPShY)
1. Chaîne Youtube sur l'analyse d'images (dont ML et DL) en python

> 290 vidéos le 03/11/2022 [Digital Sreeni](https://www.youtube.com/channel/UC34rW-HtPJulxr5wp2Xa04w)

<hr>

# **Ressources biblio<a name="biblio"></a>**
1. Livres:
      * [Deep Learning With Python](amazon.fr/Deep-Learning-Python-Fran%C3%A7ois-Chollet/dp/1617296864/ref=d_pd_vtp_sccl_2_1/258-9236609-1746668?pd_rd_w=4BxgM&content-id=amzn1.sym.226a1123-c0e2-45e0-bcf2-51becbdb358f&pf_rd_p=226a1123-c0e2-45e0-bcf2-51becbdb358f&pf_rd_r=6HPKPENCYHVRQ6VYJF2M&pd_rd_wg=3ueiO&pd_rd_r=fb9c3721-ba73-4013-832f-7c47cd68940a&pd_rd_i=1617296864&psc=1), François Chollet, avril 2022, 2e éd.
      * [Deep Learning avec Keras et TensorFlow - _Mise en oeuvre et cas concrets: Mise en oeuvre et cas concrets_](amazon.fr/Deep-Learning-avec-Keras-TensorFlow/dp/2100790668), Aurélien Géron, mai 2020, 2e éd.
      * [Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow](https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/), Aurélien Géron, sept 2019, 2e éd.
      * [The Deep Learning Book](https://www.deeplearningbook.org/), 2016, Ian Goodfellow, Yoshua Bengio et Aaron Courville.

1. Articles + codes:
      * [Paperwithcode](https://paperswithcode.com/)
1. Articles:
      * [BioImage Model Zoo: A Community-Driven Resource for Accessible
      Deep Learning in BioImage Analysis](https://www.biorxiv.org/content/10.1101/2022.06.07.495102v1.full.pdf)
      * [Active Learning = A Survey of Human-in-the-loop for Machine Learning](https://arxiv.org/pdf/2108.00941.pdf)
      * [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
      * [A Survey of Visual Transformers](https://arxiv.org/abs/2111.06091)
      * [Bayesian Optimization is Superior to Random Search for Machine Learning Hyperparameter Tuning: Analysis of the Black-Box Optimization Challenge 2020](https://arxiv.org/abs/2104.10201)
      * [Les propriétés statistiques des images naturelles](https://www.princeton.edu/~wbialek/our_papers/ruderman+bialek_94.pdf): Pourquoi un pré-entraînement sur des images naturelles fonctionne sur à peu prêt n'importe quoi qui contient des objects de toute taille?
      * [Data augmentation in microscopic images for material data mining](https://www.nature.com/articles/s41524-020-00392-6) Librairies spécifique pour la microscopie des matériaux
      * [High-plex Multiomic Analysis in FFPE at Subcellular Level by Spatial Molecular Imaging](https://doi.org/10.1101/2021.11.03.467020)
      * [Noise2Void - Learning Denoising from Single Noisy Images](https://paperswithcode.com/paper/noise2void-learning-denoising-from-single)
      * [EPySeg: a coding-free solution for automated segmentation of epithelia using deep learning](https://doi.org/10.1242/dev.194589) et son [code package Python](https://github.com/baigouy/EPySeg)
      * [Opening the Black Box of Deep Neural Networks via Information](https://arxiv.org/abs/1703.00810)
      * [Opening the black box of deep learning](https://arxiv.org/abs/1805.08355)
      * [Revisiting Small Batch Training for Deep Neural Networks](https://arxiv.org/abs/1804.07612)
      * [Omnipose: a high-precision morphology-independent solution for bacterial cell segmentation](https://www.nature.com/articles/s41592-022-01639-4) avec le [code](https://omnipose.readthedocs.io/)


1. Inpainting  = Interpolation intelligente des pixels d'image avec deep learning
      * [Adversarial Large-scale Root Gap Inpainting](https://openaccess.thecvf.com/content_CVPRW_2019/papers/CVPPP/Chen_Adversarial_Large-Scale_Root_Gap_Inpainting_CVPRW_2019_paper.pdf)
      * [Image inpainting based on deep learning: A review](https://doi.org/10.1016/j.displa.2021.102028)
      * [CARE = Content-aware image restoration: pushing the limits of fluorescence microscopy](https://www.nature.com/articles/s41592-018-0216-7)

1. Validation des résultats
      * [Avoiding a replication crisis in deep-learning-based bioimage analysis](https://www.nature.com/articles/s41592-021-01284-3)

1. A trier
      * [Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization](https://arxiv.org/abs/1610.02391)
      * [A Survey of Deep *Active Learning*](https://dl.acm.org/doi/abs/10.1145/3472291) autre [lien](https://arxiv.org/pdf/2009.00236.pdf?ref=https://githubhelp.com)


<hr>

# **Cours en ligne<a name="onlinecourse"></a>**
1. [CS231n Convolutional Neural Networks for Visual Recognition](https://cs231n.github.io/)
1. [Python for Bioimage Analysis Course](https://github.com/RMS-DAIM/Python-for-Bioimage-Analysis)
1. [NEUBIAS Academy @Home: Interactive Bioimage Analysis with Python and Jupyter](https://github.com/guiwitz/neubias_academy_biapy): notebooks #1 à #4 pour les bases des images en python
1. [(IAFIG-RMS) Python for Bioimage Analysis Course](https://github.com/RMS-DAIM/Python-for-Bioimage-Analysis)
<hr>

# **Communauté - Forums - Réseaux<a name="networking"></a>**
1. [Forum pour tous les logiciels open-source](https://forum.image.sc/)
1. [Groupe de travail « Méthodes d'analyses d'images par IA » (GT MAIIA)](https://rtmfm.cnrs.fr/gt/gt-maiia/)

``` To subscribe to the list GT MAIIA:
1- Send a message to sympa@services.cnrs.fr from the address you want to subscribe to the list with,
2- In the subject line of your message, type in: subscribe anfdl4mic-mfm@services.cnrs.fr yourFirstname yourLastName
3- Leave the message body blank.
```
3. [Forum "stackoverflow" pour les questions "programmation"](https://stackoverflow.com/)
Il faut regarder les réponses avec le plus de "coches vertes" qui seront le plus souvent les plus pertinentes.

<hr>

# **FAQ Slack<a name="faq-1"></a>**
1. Quand on ne sait pas résoudre un problème de segmentation/classification avec des filtres/méthodes classiques, on utilise le Machine Learning ? 

> Oui tout à fait. La machine vient à notre secours pour résoudre un problème qu'on juge trop complexe. Sur des sujets simples... c'est toujours utile d'utiliser les méthodes classiques.

2. Cellpose qui fonctionne pas mal mais avec des bugs sur certaines cellules très simple à detecter. Faut t'il faire un fine tuning (reapprentissage léger...) ?

> Sans doute oui.

3. Quelle est l'influence du bruit sur l'entrainement, je vois que cela reste un problème pour le ML, pour le resoudre faut t'il également faire un fine tuning (ex dapi bruité : utiliser cellpose et réapprendre sur des images bruitées) ? 

> On utilise ce qu'on appelle de la data augmentation. Il y a une série de vidéo sur le sujet dans le cours.

4. Lorsque l'on utilise un Ilastik sur des objects et sur le fond, en general on recupère tous les objets separées du fond mais pas segmentées entre eux. Est-ce possible aussi de les segmenter eux avec Ilastik...?

> On appelle cette étape: segmentation "instancielle" (distinguer les différents éléments d'une même classe). 
C'est du post traitement... jouable avec un watershed. On peut aussi imaginer ajouter une 3ième classe appelée frontière virtuelle (voir la vidéo sur le sujet) et qui permet de séparer les objets si il y a un contraste dans les interstices.

5. Peux-t'on avec le ML, à partir d'un marquage membranaire discontinu d'une cellule, recréer un marquage continu et comment (simulation) ? 

> La question fait plus penser à une approche de type modèle. Le ML est plutôt basé data et n'incorpore pas par défaut (dans les architectures de bases) des aspects de morphométrie comme boucher les trou ou interpoler. 
On appelle cette étape "Inpainting" et il existe toutefois des architectures (GAN) qui vont dans ce sens.

6. Est-ce que vous pourriez expliquer les détails de cet [article](https://doi.org/10.1101/2021.11.03.467020) sur BioArxiv (preprint)?

> En lisant rapidement :
Préparation des images avec une registration,
ils ont fait une reconnaissance des RNA via une méthode de spot "à la papa" (i.e sans i.a : laplacian of gausian find maxima etc.) et ont gardé leur localisation XYZ pour faire ensuite des analyses des plus proche voisins + threshold pour leur validation (mais cette partie là je ne suis pas très sûr du pourquoi du comment).
Puis petit prétraitement des images DAPI membrane (CD298), epithelial cells (pan-cytokeratin [PanCK]), and T cells (CD3) : ils ont mis au même niveau d'intensité que le DAPI les 3 signaux membranaire pour faire ensuite des soustraction "efficace permettant une amélioration des "bords" des différents marquage puis tout ce bazard dans cellpose (qu'il ont apparemment utilisé comme ça sans "fine tuning il semblerait) pour une segmentation 3D efficace mais sans préciser quel modèle ils ont utilisé (faut bein s'en garder un peu sous le coude)
Et pour finir ROI par ROI analyses des spots fait plus tôt.

7. Question concernant la [video episode 1 video 4](https://www.youtube.com/watch?v=2US1r-cYJSg&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=6): La fonction d'activation Heavyside est remplacée par quelque chose de différentiable mais qui ne ressemble pas du tout. Pourquoi ne pas choisir quelque chose de plus sigmoïdal? Ca serait plus coûteux numériquement sans apporter grand chose sur le résultats?

> C'est la fonction de coût (loss) qui est remplacée par quelque chose de différentiable. Dans le cas de la détection ces fonctions bornent le Heavyside. Donc si on minimise la loss différentiable on minimise aussi le heavyside.
La confusion vient peut-être du fait qu'on a deux fonctions non linéaire dans l'affaire. La fonction d'activation est appliquée après chaque convolution et qui n'a pas à être différentiable et  la fonction de coût (loss) qui mesure l'écart entre la prédiction et la vérité terrain et qui elle doit être différentiable.

8. Est-ce que les valeurs des poids de la couche convolutionnelle `conv2D(32, (3,3))` sont pris au hasard ou bien sont-ils determinées par un algo (type ligne vertical, ligne horizontal,...) ? 

> Les valeurs des poids des kernels et du biais sont initialisés par défaut avec les variables :
[kernel_initializer](https://keras.io/api/layers/convolution_layers/convolution2d/)="glorot_uniform" ou "he_normal". 
Il existe plusieurs fonction d'initialisation disponibles en boutique: https://keras.io/api/layers/initializers/. Ce paramètre est implicite (aléatoire par défaut) mais il est possible de le rajouter dans la définition du modèle (e.g. `Conv2D(32, (3, 3), activation='relu', input_shape=(28, 28, 1), kernel_initializer='random_normal', bias_initializer='zeros')`).

9. Pourquoi Cellpose fonctionne si bien, je n'arrive pas à comprendre dans l'article les images de gradient en X et Y et ce qui rend l'algo si puissant. J'ai vu dans les vidéos de ce matin que NucleAlzer donne des meilleurs résultats encore. Comment utiliser cet algo, l'avez-vous testé ? Si l'image de départ est un peu bruitée, conseillez-vous d'appliquer un filtre median? Est-ce que la normalisation en intensité des images est également importante ? 

> La puissance de Cellpose vient de l'utilisation d'une [base de données d'entraînement très varié et généraliste](https://youtu.be/7y9d4VIKiS8?t=415). Il est précisé que [70,000 cellules ont été utilisée pour l'entraînement.](https://youtu.be/3ydtAhfq6H0?t=84) Cela permet à l'algorithme de converger rapidement. Cellpose n'utilise pas d'a priori de convexité, au contraire de StarDist qui est un modèle de type U-Net avec une couche de post-traitement basé sur un a priori de convexité de cellules.
La base de données d'entraînement de [StarDist](https://www.youtube.com/watch?v=Amn_eHRGX5M) est également importante, pour le modèle dédié à la segmentation aux images fluo a requis 600 images/20,000 annotations, et aux images H&E a requis 30 images/22,000 annotations.
NucleAlzer a été il y a quelques années par T Pécot. Concernant le pré-traitement, en général, tout ce qui peut être compensé sur la base d'a priori physique fort (sûr) doit être fait, possiblement à l'ancienne, avec les outils adaptés (recalage, normalisation, débruitage, homogénéisation spatiale du contraste).

10. Quel méthode puis-je utiliser pour traiter les images RGB (trois canaux de fluo)? Ici je voudrais reconnaitre les cellules en prolifération (marquage nucléaire spécifique : KI67), les LT avec et sans noyaux et les LB avec et sans noyaux. La méthode manuelle consiste à créer des masques annulaires après détection des noyaux KI67 pour rechercher le marquage membranaire des T et B, faire un scatterplot et identifier les T et B par leur intensité. Cette méthode a un biais: la perte de nombreuses cellules à cause d'un marquage annulaire de faible intensité. Est-ce possible de détecter directement les LT et LB en prolifération sur les images RGB (KI67=bleu, LT=vert, LB=rouge) ? 

> Une approche classique consiste à détecter les noyaux dans un premier temps. Si le canal DAPI ou HOECHST est présent, cela permet de détecter tous les noyaux. Dans le cas présent, détecter tous les noyaux sur le canal KI67. Ensuite utiliser une approche comme présentée [ici](https://www.nature.com/articles/s41598-022-08355-1)
[Cellpose 2.0 répond à la question.](https://youtu.be/5qANHWoubZU)

<hr>

# **FAQ pendant les présentations (Skype) <a name="faq-2"></a>**

11. Comment optimiser l'utilisation des GPU?

>

12. Quelle est la quantité de données nécessaire pour le Deep Learning?

> Il faut au minimum quelques centaines d'instances.

13. A quel moment (=combien de temps à galérer) décision de sortir du model driven pour aller vers data driven ?

> L'idée de travailler sur les données est venue très vite, étant donné qu'on n'avait pas trop d'expérience, et que les résultats étaient déjà très satisfaisants

14. Combien de temps pour tester et implémenter jusqu'à résolution du problème ?

> L'implementation, notamment pour le post traitement (combinaison) a bien pris quelques mois. 3- au total on a bien une 30aine d'ovaires adultes (~10Gb /ovaire), d'autres en cours. Une 40aine de larves..d'autres en cours pour d'autres projets

15. Est-ce que le learning rate peut être variable pendant l'apprentissage ?

> Oui, voici deux articles sur le sujet: https://medium.com/analytics-vidhya/learning-rate-decay-and-methods-in-deep-learning-2cee564f910b#:~:text=Learning%20rate%20decay%20is%20a,help%20both%20optimization%20and%20generalization, [Demystifying Learning Rate Policies for
High Accuracy Training of Deep Neural Networks
](https://arxiv.org/pdf/1908.06477.pdf)

16. Question sur la mise en forme: j'ai des images de taille differentes (matrices carrées ou rectangulaires). Je rééchantillone les images pour obtenir une taille 150x150 par exemple. Quelle est l'influence du rééchantillonnage (resizing) sur l'apprentissage?

> Le rééchantillonnage a un impact sur le nombre de paramètres du modèle à entraîner et sur la durée d'entraînement. 

17. Quelle taille de batch faut-il choisir?

> Il est possible de choisir la taille du batch que l'on souhaite. Une recommandation et une habitude de la communauté DL est de choisir une puissance de 2 : 128, 256, 512, 1024...

18. Est-ce que c'est possible après l'entrainement de sélectionner l'epoch avec les meilleurs résultats ?

> oui, on verra ça dans le TP suivant. Ca s'appelle le earlystopping

<hr>
<hr>
