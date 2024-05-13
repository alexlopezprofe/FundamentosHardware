# Unidad 6. Arquitectura de centros de proceso de datos

Un centro de procesamiento de datos o CPD (Data Center en inglés) es el lugar o las instalaciones donde se centralizan todas las operaciones e infraestructura de IT de una organización. Aquí se almacenan y procesan los datos y aplicaciones de la misma.

Usualmente es utilizado por medianas y grandes empresas ya que el costo de implementación y mantenimiento es elevado. Existen CPDs “pequeños” que pueden ocupar una sala, o ser enormes centros que ocupan varios pisos de un edificio.

En este sentido, para las compañías la seguridad es un factor importante no solo en lo que a conexiones refiere sino a lo físico. Los Data Centers pueden tener sistemas anti vibraciones para cuidar la vida de los discos de almacenamiento, sistemas contra incendios especiales para equipos electrónicos y por supuesto, un acceso restringido al área. 

![CPD de Google](image.png)


https://www.youtube.com/watch?v=cXVteLWfzQg&ab_channel=Socalcamperz



# Elementos de un CPD

* Servidores
* Almacenamiento
* Refrigeración
* Energía
* Seguridad
* Conectividad
* Monitorización

# Estándar TIA 942. TIER

La **ANSI/TIA-942** es definida como un estándar de calidad creada por el American National Standards Institute (ANSI, por sus siglas en inglés) y el Telecommunications Industry Association (TIA, por sus siglas en inglés) para lograr la adecuada implementación de Data Center a nivel mundial.

Este estándar permite establecer un criterio de medición de los Data Center en cuanto a la parte física, así como su localización, sistema de suministro eléctrico, acondicionamiento térmico, y demás parámetros requeridos del estándar. 

En síntesis, proporciona una serie de recomendaciones y directrices (guidelines) para la instalación de sus infraestructuras.

Cuando una empresa desea validar sus instalaciones debe contar con la certificación adecuada, cumpliendo con los estándares o normas que abarcan en ese entorno.

En el caso de los Data Center, deben cumplir los alcances que establece el estándar ANSI/TIA-942-B.

Este alcance determina las áreas o funcionalidades que serán revisadas, evaluadas y certificadas según los parámetros de la norma, tales como:

*Infraestructura eléctrica.
*Sistema mecánico de enfriamiento.
*Ubicación del Data Center.
*Arquitectura del Data Center.
*Seguridad de Datos.
*Seguridad de las instalaciones.
*Sistemas de detección y supresión de incendios.


## TIER
Los estándar TIA 942 también incorporan la clasificación de los Data Center, conociendo esta clasificación como Tier, los cuáles son unos indicadores que nos sirven para conocer las capacidades y instalaciones de los Data Center

Estos Tier se componen, actualmente, de cuatro niveles diferentes que nos marcan principalmente la disponibilidad de estos, y los tiempos máximos que estos centros de datos pueden estar inoperativos durante un año. Podríamos obtener la siguiente tabla resumen sobre esta clasificación:

![Tier](image-1.png)

![alt text](image-2.png)

* **Tier I:** Es un CPD básico, sin características ni medidas contra fallos inesperados. Tiene todas las funcionalidades básicas de un CPD y permite interrupciones planeadas o no planeadas.
* **Tier II:** Este tipo de CPD cuenta ya con dispositivos redundantes que permite aguantar fallos o interrupciones no planeadas. Cuenta ya con suelo técnico, generador de reserva y alguna medida de redundancia más avanzada que los dispositivos básicos.
* **Tier III:** La característica principal que supone tener este Tier es la redundancia en la línea de alimentación. Esto permite mantenimiento y caídas de tensión sin perder disponibilidad del CPD. Se debe poder realizar tareas de mantenimiento de los dispositivos sin interrumpir el servicio. La mayoría de estos CPDs se construyen para ser convertidos en el siguiente Tier según aumente la demanda de la empresa.
* **Tier IV:** Categoria maxima de un CPD. Debe permitir que los servicios estén siempre activos soportando cualquier tipo de fallo. La redundancia de alimentación pasa a ser alimentación simultánea para no perder tiempo en un posible fallo.

