# Projet de système de surveillance de température 

## Objectif du projet  
L'objectif du projet est de concevoir un système de surveillance de température en utilisant un capteur LM35, un ESP32, un Raspberry Pi ainsi que le protocole MQTT. Les données seront transmises au Raspberry Pi via Mosquitto, stockées dans une base de données SQLite, et affichées en temps réel grâce à NodeRED. 


### Acquisition et transmission des données 
Pour pouvoir obtenir la température, nous avons utilisé un capteur de température LM35 qui est connecté à la carte ESP32. Pour effectuer les branchements entre ces deux appareils, nous avons utilisé la documentation fournie lors des séances précédentes. 

Le LM35 est donc relié à l'ESP32 grâce à 3 fils. Un reliant la pin "Alimentation" du LM35 à la pin "3.3V" de la carte ESP32, un deuxième reliant la pin OUT à la sortie analogique A5 et un troisième reliant les GND des deux appareils.

![LM35](LM35.png)
![ESP32](ESP32.png)