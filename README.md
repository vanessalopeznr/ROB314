# ROB314
## Recherche collective avec des drones

Dans le cadre de ce projet, l’objectif principal est d’assurer la navigation autonome de deux drones vers des points spécifiques de l’espace (chaque drone ayant pour cible un point différent). Cette démarche vise à simuler l’exploration effectuée par les drones dans un environnement donné. Durant leur vol, les deux drones opéreront simultanément une surveillance visuelle à l’aide de leur caméra pour détecter la présence d’êtres humains. Si l’un des drones détecte un humain, il interrompra son vol pour se positionner à l’endroit où la détection a été effectuée, tout en signalant sa découverte à l’autre drone. Ce dernier se dirigera alors vers le point où se trouve l’humain, reproduisant ainsi le processus visant à fournir des ressources telles que de la nourriture, des médicaments, dans des zones difficiles d’accès, ressources qui initialement ne pourraient pas être transportées par un seul drone

Dans chaque dossier, vous trouverez l'espace de travail de chaque ordinateur. Où télécharger le dossier : catkin_ws sur le bureau.

Ce projet fonctionne en python 3.7 et vous devez télécharger les bibliothèques Tellopy, ultralytics, open-cv, rospy et pygame.

La communication entre les ordinateurs se fait à l'aide d'un câble Ethernet et vous devez vous assurer que les deux ordinateurs sont à l'écoute l'un de l'autre. Pour cela, il est utile d'utiliser la commande ```ping ip_adr``` dans le terminal. Une fois que vous connaissez les adresses IP des deux ordinateurs, vous devez changer les adresses IP de la connexion entre les ordinateurs dans le fichier d'intégration dans catkin_ws/src/tello_driver/nodes.

Pour lancer l'implémentation du projet, il suffit de connecter chaque ordinateur à chaque drone via wifi et d'aller dans le dossier catkin_ws et de lancer les étapes suivantes:
```
source devel/setup.bash
catkin_make
roslaunch tello_driver map_detect.launch
```