![TIER 4](image-3.png)

# Servidores

## Rack

Un armario o rack es un bastidor dedicado a alojar equipos informáticos y electrónica de red en un CPD. La característica principal de este tipo de bastidores es la optimización que se hace del espacio cuando se dispone de mucho equipamiento. Hay que contar que el equipamiento utilizado en CPDs tiene formas y tamaños específicos para ubicarse en estos armarios y ahorrar el mayor espacio posible.

![Rack](image-5.png)  ![alt text](image-6.png)

## U
Una unidad rack o simplemente U es una unidad de medida usada para describir la altura del equipamiento preparado para ser montado en un rack de 19 o 23 pulgadas de ancho (48,26 cm o 58,42 cm). Una unidad rack equivale a 1,75 pulgadas (4,445 cm) de alto.

Una unidad de rack se escribe normalmente como 1U; del mismo modo dos unidades se escribe 2U y así sucesivamente. La altura de una pieza del equipamiento de un rack es frecuentemente descrita como un número en U.

Un uso común para un rack de 19 pulgadas (también llamado bastidor de 19 pulgadas) es alojar servidores permitiendo configuraciones hardware densas sin ocupar excesivo espacio ni requerir estanterías. La gran mayoría de los racks son de 42U, aproximadamente 78 pulgadas (2 metros) de altura. Normalmente equipo profesional de audio y vídeo viene con opciones de montaje en rack y usa las mismas especificaciones de medida

![alt text](image-7.png)

# Energía

## PDU

Una unidad de distribución de energía PDU (Power distribution unit) por sus siglas en inglés) es un dispositivo para controlar la energía eléctrica en un centro de datos. Las PDU más básicas son grandes regletas sin protección contra sobretensiones. Están diseñadas para proporcionar tomas de corriente estándar para los equipos del centro de datos y no tienen capacidad de supervisión ni de acceso remoto. Las PDU más avanzadas ofrecen funciones de supervisión en tiempo real y acceso remoto.

Las PDU gestionan y distribuyen la electricidad y normalmente se instalan directamente en un rack. La fuente de alimentación puede ser corriente alterna (CA) o corriente continua (CC). Puede proceder de un sistema de alimentación ininterrumpida o SAI, de un proveedor de energía de la red pública o de un generador u otra fuente de energía secundaria. Las PDU también están diseñadas para cumplir con requisitos de alimentación que suelen ser mucho mayores que las regletas y los protectores de sobretensión domésticos o de oficina.

![alt text](image-8.png)

![alt text](image-9.png)

## ATS. Interruptor de transferencia automática (ATS)

Un conmutador de transferencia automática es un interruptor eléctrico que cambia el suministro de energía entre la fuente primaria y la de reserva cuando se produce una interrupción del suministro de energía en cualquiera de las fuentes. Al detectar un fallo en la fuente de alimentación primaria, el ATS activa la fuente de alimentación alternativa, como un sistema de alimentación ininterrumpida. También es capaz de poner en marcha generadores diésel para que funcionen los aparatos eléctricos hasta que se restablezca el suministro eléctrico.

Un conmutador de transferencia automática actúa como intermediario entre el equipo eléctrico y la fuente de alimentación. Es esencial disponer de energía ininterrumpida en el centro de datos. Para su correcto mantenimiento, los sistemas conectados a la red eléctrica deben ser debidamente revisados y probados. Para garantizar la fiabilidad de un ATS durante un corte de energía, los administradores del centro de datos deben supervisarlo regularmente.

![ATS](image-10.png)

## SAI. Sistema alimentación ininterrumpida

SAI (Sistema alimentación ininterrumpida) o UPS (Uninterrupted Power Supply) son dispositivos que se utilizan  para proporcionar protección contra problemas eléctricos y cortes de corriente

