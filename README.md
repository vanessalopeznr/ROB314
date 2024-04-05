# ROB314
Recherche collective avec des drones

Dans chaque dossier, vous trouverez l'espace de travail de chaque ordinateur. Où télécharger le dossier : catkin_ws sur le bureau.

Ce projet fonctionne en python 3.7 et vous devez télécharger les bibliothèques Tellopy, ultralytics, open-cv, rospy et pygame.

La communication entre les ordinateurs se fait à l'aide d'un câble Ethernet et vous devez vous assurer que les deux ordinateurs sont à l'écoute l'un de l'autre. Pour cela, il est utile d'utiliser la commande "ping ip_adr" dans le terminal. Une fois que vous connaissez les adresses IP des deux ordinateurs, vous devez changer les adresses IP de la connexion entre les ordinateurs dans le fichier d'intégration dans catkin_ws/src/tello_driver/nodes.

Pour lancer l'implémentation du projet, il suffit de connecter chaque ordinateur à chaque drone via wifi et d'aller dans le dossier catkin_ws et de lancer les étapes suivantes
