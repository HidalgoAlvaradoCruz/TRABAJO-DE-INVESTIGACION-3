## Implementación en Thinkercad de un programa en Arduino por cada uno de los actuadores disponibles: Motor de CC, Control remoto por IR, Microservomotor, Motor de vibración, LCD, Anillo de 12 Neopixeles

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

<br>

En 2017, Tir, Z., Malik, O., Hamida, MA, Cherif, H., Bekakra, Y. y Kadrine, A., en el Congreso Internacional de Ingeniería Eléctrica - Boumerdes realizaron la Implementación de un controlador de velocidad de lógica difusa para un motor de CC de imán permanente utilizando una plataforma Arduino de bajo costo, la implementación de un controlador de velocidad Fuzzy Logic para un motor de CC de imán permanente (PMDC) utilizando un Arduino de bajo costo interconectado con un entorno estándar. La solución Arduino es aceptable a frecuencias de muestreo de kHz. El estudio del control de velocidad del motor PMDC basado en Arduino y L298N H-Bridge utilizando un método de control de inteligencia artificial, ha sido validado mediante experimentos en el sistema físico. (Tir, Z., Malik, O., Hamida,Tir, 2017, p.1) [4].


Rosly, MA, Samad, Z., Shaari, MF y Rosly, MA miembros de la Facultad de Ingeniería Mecánica y Manufactura de la Universidad Tun Hussein Onn Malasia en 2014 Rosly, realizaron estudios de viabilidad del uso del microcontrolador Arduino para el control de actuadores IPMC. El uso del microcontrolador Arduino para controlar el circuito cerrado de la respuesta del actuador de compuesto metálico de polímero iónico (IPMC) diseñado para aplicaciones subacuáticas compactas. Demostramos el control de un solo actuador IPMC mediante el controlador PID utilizando el paquete de soporte MATLAB / Simulink Arduino Input Output (ArduinoIO). Los resultados experimentales muestran que el microcontrolador es capaz de diferenciar la velocidad de respuesta, la estabilidad y el error de seguimiento de diferentes espesores del actuador IPMC cuando es estimulado por múltiples ondas de voltaje y frecuencias.(Rosly, MA, Samad, 2014, p.1) [5].



En 2015, Vidal, Y., Rodellar, J., Acho, L. y Tutiven, C desarrollaron un Control activo tolerante a fallas de actuadores de paso probado en una simulación de ARDUINO de hardware en el circuito para controladores de turbinas eólicas. El número y la complejidad de los sistemas de control en las turbinas eólicas (WT) se están expandiendo rápidamente y su diseño puede marcar la diferencia entre un sistema inmensamente rentable o un sistema dañado. El diseño de un sistema de control robusto requiere probar los algoritmos de control en el hardware del controlador real. Sin embargo, los WT son grandes y costosos, por lo que nos gustaría realizar esta prueba de forma virtual, sin utilizar prototipos del WT. (Vidal, Y., Rodellar, J., Acho, L. y Tutiven, C, 2015, p.1) [6].


En 2014, Davino, D., Giustiniani, A. y Visone, C. del 
Departamento de Ingeniería, Universidad de Sannio, Benevento, Italia realizaron un estudio para la Compensación de histéresis magnetoestrictiva por Arduino: rendimiento flotante versus de punto fijo.
El uso de capacidades computacionales integradas en dispositivos con materiales magnetoestrictivos permite el diseño de objetos, capaces de mostrar funciones inteligentes sin el uso de controladores / dispositivos externos. En este trabajo presentamos la compensación de la histéresis de un actuador magnetoestrictivo utilizando una plataforma Arduino de bajo costo (matemática de punto fijo).  Descubrimos que la solución Arduino es en gran medida aceptable, lidia con errores de compensación dentro de unos pocos porcentajes y tiempos de compensación lo suficientemente rápidos. (Davino, D., Giustiniani, A. y Visone, C, 2014, p.1) [7].


