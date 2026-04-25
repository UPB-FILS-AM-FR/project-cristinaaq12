# Système de Scan et Cartographie 2D (Micro-Radar)

| | |
| :--- | :--- |
| `Author` | Radu Cristina-Maria |

## Description
Ce projet consiste en la conception et la réalisation d'un système de balayage électronique pour la détection d'obstacles en temps réel. L'appareil utilise un capteur de distance de haute précision basé sur la technologie laser Time-of-Flight (ToF). Ce capteur est monté sur un servomoteur qui effectue une rotation contrôlée sur un arc de 180 degrés pour scanner l'environnement.

Les données collectées sont traitées par un microcontrôleur ESP32, care calcule les distances et les angles pour transformer ces informations en coordonnées graphiques. Le résultat final est affiché sur un écran OLED sous la forme d'une interface radar dynamique, permettant à l'utilisateur de visualiser la position exacte et la distance des objets environnants.

## Motivation
L'objectif principal de ce projet est d'explorer l'intégration du matériel avec des algorithmes mathématiques simples. La motivation réside dans l'apprentissage de la conversion des données spatiales (coordonnées polaires) en représentations visuelles (coordonnées cartésiennes). Ce projet constitue une base solide pour comprendre les systèmes de navigation et de vision utilisés dans la robotique autonome et les véhicules intelligents.

## Architecture

### Block diagram
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/a0b54612-7d4a-4eb4-b093-8bb3a3345bbe" />

### Components

| Device | Usage | Price |
| :--- | :--- | :--- |
| ESP32 DevKit V1 | Microcontrôleur principal pour le traitement des données | [40 RON](https://www.optimusdigital.ro/ro/placi-esp32/3013-esp32-devkit-v1.html) |
| VL53L0X ToF Sensor | Capteur de distance laser pour une mesure précise | [25 RON](https://www.optimusdigital.ro/ro/senzori-senzori-de-distana/1628-senzor-de-distana-laser-vl53l0x.html) |
| SG90 Servo | Actionneur pour le balayage rotatif motorisé | [15 RON](https://www.optimusdigital.ro/ro/servomotoare/9-servomotor-sg90.html) |
| OLED 0.96" I2C | Écran pour la visualisation graphique de l'interface radar | [25 RON](https://www.optimusdigital.ro/ro/optoelectronica-lcd-uri/1759-display-oled-096-cu-interfaa-i2c-albastru-galben.html) |
| Breadboard/Wires | Support de prototypage et câbles de connexion | [15 RON](https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html) |

### Libraries

| Library | Description | Usage |
| :--- | :--- | :--- |
| Adafruit_VL53L0X | Pilote pour le capteur laser | Lecture de la distance précise |
| ESP32Servo | Bibliothèque pour servomoteurs | Gestion du mouvement de balayage |
| Adafruit_SSD1306 | Bibliothèque graphique OLED | Dessin de l'interface et des obstacles |

## Log

### Week 8 - 14 April

### Week 9 - 21 April

### Week 10 - 28 April

## Reference links
[Introduction to Radar Visualization](https://howtomechatronics.com/projects/arduino-radar-project/)
