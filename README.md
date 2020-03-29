# Verrerie
 Augmented Reality Project
 
 Elèves: Simon RE et Anaïs THORAL

Problématique  : 
Une société de vente de verres et de carafes pour restaurant 5 étoiles veut utiliser la réalité augmentée pour faire essayer les modèles de ses catalogues aux restaurateurs. Le problème étant que l’envoi de la verrerie aux restaurants est très coûteux car ce sont des colis volumineux et fragiles. Mais d’un autre côté, dans les magazines, le rapport de taille d’un modèle à l’autre n’est pas évident, il fallait donc trouver une solution. 

Approche généraliste :
La solution 
Aujourd’hui nous avons trouvé une solution innovante. Nous proposerons au restaurateur de recevoir ou d’imprimer des images cartonnées (le nombre d’images dépendra du nombre de verres dans la collection). Il pourra alors déposer les images où il le souhaite sur ses tables et, à travers son écran de téléphone ou de tablette, il pourra voir apparaître les verres associés.
Ainsi en quelques minutes le restaurateur pourra choisir la collection qu’il souhaite afficher, positionner ses cartons et ainsi profiter du confort de pouvoir changer la décoration de ses tables comme bon lui semble !
L’avantage de cette solution est aussi qu’on ne risque plus d’endommager les verres vitrines lors du voyage et que nous n’avons plus de temps de livraison à perdre. Le professionnel pourra tester en un instant les collections et ainsi choisir celle qui lui correspond.
UX
L’utilisateur pourra afficher la verrerie qu’il souhaite depuis l’interface proposée, via une liste d’aperçus des collections. De manière intuitive il dirigera la caméra vers les marqueurs (images cartonnées). Le restaurateur verra alors s’afficher instantanément les produits.

Force du projet
L’utilisation de la réalité augmentée crée l’aspect instantané et “réel” de l’expérience. Le client peut essayer la collection qu’il veut, quand il le veut. Plusieurs personnes peuvent utiliser l’application en même temps ce qui permet aux membres de l’équipe du restaurateur de contribuer à la mise en place d’un nouveau service de vaisselle. 

Description technique
Nous allons utiliser le moteur Unity, qui va nous permettre de créer des applications pour Windows (UWP, Universal Windows Platform), Android et iOS.
Le package Vuforia pour Unity va être implémenté, et il nous permettra de gérer assez facilement l’utilisation de la réalité augmentée.
On va pouvoir stocker, dans une base de données Vuforia, des images qui correspondront à nos marqueurs, avant de les importer directement dans Unity.
Ces images devront contenir de nombreux détails géométriques, afin d’optimiser leur reconnaissance, et elles devront être très différentes les unes des autres, afin que les algorithmes de reconnaissance ne les confondent pas.
Ensuite, sur Unity, nous allons permettre à l’utilisateur de choisir la collection de verres qui l’intéresse via un slider qui en montrera un aperçu. Dans l’éditeur d’Unity on va ensuite pouvoir lier les modèles 3D des verres de la collection sélectionnée aux marqueurs correspondants.
Ainsi, lorsque les algorithmes de Vuforia vont capter la présence de ces images via la caméra de l’appareil, ils vont pouvoir les tracker (les suivre dans l’espace et calculer leur position et rotation) et afficher les modèles correspondants de façon réaliste.