Para el presente trabajo de investigación, se utilizó el entorno de Simulación AUTODESK TINKERCAD dirigido al diseño de varios Circuitos de prueba mediante el uso de ARDUINO para controlar varios ACTUADORES como: Motor de CC,Control remoto por IR, Microservomotor, Motor de vibración, LCD, Anillo de 12 Neopixeles (Tir, Z., Malik, O., Hamida,Tir, 2017, p.1), utilizando el concepto fundamental para estructurar un código que controle a la vez uno o dos actuadores mediante el uso de ARDUINO (Vidal, Y., Rodellar, J., Acho, L. y Tutiven, C, 2015, p.1). Los programas tienen la capacidad de controlar individualmente los ACTUADORES en la simulación de Tinkercad. (Davino, D., Giustiniani, A. y Visone, C, 2014, p.1).

<br>

**4. MARCO TEÓRICO**

**ARDUINO UNO**

Arduino es una plataforma de creación de electrónica de código abierto, la cual está basada en hardware y software libre, flexible y fácil de utilizar para los creadores y desarrolladores. Esta plataforma permite crear diferentes tipos de microordenadores de una sola placa a los que la comunidad de creadores puede darles diferentes tipos de uso.
Arduino UNO es una placa basada en el microcontrolador ATmega328P. Tiene 14 pines de entrada/salida digital (de los cuales 6 pueden ser usando con PWM), 6 entradas analógicas, un cristal de 16Mhz, conexión USB, conector jack de alimentación, terminales para conexión ICSP y un botón de reseteo. Tiene toda la electrónica necesaria para que el microcontrolador opere, simplemente hay que conectarlo a la energía por el puerto USB o con un transformador AC-DC

**Características:**

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


**Diagramas Eléctricos**

<br>

**•	LCD 16 X 2 Y MOTOR CC**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/d5.jpg)

El circuito esta diseñado de manera que la pantalla LCD 16x2 está conectada al ARDUINO y regulada con un potenciómetro para controlar su brillo además tiene un transistor pnp conectado a un potenciómetro para regular la velocidad del Motor CC.

<br>


**•	MICRO SERVO MOTOR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/d4.jpg)

El Micro Servo Motor esta regulado mediante un potenciómetro que controla el ángulo de rotación del Servo a siendo la entrada de datos el puerto A0 y la salida el pin 9 que genera el pulso de activación para el Servo Motor.

<br>

**•	MOTOR VIBRADOR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/d1.jpg)

El motor de vibración se encuentra conectado por su parte positiva al pin 10 del Arduino uno, mientras su polo negativo se encuentra conectado a GND (tierra). De igual manera el diodo led, por su ánodo se encuentra conectado al pin 7 del Arduino y su cátodo a GND (tierra).  

<br>


**•	CONTROL IR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/d2.jpg)

El sensor IR cuenta con tres puertos la tierra que va conectado a GND, el VDD o de poder el cual va conectado a VCC y el “data” el cual está conectado al puerto cuatro del Arduino uno. Mientras la tira de leds cuenta con tres puertos, la tierra el cual va conectado a GND, el de potencia que va conectado a VCC y el de entrada que está conectado al puerto 5 del Arduino.

<br>


**•	ANILLO DE 24 NEO PIXELES** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/d3.jpg)

Se observa un botón el cual por un extremo se encuentra conectado al puerto cinco del Arduino y por el otro extremo se encuentra enlazado a GND o tierra. También existe un diodo led el cual cuenta con su respectiva resistencia de protección, esta se encuentra conectado por su ánodo hacia la resistencia como también al puerto cuatro del Arduino mientras su ánodo se encuentra conectado a tierra. Finalmente se observa el anillo de NeoPixels, para este diagrama esquemático se usó una sustitución con la diferencia que el anillo tiene una figura redonda. Pero cuenta con los mismos puertos, la entrada el cual esta anexada al puerto tres del Arduino, la potencia el cual está conectada con Vcc y tierra el cual está conectado con GND.

<br>

<br>

**Diagrama de bloques**

<br>

**•	LCD 16 X 2 Y MOTOR CC**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/lc6.jpg)

