## Implementación en Thinkercad de un programa en Arduino por cada uno de los actuadores disponibles:Motor de CC,Control remoto por IR,Microservomotor, Motor de vibración,LCD,Anillo de 12 Neopixeles

<br>

<br>

**1. PLANTEAMIENTO DEL PROBLEMA**

Se desconoce el funcionamiento, conexión, diseño e implemetación en Thinkercad de un programa en Arduino para actuadores, para lo cual se formularon las siguientes preguntas: 

•	¿Cómo se implementa en Thinkercad un programa en arduino?

•	¿Cómo funcionan los actuadores?

•	¿Cuál es la conexión entre el arduino y actuadores?

<br>

<br>

**2. OBJETIVOS**


**Objetivo general**

Implementar en Thinkercad un programa en Arduino por cada uno de los actuadores disponibles.

**Objetivos específicos**

•	Comprender la estructura básica de funcionamiento del arduino.

•	Entender el funcionamiento de la programación utilizada entre arduino y actuadores.

•	Identificar los principales caraacterísticas y funcionamiento de los actuadores. 

<br>

<br>


**3. ESTADO DEL ARTE**



**4. MARCO TEÓRICO**

**ARDUINO UNO**

Arduino es una plataforma de creación de electrónica de código abierto, la cual está basada en hardware y software libre, flexible y fácil de utilizar para los creadores y desarrolladores. Esta plataforma permite crear diferentes tipos de microordenadores de una sola placa a los que la comunidad de creadores puede darles diferentes tipos de uso.
Arduino UNO es una placa basada en el microcontrolador ATmega328P. Tiene 14 pines de entrada/salida digital (de los cuales 6 pueden ser usando con PWM), 6 entradas analógicas, un cristal de 16Mhz, conexión USB, conector jack de alimentación, terminales para conexión ICSP y un botón de reseteo. Tiene toda la electrónica necesaria para que el microcontrolador opere, simplemente hay que conectarlo a la energía por el puerto USB o con un transformador AC-DC

**Caracterícas:**

•	Microcontrolador: ATmega328 

•	Voltaje de operación: 5V

•	Voltaje de entrada (recomendado): 7-12V 

•	Voltaje de entrada (límites): 6-20V 

•	Pines de E/S digitales: 14 (de los cuales 6 proporcionan salida PWM) 

•	Pines de entrada analógica: 6

•	Corriente DC por pin de E/S: 40 mA 

•	Corriente DC para 3.3V Pin: 50 mA

•	Memoria Flash: 32 KB de los cuales 0,5 KB utilizados por el bootloader 

•	SRAM: 2 KB (ATmega328) 

•	EEPROM: 1 KB (ATmega328) 

•	Velocidad de reloj: 16 MHz


**ESPECIFICACIONES ARDUINO UNO**

