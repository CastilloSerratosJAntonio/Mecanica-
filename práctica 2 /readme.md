# Práctica 2: Velocímetro con 3 sensores infrarrojos

## Objetivo

Desarrollar un sistema capaz de detectar el desplazamiento de una pelota pequeña utilizando sensores infrarrojos y registrar los tiempos correspondientes a su paso por diferentes puntos de la canaleta.

## Materiales

- 1 Arduino
- 3 sensores infrarrojos de barrera
- 3 protoboards
- Cables de conexión
- 1 pelota pequeña
- 1 canaleta
- 1 computadora
- 1 cable USB para conectar el Arduino

## Fundamento

Los sensores infrarrojos de barrera permiten detectar el paso de la pelota mediante una señal digital.

Al colocar los sensores en diferentes puntos de la canaleta, el Arduino puede registrar el momento en que la pelota interrumpe la barrera de cada sensor.

Con los tiempos registrados y las distancias conocidas entre los sensores es posible calcular la velocidad de la pelota.

La fórmula utilizada es:

*Velocidad = Distancia / Tiempo*

## Procedimiento

### 1. Preparación de los materiales

Primero se reunieron los materiales necesarios para realizar la práctica: la placa Arduino, los tres sensores infrarrojos de barrera, las tres protoboards, los cables de conexión, la pelota pequeña y la canaleta.

### 2. Programación de la placa Arduino

Se programó la placa Arduino utilizando el código que se nos proporcionó para realizar la práctica.

El programa permitió recibir las señales digitales provenientes de los sensores infrarrojos y registrar los momentos en que la pelota era detectada.

### 3. Configuración del rango de detección

Se dejó el rango de detección de los sensores en el valor que ya se encontraba predispuesto para la práctica.

Se trabajó con la configuración proporcionada, sin modificar el rango establecido.

### 4. Colocación de la canaleta

Se colocó la canaleta sobre una superficie estable para proporcionar una trayectoria definida para la pelota pequeña.

### 5. Colocación de los sensores

Los sensores infrarrojos fueron colocados en diferentes puntos de la canaleta para detectar el paso de la pelota durante su recorrido.

La separación entre los sensores permitió obtener diferentes puntos de referencia para realizar las mediciones.

### 6. Conexión de los sensores a las protoboards

Los sensores infrarrojos fueron conectados a las protoboards mediante cables.

Posteriormente, las protoboards fueron conectadas a la placa Arduino para proporcionar alimentación eléctrica y permitir la comunicación de las señales de los sensores con el programa.

### 7. Conexiones eléctricas

Para los sensores infrarrojos de barrera con salida digital se utilizaron las siguientes conexiones:

| IR #1 | Arduino | IR #2 | Arduino |
|------|---------|------|---------|
| VCC | 5V | VCC | 5V |
| GND | GND | GND | GND |
| OUT | Pin 2 (interrupción) | OUT | Pin 3 (interrupción) |

Los sensores se conectaron utilizando las entradas digitales correspondientes del Arduino.

*Nota:* La conexión del tercer sensor infrarrojo deberá agregarse de acuerdo con el pin que se utilizó en la práctica.

### 8. Conexión de la placa Arduino

Después de conectar los sensores a las protoboards, se conectaron los cables correspondientes desde la placa Arduino hacia las protoboards.

Se revisaron las conexiones eléctricas para comprobar que los sensores recibieran correctamente la alimentación y que sus señales llegaran a los pines establecidos.

### 9. Prueba de detección

Una vez realizadas las conexiones y cargado el programa, se comprobó que los sensores detectaran correctamente el paso de la pelota.

Se verificó que cada sensor generara la señal correspondiente cuando la pelota interrumpía la barrera infrarroja.

### 10. Realización de las mediciones

Se colocó la pelota pequeña en el inicio de la canaleta y se dejó avanzar.

Al pasar frente al primer sensor, se registró el primer tiempo.

Posteriormente, la pelota pasó frente al segundo sensor y se registró el segundo tiempo.

Finalmente, al pasar frente al tercer sensor, se registró el tercer tiempo.

### 11. Obtención de los tiempos

Con los tiempos registrados por los tres sensores fue posible obtener diferentes intervalos de tiempo:

- Tiempo entre el sensor 1 y el sensor 2.
- Tiempo entre el sensor 2 y el sensor 3.
- Tiempo entre el sensor 1 y el sensor 3.

### 12. Cálculo de la velocidad

Utilizando las distancias establecidas entre los sensores y los tiempos registrados, se calculó la velocidad correspondiente a cada tramo.

Para realizar los cálculos se utilizó:

*Velocidad = Distancia / Tiempo*

### 13. Repetición de las pruebas

Finalmente, se realizaron varias pruebas para comprobar el funcionamiento del sistema y comparar las mediciones obtenidas.