<br>

**•	MICRO SERVO MOTOR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/lc5.jpg)

<br>

**•	CONTROL REMOTO POR IR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/lc3.jpg)

<br>

**•	MOTOR DE VIBRACIÓN**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/lc2.jpg)

<br>

**• MOTOR DE VIBRACIÓN ANILLO DE 12 NEOPIXELES** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/lc1.jpg)

<br>

<br>

**6. LISTA DE COMPONENTES**

<br>

•	Laptop 

Procesador: Intel Core i5-7200U CPU @ 2.50Ghz

Memoria instalada (Ram): 8 Gb 

Tipo de sistema: 64 bits. 

Sistema operativo: Windows 8.0 en adelante. 

<br>
 
•	Software de Simulación Thinkercad 

<br>

**COMPONENTES DE LOS CIRCUITOS DISEÑADOS:**

<br>

**•	LCD 16 X 2 Y MOTOR CC**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/L1.jpg)

<br>

**•	MICRO SERVO MOTOR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/L2.jpg)

<br>

**•	CONTROL REMOTO POR IR** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/L3.jpg)

<br>

**•	MOTOR DE VIBRACIÓN**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/L4.jpg)

<br>

**• MOTOR DE VIBRACIÓN ANILLO DE 12 NEOPIXELES** 

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/L5.jpg)


<br>

<br>


**7. MAPA DE VARIABLES**

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/v1.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/v2.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/v3.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/v4.jpg)

<br>

**8. EXPLICACIÓN DEL CÓDIGO FUENTE**

<br>

**Pantalla LCD 16 X 2 y Motor CC**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cod5.jpg)
 
 <br>

El programa consiste en combinar dos actuadores y controlarlos mediante ARDUINO, el circuito consiste en conectar un Pantalla LCD 16 X 2 y proyectar un mensaje "ENCENDER ACTUADORES", al momento que se realiza esta acción se activa un pulso que es dirigdo hacia un Motor CC cuya velocidad es controlada mediante la resistencia introducida en el Potenciómetro.

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cod1.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cod2.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cod3.jpg)

<br>


![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/f1.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/f2.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/f3.jpg)


<br>

**Micro Servo Motor**


![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cod6.jpg)
 
 <br>

El programa consiste en activar un Micro Servo Motor, la rotación del motor está parametrizada de 0 a 180 grados.

El ángulo en que rota se controla mediante un potenciómetro, entre mayor sea la resistencia que se ingresa en el potenciómetro mayor será el angulo de rotación.
<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cod4.jpg)


<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/f4.jpg)

<br>

**Anillo de 12 Neo Pixeles**



![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img13.png)

La siguiente aplicación trata de la activacion de los LEDS RGB con una animación  sincronizada para el cambio de color en un espacio determinado de tiempo.

La conexión es la siguiente:

Neopixel de entrada “IN”, conectado con el  pin digital "3" del arduino.

Neopixel" PWR" conectado a "5[V]" del Arduino.

Neopixel "G" conectado al tierra o "GND" del Arduino.

Pulsador conectado a tierra o "GND" y Pin digital ~5 del Arduino.

Led con resistencia conectado a tierra o "GND" y Pin digital 4 del Arduino.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img14.png)


![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img7.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img8.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img9.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img10.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img11.png)

**Control remoto por IR**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img19.png)

La siguiente aplicación trata de la activacion de los LEDS RGB en una tira de 6 NeoPixeles con una animación  sincronizada para el cambio de color en un espacio determinado de tiempo.

Para utilizar el control remoto es necesario saber que para cada botón existe un código por lo tanto al  momento de presionar un botón este manda una serie de números que será recibida por el sensor IR y este a la vez es utilizado para manipular la tira de 6 NeoPixeles.
.
La conexión es la siguiente:

Tira de 6 NeoPixel Pin de entrada "DIN" conectado al Pin digital "~5" del arduino.

Tira de 6 NeoPixel Pin "GND" conectado a tierra "GND" del arduino.

