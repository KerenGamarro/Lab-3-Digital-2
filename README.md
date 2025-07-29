# Lab-3-Digital-2
Electronica Digital 2
Utilizando el microcontrolador ESP32, VS Code y PlatformIO
Este laboratorio consiste en que el estudiante, mediate el uso del entorno
PlatformIO, el framework de Arduino y el microcontrolador ESP32, practique la
configuración de GPIOS, lectura y control de estos, así como implementar
interrupciones y los temporizadores del microcontrolador.
El objetivo de este laboratorio es realizar un “comparador” entre 2 contadores. El
primer contador se trabajará con interrupciones de botones de suma y resta, el
segundo se trabajará con un conteo automático mediante timers. El comparador
al detectar que ambos contadores tengan el mismo valor debe encender una
alarma y reiniciarse. A continuación, se detallará el funcionamiento esperado.
Materiales:
- 1 protoboard
- 1 microcontrolador ESP32
- 2 pushbuttons
- 9 LEDs
- Jumpers
- 9 resistencias de entre 220 Ohms y 1k Ohms
Requeriminetos:
- Los botones deben implementarse con anti-rebote y no deben bloquerse
entre ellos.
- El contador con botones debe implementarse utilizando interrupciones
- El contador automático debe implementarse utilizando timers
- El código debe entregarse debidamente comentado mediante un enlace de
repositorio a GitHub.
- Ambos contadores deben tener comportamiento circular, es decir al llegar
a los valores mínimos o máximos estos deben reiniciarse en vez de
quedarse en el mismo valor.
# Parte A:
Contador con botones (30pts) – Entregable en Clase
Diseñe e implemente un contador binario de 4 bits en el que cada incremento se
hará mediante un botón (B1) y cada decremento mediante otro botón (B2) utilice
interrupciones para los botones.

# Parte B: 
Contador automático (30pts) – Entregable en Clase
Diseñe e implemente un contador binario de 4 bits en el que cada incremento se
realizará cada 250mS, utilizando un temporizador.
# Parte C: 
Comparador y Alarma (25pts)
En el momento que el contador del timer sea igual al contador de los botones,
deberá cambiar el estado de un pin como indicador y reiniciar el contador del timer.
Si el indicador de la alarma ya está encendido y el valor de los contadores vuelve
a coincidir, el indicador debe apagarse. Esto creará que el LED se encienda y
apague de forma “intermitente” y al variar el valor del contador manual el período
de intermitencia de la alarma cambiará respectivamente.
# Parte D: 
Reset (15pts)
Implemente con un sensor capacitvo un botón (B3) el cual reinicie el contador del
timer cada vez que se presione.
Tome en cuenta que todas las partes de este laboratorio deben funcionar
simultáneamente.