![](https://github.com/EvelinHidalgo/THINKERCAD-ESP8266-ARDUINO/blob/master/img/img1.jpg)

**1.Botón de reset:** Sirve para inicializar nuevamente el programa cargado en el microcontrolador de la placa. Cuando deje de responder el Arduino Uno es el botón de encendido o apagado para que vuelva a restablecerse. 

**2. Pines o puertos de entrada y salida:** son los pines donde conectar los sensores, componentes y actuadores que necesiten de señales digitales

**3. Pines o puertos de entrada y salida:** son los pines donde conectar los sensores, componentes y actuadores que necesiten de señales digitales.

**4.Puerto USB:** Utilizado tanto para conectar con un ordenador y transferir o cargar los programas al microcontrolador como para dar electricidad al Arduino. También se usa como puerto de transferencia serie a la placa, tanto para transmisión como para recepción de datos.

**5. Chip de interface USB:** es el encargado de controlar la comunicación con el puerto USB.

**6.Reloj oscilador:** es el elemento que hace que el Arduino vaya ejecutando las instrucciones. Es el encargado de marcar el ritmo al cual se debe ejecutar cada instrucción del programa.

**7. Led de encendido:** es un pequeño LED que se ilumina cuando la placa esta correctamente alimentada.

**8. Microcontrolador:** este es el cerebro de cualquier placa Arduino. Es el procesador que se encarga de ejecutar las instrucciones de los programas.

**9. Regulador de tensión:** este sirve para controlar la cantidad de electricidad que se envía a los pines, con lo que asegura que no se estropee lo que conectemos a dichos pines.

**10. Puerto de corriente continua:** este puerto es el que se usa para darle electricidad a la placa si no se usa alimentación USB.

**11. Zócalo de tensión:** aquí estarán los pines con los que alimentaremos nuestro circuito.

**12. Entradas analógicas:** zócalo con distintos pines de entrada analógica que permiten leer entradas analógicas.
POTENCIA

La placa puede funcionar con una alimentación externa de 6 a 20 voltios. Sin embargo, si se suministra con menos de 7V, la clavija de 5V puede suministrar menos de cinco voltios y la placa puede ser inestable. Si se utilizan más de 12V, el regulador de voltaje puede sobrecalentarse y dañar la placa. El rango recomendado es de 7 a 12 voltios.

**Pines de potencia**

•	VIN:El voltaje de entrada a la placa Arduino cuando está usando una fuente de alimentación externa (a diferencia de los 5 voltios de la conexión USB u otra fuente de alimentación regulada). Puede suministrar tensión a través de esta clavija o, si lo hace a través de la toma de corriente, acceder a ella a través de esta clavija. 

•	5V: Esta clavija emite un 5V regulado desde el regulador de la tarjeta. La tarjeta puede alimentarse ya sea desde el conector de alimentación de CC (7 – 12 V), el conector USB (5 V) o la clavija VIN de la tarjeta (7-12 V). La alimentación de tensión a través de las clavijas de 5V o 3,3V puentea el regulador y puede dañar la placa. 

•	3V3: Una alimentación de 3,3 voltios generada por el regulador de a bordo. El consumo máximo de corriente es de 50 mA.

•	GND: Pins de tierra.

**ENTRADA Y SALIDA, INPUT AND OUTPUT**

Cada uno de los 14 pines digitales de la Uno puede utilizarse como entrada o salida, utilizando las funciones pinMode(), digitalWrite() y digitalRead(). Funcionan a 5 voltios. Cada clavija puede proporcionar o recibir un máximo de 40 mA y tiene una resistencia pull-up interna (desconectada por defecto) de 20-50 kOhms. Además, algunos pines tienen funciones especializadas: 

•	Serial: 0 (RX) y 1 (TX). Se utiliza para recibir (RX) y transmitir (TX) datos en serie TTL. Estos pines están conectados a los pines correspondientes del chip Serial ATmega8U2 USB-to-TTL.

•	Interrupciones externas: 2 y 3. Estos pines pueden configurarse para activar una interrupción en un valor bajo, un flanco ascendente o descendente, o un cambio de valor. Vea la función attachInterrupt () para más detalles. 

•	PWM: 3, 5, 6, 9, 10 y 11. Proporciona salida PWM de 8 bits con la función analogWrite (). 

•	SPI: 10 (SS), 11 (MOSI), 12 (MISO), 13 (SCK). Estos pines soportan la comunicación SPI utilizando la biblioteca SPI. 

•	LED 13: Hay un LED incorporado conectado al pin 13 digital. Cuando la clavija es de valor ALTO, el LED se enciende, cuando la clavija es BAJA, se apaga. 

La Uno tiene 6 entradas analógicas, etiquetadas de A0 a A5, cada una de las cuales proporciona 10 bits de resolución (es decir, 1024 valores diferentes). Por defecto miden de tierra a 5 voltios, aunque es posible cambiar el extremo superior de su rango usando el pin AREF y la función analogReference(). 

**PINES TIENEN FUNCIONALIDAD ESPECIALIZADA**

•	TWI: Pin A4 o SDA y pin A5 o SCL. Soporta la comunicación TWI usando la biblioteca Wire.

•	AREF: Tensión de referencia para las entradas analógicas. Se utiliza con analogReference (). 

•	RESET: Lleve esta línea a un nivel BAJO para reiniciar el microcontrolador. Típicamente se usa para añadir un botón de reinicio a los escudos que bloquean el que está en la placa.

**DIAGRAMA PINOUT ARDUINO UNO**

![](https://github.com/EvelinHidalgo/THINKERCAD-ESP8266-ARDUINO/blob/master/img/img2.jpg)

**ARDUINO UNO PINOUT – FUENTE DE ALIMENTACIÓN**

Hay 3 formas de alimentar el Arduino Uno: 

•	Barrel Jack: El Barrel Jack, o DC Power Jack puede ser usado para alimentar tu placa Arduino. El conector cilíndrico suele estar conectado a un adaptador de pared. La tarjeta puede ser alimentada por 5-20 voltios, pero el fabricante recomienda mantenerla entre 7-12 voltios. Por encima de 12 voltios, los reguladores podrían sobrecalentarse, y por debajo de 7 voltios, podrían no ser suficientes.

•	VIN Pin: Este pin se utiliza para alimentar la placa Arduino Uno utilizando una fuente de alimentación externa. El voltaje debe estar dentro del rango mencionado anteriormente. 

•	Cable USB :cuando se conecta a la computadora, proporciona 5 voltios a 500mA.

![](https://github.com/EvelinHidalgo/THINKERCAD-ESP8266-ARDUINO/blob/master/img/img3.jpg)

Hay un diodo de protección de polaridad que se conecta entre el positivo de la clavija del barril y la clavija VIN, con una capacidad nominal de 1 amperio.

Cuando se alimenta un circuito a través de la toma de barril o VIN, la capacidad máxima disponible está determinada por los reguladores de 5 y 3.3 voltios a bordo del Arduino. 

•	5v y 3v3 Proporcionan 5 y 3.3v regulados para alimentar componentes externos de acuerdo con las especificaciones del fabricante. 

•	GND En el pinout de Arduino Uno, puedes encontrar 5 pines GND, todos ellos interconectados. 

Las clavijas GND se utilizan para cerrar el circuito eléctrico y proporcionar un nivel de referencia lógico común en todo el circuito. Asegúrate siempre de que todos los GNDs (del Arduino, periféricos y componentes) estén conectados entre sí y tengan una conexión a tierra común. 

•	RESET – reinicia el Arduino

•	IOREF – Este pin es la referencia de entrada/salida. Proporciona la referencia de tensión con la que funciona el microcontrolador.

**ARDUINO UNO PINOUT – ANALOG IN**

 La placa Arduino Uno tiene 6 pines analógicos, que utilizan ADC (Convertidor de Analógico a Digital). Estos pines sirven como entradas analógicas, pero también pueden funcionar como entradas o salidas digitales.
 
![](https://github.com/EvelinHidalgo/THINKERCAD-ESP8266-ARDUINO/blob/master/img/img4.jpg)

**Conversión de analógico a digital**

 ADC son las siglas de Analog to Digital Converter. El ADC es un circuito electrónico utilizado para convertir señales analógicas en señales digitales. Esta representación digital de señales analógicas permite al procesador, que es un dispositivo digital, medir la señal analógica y utilizarla durante su funcionamiento. 
Los pines Arduino A0-A5 son capaces de leer tensiones analógicas. En Arduino el ADC tiene una resolución de 10 bits, lo que significa que puede representar una tensión analógica de 1.024 niveles digitales. El ADC convierte el voltaje en bits que el microprocesador puede entender.

**ARDUINO UNO PINOUT – DIGITAL PINS**

•	Los pines 0-13 del Arduino Uno sirven como pines de entrada/salida digital.

•	El pin 13 del Arduino Uno está conectado al LED incorporado. 

•	En el Arduino Uno – los pines 3,5,6,9,10,11 tienen capacidad PWM.
 Es importante tener en cuenta: 
 
•	Cada clavija puede proporcionar hasta 40 mA máx. Pero la corriente recomendada es de 20 mA. 

•	La corriente máxima absoluta proporcionada de todos los pines juntos es de 200 mA.

![](https://github.com/EvelinHidalgo/THINKERCAD-ESP8266-ARDUINO/blob/master/img/img5.jpg)

**ACTUADORES**

Un actuador es un dispositivo capaz de transformar energía hidráulica, neumática o eléctrica en la activación de un proceso con la finalidad de generar un efecto sobre elemento externo. Este recibe la orden de un regulador, controlador o en nuestro caso un Arduino y en función a ella genera la orden para activar un elemento final de control como, por ejemplo, una válvula.

Existen varios tipos de actuadores como son:

•	Electrónicos

•	Hidráulicos

•	Neumáticos

•	Eléctricos

•	Motores

•	Bombas

Los actuadores van conectados a las salidas de Arduino.

**Motor de CC**

Los motores de corriente continua a menudo se usan con una caja de engranajes para aumentar el torque mientras se mantienen las pequeñas dimensiones. El motor DC es bastante simple de usar. Para que funcione, lo único que hay que hacer es aplicarle voltaje. La señal y el nivel de voltaje determinarán la velocidad y la dirección de rotación.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img1.jpg)

**Control remoto por IR**

El control remoto IR (infrarrojos) o mando a distancia de infrarrojos funciona emitiendo pulsos de luz infrarroja (por debajo del visible). La señal infrarroja transmite el código correspondiente al botón del mando a distancia pulsado al dispositivo en forma de una serie de impulsos de luz infrarroja. El receptor recibe la serie de impulsos de infrarrojos y los pasa a un procesador que descodifica y activarán una determinada función del dispositivo.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img2.jpg)

**Microservomotor**

Servo es un tipo de motor DC con reductora que sólo puede girar 180 grados. Se controla mediante el envío de impulsos eléctricos de Arduino. Estos pulsos le dice al servo a qué posición se debe mover. El Servo tiene tres cables, marrón es el cable a masa y debe conectarse a GND, el rojo es el cable de corriente y debe conectarse al puerto de 5v y el naranja es el cable de señal y debe conectarse al pin #9.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img3.png)

**Motor de vibración**

Este es un pequeño motor de vibración adecuado como un indicador no audible. Cuando la entrada es alta, el motor vibra, al igual que un teléfono en modo silencioso.Posee un controlador de amplificación Mos, puede pasar directamente el control de puerto digital Ard-uino.La intensidad de vibración del motor puede ser controlada por PWM; este módulo puede convertir fácilmente señales eléctricas a vibraciones mecánicas.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img4.jpg)

**LCD**

Una pantalla LCD (liquid crystal display: ‘pantalla de cristal líquido’ por sus siglas en inglés) es una pantalla delgada y plana formada por un número de píxeles en color o monocromos colocados delante de una fuente de luz o reflectora. A menudo se utiliza en dispositivos electrónicos de pilas, ya que utiliza cantidades muy pequeñas de energía eléctrica.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img5.jpg)

**Anillo de 12 Neopixeles**

Los NeoPixel son originales de Adafruit y son diodos LED de tipo 5050 con un controlador WS2812 integrado. Existen en varios tamaños y formas y tienen una amplia documentación, tutoriales así como librerías lista para utilizar con Arduino.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img6.jpg)