Una de las funciones principales que tiene un SAI (UPS) es la de  suministrar energía eléctrica acumulada en sus baterías cuando se producen apagones o cortes de suministro eléctrico, impidiendo así posibles averías de los dispositivos conectados al evitar que se apaguen repentinamente, pero no es la única función, la mayoría de los sistemas de alimentación ininterrumpida disponen de un AVR o regulador de tensión lo que nos garantiza un estabilidad en la corriente de salida eliminando armónicos de la red eléctrica  para lograr una alimentación más constante lo que ayuda a extender la vida útil de los equipos conectados al SAI. 

### Tecnologías de SAI

#### Off-Line
Un SAI dotado con tecnología Off-Line suministra la corriente eléctrica sin ningún filtro a los dispositivos conectados,  este tipo de tecnología carece de AVR (Regulador de voltaje). El SAI  Off-Line solamente empezará a funcionar cuando detecte un fallo de corriente eléctrica, es en este momento preciso cuando el SAI conmuta a modo baterías, es decir se comenzará a suministrar la energía que ha ido almacenando en sus baterías a los dispositivos conectados. Estos Sais necesitan un tiempo de conmutación (normalmente 2-10 ms) para pasar a modo baterías, es preciso tener este dato en cuenta a la hora de conectar dispositivos sensibles que pudieran verse afectados en el proceso de conmutación,  es impórtate indicar que este tipo de Sais son solo recomendables para las zonas que disponen de una red estable ya que al no realizar ningún filtrado de la corriente, solo protegen ante un corte de suministro eléctrico.

