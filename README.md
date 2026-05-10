# Système de Scan et Modélisation 3D d'Objets

| | |
| :--- | :--- |
| `Author` | Radu Cristina-Maria |

## Description
Ce projet consiste à réaliser un système de capture 3D pour modéliser des objets. Pour augmenter la complexité du système, le montage utilise 3 capteurs de distance laser (ToF) positionnés sous différents angles pour scanner l'objet ciblé. Le microcontrôleur collecte les données spatiales (distances et angles) et les transmet à un PC. Le PC se charge ensuite de traiter ces informations pour générer et afficher une capture 3D de l'objet. Ce projet explore la cartographie spatiale avancée, même à l'état de prototype expérimental.

## Motivation
L'objectif principal de ce projet est d'explorer l'intégration du matériel multi-capteurs avec des algorithmes de reconstruction spatiale. La motivation réside dans l'apprentissage de la collecte de données, la gestion du bus I2C pour plusieurs capteurs identiques, et la transmission vers un environnement logiciel sur PC pour le rendu 3D. Ce projet constitue une base solide pour comprendre les principes de la numérisation 3D et de la vision par ordinateur.

## Architecture

### Block diagram
<img width="937" height="507" alt="image" src="https://github.com/user-attachments/assets/282c69c2-6a87-49c8-ad3f-6775b975964d" />


### Components

| Device | Usage | Price |
| :--- | :--- | :--- |
| ESP32 DevKit V1 | Microcontrôleur principal pour le traitement des données | [40 RON](https://www.optimusdigital.ro/ro/placi-esp32/3013-esp32-devkit-v1.html) |
| 3x VL53L0X ToF Sensor | Capteurs de distance laser pour la capture 3D sous plusieurs angles | [3x 25 RON](https://www.optimusdigital.ro/ro/senzori-senzori-de-distana/1628-senzor-de-distana-laser-vl53l0x.html) |
| SG90 Servo | Actionneur pour faire pivoter l'objet (plateau tournant) | [15 RON](https://www.optimusdigital.ro/ro/servomotoare/9-servomotor-sg90.html) |
| Résistances (10kΩ) | Pour configurer les adresses I2C multiples des capteurs | ~5 RON |
| Breadboard/Wires | Support de prototypage et câbles de connexion | [15 RON](https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html) |

### Libraries / Software

| Library / Tool | Description | Usage |
| :--- | :--- | :--- |
| Adafruit_VL53L0X | Pilote pour les capteurs laser | Lecture des distances précises |
| ESP32Servo | Bibliothèque pour servomoteurs | Gestion de la rotation de l'objet |
| Python / Processing (PC) | Logiciel sur PC | Réception des données série et rendu 3D |

## Log

### Week 8 - 14 April

### Week 9 - 21 April

### Week 10 - 28 April

## Reference links
[Introduction to 3D Scanning concepts](https://howtomechatronics.com/projects/arduino-radar-project/)
