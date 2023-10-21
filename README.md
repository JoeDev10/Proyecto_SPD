Integrantes:
-Ivan Rammunda
-Fernando Torres
-Joel Rodriguez

![proyecto_spd_final](https://github.com/JoeDev10/Proyecto_SPD/assets/118489703/33771a4b-6250-4f6f-bb1a-e429ce1ff2bb)

DESCRIPCION:

Este proyecto utiliza LEDs, botones y pantallas LED para crear un sistema interactivo que permite a los usuarios gestionar un contador numérico. Sus características clave incluyen:

Contador Numérico: Controla y muestra valores en dos pantallas LED, una para las unidades y otra para las decenas.

Botones de Control: Tres botones permiten aumentar, disminuir y restablecer el contador.

Visualización Clara: Los LEDs representan los dígitos de forma clara y fácil de entender.

Configuración Personalizada: La duración de visualización en las pantallas LED es configurable.

FUNCIONES:
-> setup(): Esta función se llama una vez al inicio del programa. Aquí se configuran los pines de entrada y salida para los botones, LEDs y pantallas. También se inicia la comunicación serial a una velocidad de 9600 baudios.

-> loop(): Esta función se ejecuta continuamente en un bucle. Controla la lógica principal del programa. Lee los botones, actualiza el contador y llama a printContador() para mostrar el valor en las pantallas.

-> printDigit(int digit): Esta función toma un dígito como entrada y enciende los segmentos de un display de siete segmentos para mostrar ese dígito en el LED correspondiente.

-> prendePantalla(int digito): Enciende una de las dos pantallas (unidad o decena) y apaga la otra según el valor de digito. Esto permite alternar entre las dos pantallas para mostrar números de dos dígitos.

-> printContador(int contador): Muestra el valor del contador en las pantallas. Divide el contador en sus dígitos decena y unidad y llama a printDigit() para mostrar cada dígito en la pantalla correspondiente.

-> botonPresionado(): Esta función detecta si se ha presionado alguno de los tres botones (SUMA, RESTA, RESET) y devuelve un valor correspondiente para identificar cuál de los botones se presionó. También gestiona el estado previo de los botones para evitar lecturas repetidas cuando se mantienen presionados.

MULTIPLEXACION:
la implementación de la multiplexación en este código se logra alternando rápidamente entre dos pantallas de un display de siete segmentos (unidad y decena) utilizando dos pines de control (UNIDAD y DECENA). Esto permite mostrar números de dos dígitos en la pantalla con solo dos pines de control en lugar de requerir un pin para cada segmento del display.

Se agrego al proyecto un tercer display para mostrar numeros primos, ademas de 2 interruptores deslizantes y un sensor de temperatura.
En la tercera parte del ejercicio se agrego un led junto con una fotorresistencia, el led enciende cuando la fotorresistencia se pone en > 300 o < 600

LINK AL PROYECTO:
https://www.tinkercad.com/things/2crX9IE3Eb5-copy-of-intento-4/editel



