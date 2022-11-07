david.rousseau
  18 h 49
Une captation des répétitions des TP 1 et 2 pour ceux d'entre-vous qui souhaitent réviser.
Video-20220608_154610-Meeting Recording.mp4
 
18 h 50
Pour rappel pour le TP 3 : La vidéo est ici avec le code dans le commentaire. https://www.youtube.com/watch?v=wOmJnn3NrvE&t=419s
YouTubeYouTube | ImHorPhen Bio imaging research group
UNET demo 

18 h 52
Bonsoir à tous. Après la répétition, nous arrivons à l'idée qu'il faut démarrer tous ensemble pour la partie connection sur Colab et 1er réseau de neurone. On se séparera sans doute à la pause de 15H le premier jour.
:+1:
4



Anaïs Badoual
  17 h 36
Bonjour à tous,
Dans le TP1 je n’arrive pas à me connecter à TensorFlow visualization Toolkit. Ïnitialization failed”. Est ce que d’autres ont le même pb ?
Anaïs Badoual
  il y a 4 mois
Ok en fait lors de l’inscription ngrok envoie ensuite un mail pour vérifier l’adresse mail. Maintenant que j’ai cliqué sur leur lien de validation du mail cela fonctionne. J’ai reçu ce mail de validation plusieurs heures après l’inscription. Est ce que les étudiants auront créé leur compte ngrok en amont du cours ou bien ils doivent le faire en live, auquel cas ils risquent d’avoir le même pb que moi.





Félix Mercier
  il y a 4 mois
Bonjour Anaïs,
As tu réussi à faire fonctionner les tensorboards sur l'ensemble des code finalement ? Sinon, il y a une solution alternative pour afficher les courbes directement sur le Colab (la cellule après celle de l'entraînement permet de les afficher).
Pour ce qui est du compte ngrok, nous n'avions pas eu à attendre longtemps le mail de validation mais on peut leur envoyer ce lien : https://ngrok.com et leur demander de créer un compte avec l'adresse gmail qu'ils utiliseront pour colab. (modifié) 
ngrok.com
ngrok - Online in One Line
ngrok is the fastest way to put anything on the internet with a single command.

Anaïs Badoual
  17 h 38
A ce sujet, les versions des jupyter notebooks diffèrent entre celle que tu nous as envoyée par mail David et celle qui est dans le dossier FC_2021 donnée aux étudiants. Par exemple dans cette partie TensorFlow’s visualization toolkit. (Je pense que vous attendiez les retours pour mettre à jour les fichiers dans FC_2021 mais au cas où…) (modifié) 


Juliette Moreau
  8 h 51
Il y a certains documents dans le canal #deep-learning (modifié) 

david.rousseau
  12 h 39
Le niveau est assez haut : des points pratiques soulevés ce matin dans le chat comme le conseil pour l'achat d'un GPU. Bien si on peut ajouter des éléments dans le channel bibliographie à ce sujet.

Félix Mercier
  12 h 48
David, où se trouve les données pour le CNN afin de montrer comment faire la mise en place sur le drive ?
felix, as tu trouvé les données?  les data etaient dans le repertoire compressé: https://drive.google.com/file/d/1Nw5IdFe6Rk6UG8how_Ff_KGW67QxHwR4/view?usp=sharing


@Anaïs Badoual
... get ready pour la connection à 13H sur le démarrage des TP. On va démarrer à deux avec Félix pour synchroniser tout ensemble le démarrage de la connection Colab et la réalisation du premier réseau de neurone.

vernayb
  13 h 41
pas de possibilités d'accéder individuellement à chaque fichier du drive en lecture seule.? J'ai l'impression que l'on m a pas le choix que de tout télécharger


david.rousseau
  13 h 57
Oui pas très pratique ... :perplexe: mais volume reste raisonnable quand même


vernayb
  16 h 15
pour le CNN ils restent en CPU ou passent en GPU? ou d'abord CPU pûis redemarre en GPU?
16 h 16
70 secondes par epoch CPU, 7secondes en GPU à l'instant


