Engineering materials
====

This repository contains engineering materials of a self-driven vehicle's model participating in the National WRO El Salvador Future Engineers competition in the season 2025.

## Content

* `t-photos` contains 2 photos of the Robotlan-team (an official one and one funny photo)
* `v-photos` contains 6 photos of the vehicle (from every side, from top and bottom)
* `video` contains the video.md file with the link to a video where driving demonstration exists
* `schemes` contains schematic diagrams in form of JPEG, PNG or PDF of the electromechanical components illustrating all the elements (electronic components and motors) used in the vehicle and how they connect to each other.)
* `src` contains code of control software for all components which were programmed in Arduino IDE to participate in the competition
* `models` is for the files for models used by 3D printers, and laser cutting machines to produce the vehicle elements.
* `other` is for other files which can be used to understand how to prepare the vehicle for the competition. It includes documentation (how to connect to a SBC/SBM and upload files there, datasets, hardware specifications, communication protocols descriptions etc.

## Introduction

Nuestro robot
Nuestro robot, Jonny Carre Bravo, es una creación hecha a partir de distintos competentes diseñados por nosotras para la categoría Future Engineers. 

Herramientas
•	Lenguaje: C++ (Arduino IDE)
•	Librerías: HUSKYLENS, Servo, AFMotor, MPU6050_light, Wire y PID_v1
Gestión de la movilidad
Motores e implementación
Para nuestro robot, utilizamos 2 tipos de motores:
1.	Un motor DC con un diferencial diseñado e impreso en 3D en el tren trasero para ayudar con la propulsión.
2.	Un micro servo SG90 en el tren delantero para controlar la dirección de las ruedas. 
Diseño del chasis 
El chasis está compuesto por piezas diseñadas por nosotras en 3D en Tinkercad con el fin de que nuestro diseño sea simple pero efectivo. Para facilitar las vueltas, se ha tratado de mantener una distancia corta entre ruedas. Esta distancia entre ejes y tamaño del eje facilitan especialmente las vueltas cerradas. La distribución del peso de los motores, baterías y componentes está pensada para que el robot tenga un centro de gravedad bajo, algo que también ayuda a que no se vuelque al girar. Las cuatro ruedas que utilizamos son iguales, grandes y con gomas, para poder agregarle velocidad. Al ser diseñado en 3D, procuramos que el chasis fuera ligero pero firme, para que así no se doble por el peso del resto de componentes. Nuestro diseño también permite que se puedan hacer modificaciones entre las pruebas de manera rápida en caso de que se necesiten revisar o cambiar los componentes y cables. Al mismo tiempo, los cables están ordenados con un código de color para facilitar su identificación.

Gestión de potencia, sentidos y obstáculos 
Los elementos principales para la gestión de potencia y sensores son: 
•	Fuente de energía: 2 sets de baterías, uno para alimentar el controlador de motores y uno para el Arduino.
•	Distribución de energía: una placa reguladora/convertidora de voltaje Elegoo Power MV V2
•	Arduino UNO para el control del vehículo y gestión de sensores
•	Controlador de motores L293D Motor Driver Shield para controlar el servo y motor DC
Sensores
•	2 Sensores ultrasónicos HC-SR04 para la detección de distancia entre las paredes de la pista y el robot, para que así pueda alinearse en el campo de juego.
•	Un giroscopio y acelerómetro MPU6050 para verificar y guiar la orientación del carro y el ángulo de rotación en el eje Z del vehículo para facilitar los giros.
•	Cámara con IA Huskylens para detectar las señales de tránsito y objetos con la función “color tracking”.