**5. DIAGRAMAS**



**Diagramas Eléctrico**



**Diagrama de bloques**



**6. LISTA DE COMPONENTES**



**7. MAPA DE VARIABLES**



**8. EXPLICACIÓN DEL CÓDIGO FUENTE**


**Anillo de 12 Neo Pixeles**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img7.png)

**9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN**



**10. APORTACIONES**



**11. CONCLUSIONES**

<br>

En conclusión:

•	Arduino al ser una plataforma de código abierto permite la simplificación del proceso de trabajo de micro controladores ayudando incluso en el uso de un lenguaje de programación muy entendible y fácil ,convirtiéndose  en un instrumento altamente flexible y adaptable para desarrollar actuadores.

•	La evidencia que los actuadores hacen parte de los elementos más importantes en la industria es inevitable por lo tanto  gracias a ellos es posible verificar su misión de  generar el movimiento de los elementos de estos según las órdenes dadas mediante el Arduino su unidad de control.

•	Controlar cada uno de los actuadores disponibles en Thinkercad desde Arduino se tornó una tarea sencilla gracias al uso de la librerías existentes para cada actuador simplificando de gran manera la programación.


**12. RECOMENDACIONES**


•	Recordar que Arduino solo puede manejar un total de 200 mA de salida. Es decir  es redomendable que la corriente máxima que admite Vcc y GND son 200 mA.

•	Recordar que los pines Arduino solo pueden tener los valores de 5V (3.3V en algunos modelos) y 0V. No es posible cualquier otro valor de tensión.

•	Recordar que los pines de Arduino solo pueden manejar un máximo de 40mA y recomendable usar 20mA de forma continua.





**13. CRONOGRAMA**



**14. BIBLIOGRAFÍA**



**15. ANEXOS**

<br>

**15.1 MANUAL DE USUARIO**


**15.2 HOJAS TÉCNICAS**



