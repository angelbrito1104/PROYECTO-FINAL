# PROYECTO FINAL

## Integrantes 
- Angel Brito
- Sergio Alarcon




## Introduccion 

Este proyecto consiste en un carro robótico que sigue líneas, desarrollado sobre Arduino Uno. Tiene la capacidad de detectar líneas a través de un sensor infrarrojo y controlar el desplazamiento de los motores por medio de un driver L298N. El proyecto, que se incluye en el curso de Sistemas Digitales, tiene como objetivo combinar la automatización, la programación y la electrónica en un sistema embebido.

El carro hace uso de sensores para detectar la línea en el suelo y corregir de manera automática la dirección del movimiento. Asimismo, es posible añadir una interfaz en Streamlit al proyecto para supervisar el sistema y visualizar la información.

## Objetivo General

Crear e implementar un carro robótico con Arduino que siga líneas y controle el movimiento de los motores de manera automática.


## Objetivos Especificos
- Ensamblar el chasis robótico con motores y ruedas.
- Conectar el Arduino Uno con el driver L298N.
- Instalar y configurar el sensor seguidor de línea.
- Programar el movimiento automático del carro.
- Verificar el funcionamiento de detección y seguimiento de línea.


## Materiales

- Arduino Uno
- Driver L298N
- Chasis 
- 4 Motores DC con ruedas
- Sensor infrarrojo seguidor de línea
- Protoboard
- Cables 
- Batería de 9V
- Cable USB
- Tornillos y soportes



## Imagen 1

En la primera imagen se observa el sensor infrarrojo instalado en la parte frontal del carro.



<img width="720" height="1280" alt="92ea4e80-811a-4a27-ab00-79e1fbf12e61" src="https://github.com/user-attachments/assets/773cf803-bc27-4a42-b688-37acb764975b" />



## Explicación

El sensor tiene dos LEDs:

Uno emisor infrarrojo.
Uno receptor.

Su función es detectar diferencias entre superficies claras y oscuras:

La superficie blanca refleja más luz infrarroja.
La línea negra absorbe la luz.

Cuando el sensor detecta la línea negra, envía una señal al Arduino para corregir la dirección del carro.

Resultado esperado

El sensor debe encender su LED indicador cuando detecta una superficie oscura.


## Imagen 2 y 3 

En la segunda y tercera imagen se observa el montaje completo del carro robótico.



<img width="1280" height="720" alt="be950faa-97fa-4f96-86f8-70b27f055125" src="https://github.com/user-attachments/assets/17f2ee89-f256-42a1-94d6-272a02bf7255" />

<img width="720" height="1280" alt="b10b7790-01b5-4674-96db-8331cbed5f93" src="https://github.com/user-attachments/assets/c7a3e373-ccd5-4a40-ac78-a6a9107e3968" />


## Explicación

Se realizó el ensamblaje de:

- Las 4 ruedas.
- Los motores DC.
- El Arduino Uno.
- El driver L298N.
- El sensor frontal.


| Componente        | Función                                   |
| ----------------- | ----------------------------------------- |
| Arduino Uno       | Controla todo el sistema                  |
| Driver L298N      | Controla velocidad y dirección de motores |
| Motores DC        | Permiten el movimiento                    |
| Sensor infrarrojo | Detecta la línea                          |
| Batería           | Alimenta el circuito                      |
