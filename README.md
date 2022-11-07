![Bandeau ANF](https://github.com/bvernay/ANF_Deepscopie/blob/main/img/Bandeau_ANF_Deepscopie.PNG)


# Contexte et enjeu
Les méthodes d’intelligence artificielle et notamment d’apprentissage profond ont bouleversé l’analyse d’images. Aujourd’hui l’apprentissage profond représente la méthode la plus puissante pour la segmentation d’images, la classification de patterns, voire la résolution de certains problèmes inverses. Les algorithmes de deep learning sont largement accessibles via des sites de partages de codes (Github par exemple) mais leur prise  en  main  nécessite  une  initiation  pour  une  utilisation  en  routine  sur  des  plateformes de microscopie ou pour les adapter à de nouvelles techniques de microscopie ou types de données.  Il  est  aussi  important  de  connaitre  les  limites  et  les  écueils  de  ces  techniques. Les  méthodes  d’intelligence  artificielle  ont  aussi  un  fort  potentiel  dans  l’automatisation intelligente   des   acquisitions.   Ces   récents   développements   constituent   des   pistes intéressantes,  mais  pour  lesquelles  une  formation  est  nécessaire  afin  d’en  permettre l’implémentation   efficace   en   microscopie.   Les   constructeurs,   ainsi   que   certaines entreprises  indépendantes,  proposent  des  outils  intégrant  les  codes  de  deep  learning. Pour  comprendre  la  pertinence  de  ces  outils  et  les  limites  de  leur  intégration  il  est nécessaire de disposer d’un bagage suffisant dans le domaine. 

# Public  visé
Cette  action  nationale  de  formation  du  CNRS  s’adresse  aux  ingénieurs  de plateformes de microscopies et aux biologistes amenés à analyser des images ou interagir avec des traiteurs d’images. 

# Prérequis
Posséder des bases d’analyse d’images classique. La pratique d’un langage de programmation (quel qu’il soit) est conseillée mais pas indispensable

**Modalités  de  l’épisode  1**  Enseignement  de  cours,  discussions,  travaux  pratiques  en ligne selon le planning ci-dessous. 

# Objectifs
A l'issue  de  la  formation  vous  aurez  les  connaissances  de  base  pour comprendre  le  fonctionnement  des  réseaux  de  neurones  profonds  et  serez  à  même  de démarrer vos propres projets d’analyse d’image par ces méthodes. Un accompagnement sera  proposé  dans  l’épisode  2  (en  présentiel)  de  cette ANF  pour  un  niveau  avancé.  Une comparaison (en présentiel) des outils commerciaux sera enfin réalisée dans l’épisode 3.

# Programme

<table>
<thead>
  <tr>
    <th></th>
    <th>Lundi 13 juin</th>
    <th>Mardi 14 juin</th>
    <th>Mercredi 15 juin</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td><b> 9h - 10h30 </b></td>
    <td><b> [Matin ou en cours asynchrone en ligne : Principes](#jour-1-les-principes-du-deep-learning) </b></td>
    <td><b> [Matin ou en cours asynchrone en ligne : Annotation d’images](#jour-2-annotations-dimages) </b></td>
    <td><b> [Matin ou en cours asynchrone en ligne : “Kind of Easy” deep learning](#jour-3-kind-of-easy-deep) </b></td>
   </tr>
  <tr>
    <td><b>10h30 - 12h </b></td>
    <td><b> Discussion en ligne en présence de biologistes ayant récemment utilisé avec succès les méthodes de deep learning pour leurs propres questions. </b></td>
    <td><b> Discussion en ligne en présence d’acteurs public et privé de l’annotation de donnée. </b></td>
    <td><b> Discussion en ligne en présence d’ingénieurs de plateformes de microscopies qui utilisent des outils de deep learning au quotidien. </b></td>
  </tr>
  <tr>
    <td><b> 13h - 17h </b></td>
    <td><b> TP en ligne : Mon premier TP les mains dans le moteurs 1/3 • CNN par la pratique avec MNIST puis adaptation de MNIST vers un exemple de classification en microscopie </b></td>
    <td><b> TP en ligne : Mon premier TP les mains dans le moteurs 2/3 • Transfer learning on CNN example • Data augmentation on CNN example • Optimize code with early stopping </b></td>
    <td><b> TP en ligne : Mon premier TP les mains dans le moteurs 3/3 • Segmentation d’images avec UNet via ZeroCostDL4Mic. • Bilan de la formation sur le choix des outils </b></td>
  </tr>
</tbody>
</table>

---
# Pré-requis pour la formation

## Outils à installer
* Télécharger et installer iLastik que vous trouverez [ici](https://www.ilastik.org/).
* Créer un compte Google spécifique pour l’utilisation de Collaboratory. Certains workflow que nous allons utiliser nécessitent d’utiliser les ressources en-ligne mises à disposition par Google. En amont de la formation, il vous est demandé de créer un compte spécifique via [ce lien](https://accounts.google.com/signup/v2/webcreateaccount?flowName=GlifWebSignIn&flowEntry=SignUp). A vrai dire, les ressources de calcul disponibles pouvant être limitées par Google, il pourra être utile de créer plusieurs comptes dédiés.

## e-learning: cours asynchrones en ligne

* [Regarder la vidéo : How to get started with Jupyter and Colab.](https://www.youtube.com/watch?v=OH3VKI7ErAE&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=9)

#### Jour 1: les principes du deep learning
* [Shift from model driven to data driven (25:50)](https://youtu.be/264ZrAb_7PA)
* [Introduction to ML and DL : Partie 1 (15:57)](https://www.youtube.com/watch?v=RzN5RVSwrRw)
* [Introduction to ML and DL : Partie 2 (17:12)](https://www.youtube.com/watch?v=C8pPx-AbRHI&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=2)
* [Introduction to ML and DL : Partie 3 (23:02)](https://www.youtube.com/watch?v=Rb-4Yu-qLR4&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=3)
* [Introduction to ML and DL : Partie 4 (16:11)](https://www.youtube.com/watch?v=2US1r-cYJSg&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=4)
* [CNN principles (20:16)](https://www.youtube.com/watch?v=muY5FAn04FI&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=6)
* [Basic architecture in deep learning (29:26)](https://www.youtube.com/watch?v=a8XvknLW-Dg&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=7)
* [PlaygroundTensorFlow demo (15:36)](https://www.youtube.com/watch?v=zAN3xUBiaPI&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=5)

#### Jour 2: annotations d'images
* [Data augmentation : Partie 1 (14:01)](https://www.youtube.com/watch?v=jjVao6YDDIA&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=16)
* [Data augmentation : Partie 2 (13:30)](https://www.youtube.com/watch?v=N0K0kPehqKg&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=17)
* [Data augmentation : Partie 3 (9:21)](https://www.youtube.com/watch?v=wWk48qkgjB8&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=18)
* [Data augmentation : Partie 4 (11:45)](https://www.youtube.com/watch?v=NvV94Fv8pL4&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=19)
* [Speeding up image annotation (11:59)](https://www.youtube.com/watch?v=TSx4xV--b2A&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=20)
* [Introduction to Ilastik : sur la playlist Easy annotation with ilastik (16:05)](https://www.youtube.com/watch?v=NTdDB6baZ_8&list=PLUukCwr0iCef9M7WUOx9_bJYJpvMxek6F&index=20)

#### Jour 3: “Kind of Easy” deep
* [DeepImageJ: sur la playlist (10:07)](https://www.youtube.com/watch?v=eIqQandVtEU&t=63s)
* [ZeroCostDL4mic (1:33:36)](https://www.youtube.com/watch?v=dcgU5WKE70I)
* [EGI Service (39:48)](https://www.youtube.com/watch?v=tAjTGtijt5A&t=10s)

# Atelier Jour 1
Discussion en ligne en présence de biologistes ayant récemment utilisé avec succès les méthodes de deep learning pour leurs propres questions.
 * [Introduction du Jour 1 (03:01)](https://seafile.unistra.fr/f/dcc022d7957344a5b506/)
 * [Discussion (01:05)](https://seafile.unistra.fr/f/c9b0a70094154e3c9cbe/)
 * [Questions & Réponses E-learning "Les principes du Deep Learning" (33:50)](https://seafile.unistra.fr/f/0e11e49d007b476495ce/)
 * [Success Story: Manon Lesage (14:25)](https://seafile.unistra.fr/f/bf95abcaeeef46be8903/)
 * [Success Story: Héloïse Monnet (07:41)](https://seafile.unistra.fr/f/49dc2fe9aed04289a53f/)
 * [Success Story: Quentin Giraud (07:06)](https://seafile.unistra.fr/f/5acbf054fbe74cb091ac/)
 * [Success Story: Herve Alegot (12:40)](https://seafile.unistra.fr/f/b3774bccfcdc432e95d6/)
 * [Conclusion (03:30)](https://seafile.unistra.fr/f/660270e29efb4ffdb209/)

* TP en ligne : 
  * Mon premier TP les mains dans le moteurs 1/3 
  * Regarder la vidéo : How to get started with Jupyter and Colab.
  * CNN par la pratique avec MNIST puis adaptation de MNIST vers un exemple de classification en microscopie
 * [Tensorflow Playground (24:01)](https://seafile.unistra.fr/f/b27d32b58c2a48998e11/)
 * [Mon premier réseau: NMIST première partie (48:27)](https://seafile.unistra.fr/f/33c8dce141bb48859543/)
 * [Mon premier réseau: NMIST seconde partie  (01:36:19)](https://seafile.unistra.fr/f/648f114e590147a1ad2a/)

Discussion en ligne jour 1
* [Jour 1 Chat](https://gitlab.com/igbmc/mic-photon/anf_deepscopie/-/raw/main/workshop_chat/chat_ANF_Deepscopie_edited.txt)

# Atelier Jour 2
Discussion en ligne en présence d’acteurs public et privé de l’annotation de donnée.
 * [Dessine moi un réseau (23:01)](https://seafile.unistra.fr/f/5e79342a97974555bc88/)
 * [ilastik (15:50)](https://seafile.unistra.fr/f/a68365dd14694bb8a4f8/)
 * [Cytomine (16:12)](https://seafile.unistra.fr/f/62b419451a05404d90f3/)
 * [Creatis (20:14)](https://seafile.unistra.fr/f/05b2bf2a31f1480bb2a1/)
 * [Conclusion (04:59)](https://seafile.unistra.fr/f/6c65767fde7944f79193/)

* TP en ligne : 
  * Mon premier TP les mains dans le moteurs 2/3 
  * Transfer learning on CNN example 
  * Data augmentation on CNN example 
  * Optimize code with early stopping
* [Discussion(23:32)](https://seafile.unistra.fr/f/5ae4a53e21f14963a549/)
* [CNN (01:56:09)](https://seafile.unistra.fr/f/71e95cecc2114874b663/)
* [Réglage des hyperparamètres (01:30:09)](https://seafile.unistra.fr/f/d70a5972438e4a1386cb/)

Discussion en ligne jour 2
* [Jour 2 Chat](https://gitlab.com/igbmc/mic-photon/anf_deepscopie/-/raw/main/workshop_chat/chat_ANF_Deepscopie_edited.txt)

# Atelier Jour 3
* Discussion en ligne en présence d’ingénieurs de plateformes de microscopies qui utilisent des outils de deep learning au quotidien.
 * [A AJOUTER (00:00)](https://www.youtube.com/)

* TP en ligne : 
  * Mon premier TP les mains dans le moteurs 3/3 
  * Segmentation d’images avec UNet via ZeroCostDL4Mic. 
  * Bilan de la formation sur le choix des outils
 * [A AJOUTER (00:00)](https://www.youtube.com/)

Discussion en ligne
* [Jour 3 Chat](https://gitlab.com/igbmc/mic-photon/anf_deepscopie/-/raw/main/workshop_chat/)

Wiki et FAQ
* [Tout savoir sur le DL](https://gitlab.com/igbmc/mic-photon/anf_deepscopie/-/blob/main/workshop_chat/chat_ANF_deepscopie_keepcontent_ongoing.md)

# Formateurs
Adnane Aitoussaye, Université d’Angers  
Anaïs Badoual, INRIA Rennes  
Marine Breuilly, Université Claude Bernard Lyon1  
Nima Hatami, CREATIS, Lyon  
Valentin Gilet, Université d’Angers  
Felicia Marianne INRAe Toulouse  
Félix Mercier, Université d’Angers  
Herearii Metuarea, Université d’Angers  
Juliette Moreau, CREATIS, Lyon  
Guillaume Mougeot, UCA Clermont-Ferrand  
Thierry Pecot, Université Rennes 1  
Sylvain Prigent, INRIA Rennes  
Pejman Rasti, Université d’Angers  
David Rousseau, Université d'Angers  
Daniel Sage, EPFL Lausanne  
Hervé Turlier, Collège de France  
Bertrand Vernay, INSERM 