Tira de 6 NeoPixel Pin "+5V" conectado a  "5v" del arduino.

Sensor IR Pin "Potencia" conectado a "5v" del arduino.

Sensor IR Pin "Señal" conectado al Pin "4" del arduino.

Sensor IR Pin "GND" conectado a tierra Pin "GND" del arduino.

Nota: Las Tiras de 6 NeoPixel utilizadas son 4, todas conectadas en cascada con sus tres pines en común.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img20.png)


![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img15.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img16.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img17.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img18.png)

**Motor de vibración**

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img23.png)

La siguiente aplicación trata de un motor de vibración que convierte pulsos eléctricos en movimientos mecánicos discretos en este caso de un led.

La conexión es la siguiente:

Motor de vibración pin "Positivo" conectado con el Pin digital "~10" de arduino.

Motor de vibración pin "Negativoo" conectado con tierra Pin "GND" de arduino.

Led "ánodo" conectado con el Pin Digital "7" de arduino.

Led "cátodo" conectado con el Pin "GND" de arduino.


![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img24.png)


![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img21.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/img22.png)

<br>

**9. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN**

<br>

Tener una cuenta de Google o una cuenta institucional en este caso la cuenta de Mi ESPE, debido a que la verificación y creación de la cuenta en Tinkercad será a partir de esta. 

Es esencial tener una conexión estable a internet, debido que será necesario para la creación del circuito en el simulador. 

Los sistemas operativos de los computadores en los cuales funciona Tinkercad son: 

•	Macintosh (con procesador Intel): Mac OS X 10.5, 10.6

•	Windows: Windows XP, Windows Vista, Windows 7

•	GNU / Linux: Ubuntu 8 +, 5 + Debian

<br>

Tener un computador con todas las actualizaciones necesarias, como también nuestro navegador deberá tener las siguientes especificaciones: 

•	Mozilla Firefox 3.6 o superior

•	Apple Safari 5.0 o superior

•	Google Chrome 4.0 o superior

•	Microsoft Internet Explorer 7 o superior

<br>

El circuito creado en Tinkercad puede funcionar en cualquier servidor si se le da el atributo de público y se comparte el enlace que se genera, dicho enlace será la única forma en la que se pueda acceder y editar el diseño del circuito.

<br>

<br>

**10. APORTACIONES**

Implementación en físico de Arduino con actuadores.

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/a1.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/a2.png)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/a3.png)

<br>

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

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/cronograma.jpg)

<br>



**14. BIBLIOGRAFÍA**

[1] Galian, H. (2017, 5 junio). Aprendiendo Arduino. Aprendiendo Arduio. https://aprendiendoarduino.wordpress.com/category/actuadores/

[2]Cardan, J. (2017, 5 febrero). CLR. Uso de Actuadores con Arduino. https://clr.es/blog/es/actuadores-arduino/

[3] Cailla, F. (2018, 1 diciembre). Juegos Robótica. Iniciación a Arduino por bloques #3. Interacción con el medio físico: sensores y actuadores. https://juegosrobotica.es/cursos/curso-iniciacion-arduino-bloques/3-sensores-y-actuadores/

[4] Tir, Z., Malik, O., Hamida, MA, Cherif, H., Bekakra, Y. y Kadrine, A. (2017). Implementación de un controlador de velocidad de lógica difusa para un motor de CC de imán permanente utilizando una plataforma Arduino de bajo costo. 2017 V Congreso Internacional de Ingeniería Eléctrica - Boumerdes (ICEE-B). doi: 10.1109 / icee-b.2017.8192218 

[5] Rosly, MA, Samad, Z., Shaari, MF y Rosly, MA (2014). Estudios de viabilidad del uso del microcontrolador Arduino para el control de actuadores IPMC. 2014 IEEE International Conference on Control System, Computing and Engineering (ICCSCE 2014). doi: 10.1109 / iccsce.2014.7072697 

