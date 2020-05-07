<h1 align="center">Introduction to mobile ROBOTICS & Internet of things 👋</h1> 



# ✨ Detection and tracking of a moving person



## ✨ Pour exécuter le projet : 

Nous utilisons CMake comme notre système de construction, et il doit être utilisé même pour les nodesPythons. En effet il est nécessaire de générer le code Python pour les messages et les services. Pour cela ilfaut aller dans le workspace catkin et lancer la commande catkin_make :

```sh
cd ~/catkin_ws
catkin_make
```



Pour pouvoir localiser et interagir entre les nodes il faut un annuaire. C’est le rôle de roscore. Il doit être lancé systématiquement mais une seule fois : 


```sh
roscore
```

Aprés on passera à la lecture des données sauvergardées qui ce fait par la commande : 

```sh
Rosbag play data_file.bag
exemple : rosbag play Data/2018-01-24-17-44-23.bag
```


Lancer les deux programmes : 

```sh
rosrun follow_me moving_person_detector_node
rosrun follow_me robot_moving_node
```

Finalement on lance l'outil de visualisation de ROS : 


```sh
rviz
```