![image](https://github.com/alexlopezprofe/FundamentosHardware/assets/148449360/4ac33889-0d62-490d-83ec-7a9f6951ad13)

#### In-Line

Un SAI Interactivo o In-Line ofrece una protección eléctrica intermedia, su tecnología es similar a la de los Sais Off-Line pero incorpora una serie de filtros activos como microprocesador que controla las fluctuaciones de la red eléctrica en ±15%, regulando la tensión de salida (efecto Buck/Boos AVR Integrado) habitualmente este tipo de Sais devuelven una onda pseudo-sinusoidal o sinusoidal pura dependiendo del modelo , este proceso de filtrado y mejora de la corriente que llega a los dispositivos conectados al SAI se realiza sin que entren a funcionar las baterías, por lo que la protección con un SAI interactivo es superior aún sin sufrir apagones. Al igual que los SAI Off-line tienen un pequeño tiempo de conmutación en el que no hay suministro eléctrico, normalmente de 2-10 ms, es por este motivo por el que se tiene que tener especial cuidado a la hora de conectar dispositivos sensibles que pudieran verse afectados en el tiempo de conmutación a modo baterías.

![image](https://github.com/alexlopezprofe/FundamentosHardware/assets/148449360/dcaa7025-e673-4d06-b4ae-c199a5dcb7b1)

#### On-Line

Un SAI On-Line realiza una doble conversión de la energía eléctrica que recibe, transformándola en continua y después a alterna de nuevo, eliminando de esta manera todos los problemas que pueda tener. Un Sai On-Line siempre proporciona energía eléctrica directamente desde sus baterías mientras estas se van cargando de la red, y esto es lo que garantiza que la protección contra cualquier problema de la red eléctrica sea total. Debido a su alta fiabilidad, la tecnología On-Line ocupa el sector profesional en el mercado de SAIS y está generalmente destinada a proteger servidores, equipos industriales o cualquier instalación informática que por su importancia o coste necesite la seguridad de no verse afectados por problemas derivados de la red eléctrica.

![image](https://github.com/alexlopezprofe/FundamentosHardware/assets/148449360/aed09ab9-ddb0-4018-b2c2-4594836f28d3)

#### Capacidad SAI

**Potencia aparente (S)**

La unidad de "potencia aparente" (S) que encontramos en los Sais es el Voltiamperio (Va) o el KiloVoltioampério (KVa), también llamado Kavea ( 1KVa = 1000 Va ).

La fórmula es: S=V*I; donde la «S» es la potencia eléctrica total cuya unidad es el voltiamperio (VA), la «V» es la tensión eléctrica (V) y la «I» es la corriente eléctrica (A)

**Factor de potencia FP**

Es la relación entre la energía suministrada (potencia aparente) y la energía realmente consumida (potencia activa). 

Se calcula así: FP=P/S; donde el «FP» es la relación entre la potencia activa y la potencia aparente y carece de unidad, la «P» es la potencia activa (W) y la «S» es la potencia aparente (VA).

Ejemplo: Si tenemos un consumo de P=400W y un factor de potencia FP=0.6 Necesitos un SAI de potencia aparente de al menos S=P/FP=666.6VA

EL factor de pontencia tambien lo podemos ver expresado en porcentaje FP=0.6=60%

**Autonomía**

T = [(N*V*Ah*Ef)/S]*60

Donde
* T: Es el tiempo de autonomía total que tendrá el SAI
* N: Es el número de baterías del SAI, normalmente el fabricante indica este parámetro
* V: Es la tensión que ofrecen las baterías
* Ah: Son los amperios/hora (Ah) de la batería
* Ef: Es la eficiencia de las baterías. Normalmente es entre el 98-90%, aunque normalmente para el cálculo de la autonomía se toma el 95%, que es un término medio
* S: Es la potencia aparente del SAI
* 60: Representa una hora en minutos y sirve para convertir el resultado en una unidad de medida fácilmente manejable

Ejemplo

Pongamos que tenemos un SAI de 700VA, dos baterías, una tensión de batería de 9V y 5Ah. Suponemos además una eficiencia del 95% (cuando lo aplicamos en la fórmula, es interesante hacerlo ya convertido, siendo 0.95). Ahora simplemente cambiamos los datos en la fórmula, tal que así:

T= [(2*9*5*0.95)/700]*60  —>  T= 7.32 minutos

Así que con el SAI elegido, tendremos más de 7 minutos de autonomía para poder cerrar el sistema con seguridad. Debemos tener en cuenta que la potencia para la que estamos el SAI es superior a la potencia real de consumo, para tener un margen, así que la autonomía será mucho mayor. Sea como fuese, la autonomía es más que suficiente para apagar el sistema con seguridad.

https://www.rackonline.es/sai-ups

# Refrigeración

La producción de calor de los equipos que conforman un centro de datos es uno de los problemas principales y que más preocupa a sus administradores. El exceso de calor en una sala de servidores afecta negativamente el rendimiento del equipo y acorta su vida útil, además de suponer un peligro en el caso de alcanzar niveles elevados. Por eso, es de vital importancia el diseño de un buen sistema de refrigeración de los centros de datos.

En este diseño es fundamental el dimensionamiento del sistema, que exige comprender la cantidad de calor producida por los equipos TI, así como la derivada del funcionamiento de otros elementos habitualmente presentes como los SAI, la distribución de alimentación, unidades de aire acondicionado, iluminación y personas…

Fijarse en todo ello es básico para calcular la carga térmica. En una instalación típica, las cargas que más peso tienen son:

* El 70% se suele corresponder con la carga de los equipos TI.
* El 9%, a la iluminación.
* El 6%, a la distribución de la alimentación.
* El 2%, a las personas.

https://www.youtube.com/watch?v=vZkA0z9JRgw&ab_channel=TheEngineeringMindset

# Monitorización

Cuando se dispone de tanto equipamiento informático (en un solo CPD puede haber cientos de equipos informáticos y otros dispositivos) se hace muy necesario poder monitorizar su comportamiento. No es posible evaluar el rendimiento o vigilar los equipos de forma manual.

Herramientas como Nagios [Nagios](https://www.nagios.org/) permiten monitorizar todo el equipamiento informático de una manera automática y gráfica, de manera que en caso de fallo es la propia aplicación quién avisa a los técnicos del equipo que ha fallado y por qué.

![Nagios](image-4.png)

# Bibliografía
* https://ucloudglobal.com/blog/centro-procesamiento-de-datos/
* https://es.wikipedia.org/wiki/Unidad_rack
* https://www.cofrico.com/procesos-industriales/la-refrigeracion-de-los-centros-de-datos/