[6] Vidal, Y., Rodellar, J., Acho, L. y Tutiven, C. (2015). Control activo tolerante a fallas para fallas de actuadores de paso probado en una simulación de hardware en el circuito para controladores de turbinas eólicas. 2015 XXIII Congreso Mediterráneo de Control y Automatización (MED). doi: 10.1109 / med.2015.7158749

[7] Davino, D., Giustiniani, A. y Visone, C. (2014). Compensación de histéresis magnetoestrictiva por Arduino: rendimiento flotante versus de punto fijo. IEEE Transactions on Magnetics, 50 (11), 1–4. doi: 10.1109 / tmag.2014.2320412  

<br>

**15. ANEXOS**

<br>

**15.1 MANUAL DE USUARIO**

<br>

1.	Para ejecutar la simulación de los  Circuitos Actuadores controlados mediante ARDUINO se debe ingresar a los siguienteS enlaces de Tinkercad:

**•	LCD 16 X 2 Y MOTOR CC**

https://www.tinkercad.com/things/0RJk5Bnk6NZ-actuadores/editel?sharecode=v0elIx3IfH7I5sUWBLL7eGSKoobQMO6wK-31DQ5_H8k?sharecode=v0elIx3IfH7I5sUWBLL7eGSKoobQMO6wK-31DQ5_H8k

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m1.jpg)

<br>

**•	MICRO SERVO MOTOR** 

https://www.tinkercad.com/things/4aBM1WC2IdW-micro-servo-motor/editel?sharecode=s-cT7fXU_tnPE4uFage6AvsW53XGo7URlYGG6sal78E

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m2.jpg)


<br>

**•	CONTROL REMOTO POR IR** 

https://www.tinkercad.com/things/4s1lsZ5nRsS-copy-of-trainvcontrol-ir/editel?tenant=circuits?sharecode=Wn_WwZJIUiIhCIZCpTXqwQ4hXOhLvjUYtMWV9o3Lj04

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m3.jpg)

<br>

**•	MOTOR DE VIBRACIÓN**

https://www.tinkercad.com/things/bC2lcUqIPkz-copy-of-trabinvesmotor-de-vibracion/editel?tenant=circuits?sharecode=STefrgk-S4TRrE6naxMbTZG5prn6YaZhpvP-OXesrGg

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m4.jpg)

<br>

**• MOTOR DE VIBRACIÓN ANILLO DE 12 NEOPIXELES** 

https://www.tinkercad.com/things/7uoJzTNgzUh-copy-of-trabinvesanillo-12-neo-pixeles/editel?tenant=circuits?sharecode=2WkW_zUB4osBsBCYWfObZ2cx1VZ830soNz909e_ayoc

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m5.jpg)

<br>

2.	Una vez en la ventana principal de Tinkercad se puede observar el diseño del circuito, para el ejemplo se va ha utilizar el circuito Actuador con una pantalla LCD 16X2 y un Motor CC. Antes de iniciar la simulación se debe verficar que el código de programación ingresado sea el correcto, este proceso se debe relizar en todos los circuitos Actuadores diseñados.

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m6.jpg)

<br>

3.	Una vez revisado el código de programación, para iniciar la simulación se presiona el botón “Iniciar simulación” ubicado en la parte superior derecha.

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m7.jpg)

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m9.jpg)

<br>

4.	El Circuito proyecta un mensaje en la Pantalla LCD y se enciende el Motor CC, tanto el motor como la pantalla LCD se rigen a la resistencia ingresada en el potenciómetro de la siguiente manera:

LCD......Mayor resistencia en el potenciómetro .......  Mayor brillo

Motor CC......Mayor resistencia en el potenciómetro .......  Mayor velocidad

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m8.jpg)

<br>

5.	Finalmente, para detener la simulación presionamos el botón “Detener simulación” y todos los actuadores se detienen y el circuito se apaga.
<br>

![](![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m10.jpg)

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/m11.jpg)

<br>

<br>

**15.2 HOJAS TÉCNICAS**

<br>

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/h1.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/h2.jpg)

![](https://github.com/HidalgoAlvaradoCruz/TRABAJO-DE-INVESTIGACION-3/blob/master/img/h3.jpg)


