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



<img width="520" height="600" alt="92ea4e80-811a-4a27-ab00-79e1fbf12e61" src="https://github.com/user-attachments/assets/773cf803-bc27-4a42-b688-37acb764975b" />



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



<img width="500" height="580" alt="be950faa-97fa-4f96-86f8-70b27f055125" src="https://github.com/user-attachments/assets/17f2ee89-f256-42a1-94d6-272a02bf7255" />

<img width="480" height="580" alt="b10b7790-01b5-4674-96db-8331cbed5f93" src="https://github.com/user-attachments/assets/c7a3e373-ccd5-4a40-ac78-a6a9107e3968" />


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



Resultado esperado

El carro debe quedar firme y todos los componentes correctamente ajustados.


## Conexión del sensor

En la imagen 2 se observa el sensor conectado en la parte frontal del vehículo.

Explicación de conexiones

El sensor normalmente tiene:

VCC → 5V Arduino
GND → GND Arduino
OUT → Pin digital del Arduino

El cable naranja y morado observados en la imagen corresponden a señales de alimentación y salida del sensor.



## Imagen 4

El módulo rojo corresponde al driver de motores.

<img width="520" height="580" alt="5a825980-6484-4815-8e49-b397566f2a5f" src="https://github.com/user-attachments/assets/386b8145-5b0b-4c26-b2ec-c7d5ea4322cd" />


## Explicación

El L298N permite controlar:

- Giro hacia adelante.
- Giro hacia atrás.
- Velocidad de los motores.


| L298N   | Arduino     |
| ------- | ----------- |
| IN1     | Pin digital |
| IN2     | Pin digital |
| IN3     | Pin digital |
| IN4     | Pin digital |
| ENA/ENB | PWM         |
| GND     | GND         |
| 12V     | Batería     |


## Resultado esperado

Los motores deben responder correctamente a las señales enviadas por el Arduino.




## Organización del cableado

En la última imagen se observan:

- Los cables del lado izquierdo.
- La conexión de los motores.
- El protoboard.
- La ubicación frontal del sensor.


## Explicación

Se organizaron los cables para:

- Evitar falsos contactos.
- Mejorar la alimentación.
- Facilitar mantenimiento.

El lado marcado en rojo corresponde principalmente al cableado de señales y control, mientras que el lado verde corresponde a conexiones de motores.

## Programación Básica del Carro
Funcionamiento lógico

El programa realiza:

- Lectura del sensor.
- Verificación de línea negra.
- Movimiento automático:
- Adelante.
- Giro izquierda.
- Giro derecha.

## Funcionamiento Esperado
- El carro avanza siguiendo la línea.
- El sensor detecta cambios de color.
- Los motores corrigen la dirección automáticamente.


# Pruebas funcionamiento 

<img width="480" height="460" alt="af397688-b7b4-46b7-a4e5-68a209c30d9e" src="https://github.com/user-attachments/assets/685fef8a-28ab-4e29-befd-fbe9490f5fe1" />
<img width="480" height="460" alt="35eea9e2-2a61-4c11-836b-8a151f72dad4" src="https://github.com/user-attachments/assets/82a64ea1-59b7-45d3-8fe8-780630ef3f1d" />
<img width="480" height="460" alt="ec45df10-e161-422a-b773-e94d0c00012b" src="https://github.com/user-attachments/assets/f85ce2bc-5a14-4e1a-8f74-65671ca3f38c" />
<img width="480" height="460" alt="af4c5fcf-c1f5-4d23-83b0-342eb9260557" src="https://github.com/user-attachments/assets/4775d068-eb2f-4781-9032-ef13259efe83" />

<img width="480" height="460![Uploading 3a96178f-2821-4ff6-8a6f-0b310ffaabff.jpg…]()
" alt="306c63b7-c6ac-4663-997e-dda4c47b1293" src="https://github.com/user-attachments/assets/24d5243c-086c-4eb4-b4b5-1cb41d319058" />

<img width="480" height="460" alt="image" src="https://github.com/user-attachments/assets/4916471b-a5ef-4dc6-84c7-0a69902f6584" />

Las imágenes muestran el funcionamiento de un carro inteligente controlado con Arduino y una interfaz en Streamlit. En las primeras tres imágenes se observa cómo el sistema detecta diferentes colores en tiempo real, mostrando estados como azul, rojo y no reconocido. La interfaz cambia visualmente según el color detectado y muestra la comunicación serial con Arduino. En la última imagen se presenta la estructura física del proyecto, donde se observan componentes como Arduino UNO, el módulo L298N, la protoboard, motores y conexiones eléctricas utilizadas para el funcionamiento del carro.



## Conclusiones
- Se logró construir un carro seguidor de línea funcional basado en Arduino.
- El sensor infrarrojo permitió detectar correctamente superficies negras y blancas.
- El driver L298N controló adecuadamente los motores.
- El proyecto permitió aplicar conocimientos de programación, electrónica y automatización.