david.rousseau
  16 h 20
Oui. Bien si on fait ce test à cet entroit.... Merci pour tes feedbacks Bertrand !!!


david.rousseau
  7 h 21
For today an additional hands on https://drive.google.com/drive/folders/1E8BYoYKCDLH56e0tkd_72ALdNzfA8cDc?usp=sharing with automatic adjustment of the hyperparameters

vernayb
  8 h 20
Question pratique sur la procédure pour le fichier zip: 1- importer le zip sur le drive et dézipper dans le drive avec ZipExtractor? ou 2-  le dézippage est codé dans le notebook?


Juliette Moreau
  8 h 27
Pour les TP CNN le dézipage est codé dans le notebook

david.rousseau
  9 h 10
Je suis assez d'accord avec Bertrand. Pour aujourd'hui 
@Valentin Gilet
 peut prendre le lead. Demain si ok pour 
@Anaïs Badoual
 ou 
@Guillaume Mougeot
 la demo pourrait être faite en s'appuyant sur zerocostDL4 mic ? Sinon chez nous 
@Juliette Moreau
 ou 
@Herearii Metuarea
 peuvent assurer.


vernayb
  9 h 23
Un retour d'expérience personnelle avec des TPs Colab et la gestion des données sur le Drive. Vraiment dérouler pas à pas la partie connexion au Drive, comment utiliser la fenêtre d'arborescence à gauche et peut être suggérer une organisation identique à tout le monde des dossiers?
:+1:
1



vernayb
  11 h 27
Il nous faudrait un serveur Cytomine pour ANF Deepscopie et le GT MAIIA RTmfm

david.rousseau
  11 h 27
On va contacter Montpellier pour utiliser https://biaflows-sandbox.neubias.org/#/


Anaïs Badoual
  11 h 57
Pour cet après midi lors des TPs est ce qu’on commence par le TP 2 qu’on n’a pas eu le temps de faire hier ? Ou on commence directement par le TP1 du jour  2?


david.rousseau
  12 h 01
On va commencer par finir le TP d'hier. On propose de continuer en mode salle commune pour aujourd'hui avec 
@Valentin Gilet
 à la manette. Est-ce que 
@Anaïs Badoual
 tu serais ok pour faire la démo U-Net demain à partir de zerocostDL4Mic ?


Anaïs Badoual
 14 juin à 12 h 08
Pas de soucis. Par contre je suis juste un peu perdue sur le jupyter notebook de demain. Est ce que c’est le Unet_based_Apple_segmentation.ipynb ou le Unet_segmentation_notebook.ipynb ?
Anaïs Badoual
  il y a 4 mois
Ou est ce que tu pensais faire un autre jupyter notebook (que je prends sur zerocost) en plus de ces 2 là ?


Anaïs Badoual
  il y a 4 mois
je peux faire le zeroCost 2D Unet Sur les HellaCells que j’avais fait à Mifobio si tu veux
:fléchette:
1



david.rousseau
  il y a 4 mois
Oui c'est parfait. L'idée est de montrer l'utilisation des outils "easy". Est-ce que tu penses pouvoir faire aussi une démo DeepImageJ ? (pas forcément indispensable puisque nous avons donné une vidéo le matin) Peut être juste bien mentionner /différencier DeepImageJ et Zerocost.


Anaïs Badoual
  il y a 4 mois
Ca marche :clin_d'œil:. Je fais tous ça en mode démo (moi seule) ou en mode TP ?


david.rousseau
  il y a 4 mois
En mode comme on a fait sur les deux premiers jours... je ne sais pas trop comment l'appeler.


Anaïs Badoual
  il y a 4 mois
ok donc en mode TP avec les participants qui le font en même temps.
Par contre on va avoir le temps ? Entre les Tps d’aujourd’hui à finir, les 2 TPs déjà prévu demain, DeepImageJ et ZeroCost ça me semble beaucoup en 3h


david.rousseau
  il y a 4 mois
