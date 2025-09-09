Proyecto: Control de LEDs con menú y pulsador en Arduino

Este programa permite controlar tres LEDs (rojo, amarillo y verde) conectados a un Arduino mediante:

Un pulsador (botón en el pin 13).

Cada vez que se presiona, incrementa un contador.

Si pasa 1 segundo sin nuevas pulsaciones, el programa ejecuta la acción correspondiente al número de pulsos.

Un menú interactivo en el monitor serie.

Se puede escribir un número del 0 al 9 en el monitor serie para seleccionar una acción.

⚙️ Funcionalidades del programa

LED rojo

[1] Encender

[2] Apagar

[0] Interruptor (toggle):

Si está apagado, se enciende.

Si está encendido, se apaga.

Si está en intermitencia, se apaga y se detiene el parpadeo.

LED amarillo

[3] Encender

[4] Apagar

LED verde

[5] Encender

[6] Apagar

Acciones globales

[7] Encender los tres LEDs

[8] Apagar los tres LEDs

[9] Poner los tres LEDs en intermitencia

🕹️ Detalles técnicos

Usa millis() en lugar de delay() para manejar la intermitencia, permitiendo que el programa siga respondiendo mientras los LEDs parpadean.

Incluye un sistema de antirrebote básico para el pulsador.

Permite dos formas de control:

Pulsador físico (con temporizador de 1 segundo).

Menú desde el monitor serie de Arduino.

👉 En resumen, este código es un menú de control de LEDs que combina entrada por hardware (pulsador) y software (monitor serie), con opciones de encendido, apagado, intermitencia y un interruptor (toggle) especial para el LED rojo.