On a les vidéos pour finir les TP d'aujourd'hui. Demain Zerocost quoi qu'il en cost :clin_d'œil: (modifié) 


Anaïs Badoual
  il y a 4 mois
Ca marche :clin_d'œil: du coup je t’envoie le matériel ce soir. Est ce que vous avez déjà demandé aux participants d’installer DeepImageJ ? Ça peut prendre du temps


david.rousseau
  il y a 4 mois
Non on n'a pas demandé. Est-ce qu'on reste sur Zerocost seulement ?


Anaïs Badoual
  il y a 4 mois
Ba honnêtement je pense que c’est plus safe si on veut avoir le temps de bien le faire. Sinon j’ai peur qu’on passe beaucoup de temps sur des soucis d’installation. Mais j’essaierai de bien expliquer la différence entre DeepImageJ et ZeroCost


david.rousseau
  il y a 4 mois
Ok on reste sur Zerocost uniquement. Merci 
@Anaïs Badoual
... on s'adapte au groupe.
:+1:
1



david.rousseau
  il y a 4 mois
@Anaïs Badoual
 pourras tu à nouveau illustrer le data augmentation demain avec Zerocost ?


Anaïs Badoual
  il y a 4 mois
Yes. Il me semble qu’il y a une partie data augmentation dans le notebook zerocost


david.rousseau
  il y a 4 mois
Merci. Parfait. Car on est un peu juste pour cette fin de journée.


david.rousseau
  12 h 44
@Pejman Rasti
 will you be able to take over 
@Valentin Gilet
 for the https://drive.google.com/drive/folders/1E8BYoYKCDLH56e0tkd_72ALdNzfA8cDc?usp=sharing


Pejman Rasti
  13 h 02
Sure,


Pejman Rasti
  13 h 41
Pendant que vous travaillez sur le premier code, veuillez télécharger ces données dans votre google drive pour l’exercice suivant.
Zip
 

data_colon_binary.zip
Zip


vernayb
  15 h 55
le keras_tuner c'est l'autoML de google?


david.rousseau
  15 h 56
kind of... ajustement des hyperparamères automatique dans des ranges.



david.rousseau
  12 h 10
@Pejman Rasti
 would you be available to finish the transfer learning exercice of yesterday ? (modifié) 


david.rousseau
  12 h 47
@Félix Mercier
 est-ce que tu veux/peux reprendre la fin de l'exercice data augmentation ?


Félix Mercier
  12 h 58
Je peux mais je n'ai pas une idée précise de ce qui restait à faire. On reprend le notebook 3_Transfert_learning_with_Data_Augmentation au début ? Il faudra tout exécuter pour arriver à la fin.


Marine BREUILLY
  15 h 32
Bonjour à tous, je ne sais pas si quelqu'un consulte entre le slack... au cas où je poste le message ici:
15 h 35
je me permets de vous contacter car j ai remarqué que le slack ne garde l'historique des messages que pendant 90j (en compte gratuit).
A priori il y a une parade - en tant qu'admin - il serait possible de sauvegarder / exporter les messages.
Je ne sais pas si vous l'avez déjà fait mais j'ai trouvé ce lien qui explique comment faire: https://www.businessinsider.com/how-to-export-slack-conversation?r=US&IR=T.
Ca pourrait être pas mal de garder une trace notamment des canaux bibliographie, deep-learning et episode-2-wishliste, afin de pouvoir les renvoyer aux participants, sinon on va perdre la trace.
Qu'en pensez-vous?

Business InsiderBusiness Insider
How to export a Slack conversation in 2 different ways
There are two ways to export a Slack conversation, depending on whether you have a standard or Plus plan. (71 ko)
https://www.businessinsider.com/how-to-export-slack-conversation?r=US&IR=T



vernayb
  15 h 36
je suis d'accord. j'avais essayé mais n'étant pas admin cela n'était pas possible et puis j'ai oublié ...
15 h 37
même problème avec la discussion sur Skype. J'ai un export en xml pas très pratique pour extraire les infos
