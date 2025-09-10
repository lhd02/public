# Cableado del sistema de almacenamiento fotovoltaico

* Los productos de nuestra empresa se pueden usar para un sistema doméstico de almacenamiento de energía. El sistema doméstico de almacenamiento de energía está formado por paneles fotovoltaicos, inversores, paquetes de baterías, interruptores de control maestro, Gateway, cargas, redes eléctricas, etc.
* La función principal del sistema doméstico de almacenamiento de energía es almacenar la corriente continua generada por los paneles fotovoltaicos en paquetes de baterías. O, alternativamente, la electricidad del sistema fotovoltaico y el paquete de baterías puede convertirse en corriente alterna para que lo use la carga o bien incorporarse a la red.

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">**En cableado del sistema de corriente de emergencia, la duración del funcionamiento aislada de la red de la carga de corriente de emergencia depende de la capacidad de suministro de energía del sistema de almacenamiento fotovoltaico. Si durante el funcionamiento aislado de la red el suministro de energía del sistema de almacenamiento fotovoltaico presenta alguna anomalía (incluidas, entre otras, generación anómala de energía fotovoltaica, carga insuficiente de la batería o suministros de energía del generador diésel anómalos), la carga de corriente de emergencia no podrá funcionar.**</mark>

### **Diagrama de cableado de un sistema de reserva doméstico total**

<figure><img src="../../.gitbook/assets/SHA1OV00009-es.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="61.11114501953125" align="center">N.º</th><th width="114.77777099609375">Descripción</th><th width="60.33331298828125" align="center">N.º</th><th>Descripción</th><th width="59" align="center" valign="middle">N.º</th><th>Descripción</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>Panel FV</td><td align="center"><strong>B</strong></td><td>Sigen Hybrid</td><td align="center" valign="middle"><strong>C</strong></td><td>Sistema de almacenamiento de energía SigenStor (SigenStor BC + SigenStor BAT)</td></tr><tr><td align="center"><strong>D</strong></td><td>Gateway</td><td align="center"><strong>E</strong></td><td>Panel de distribución de reserva</td><td align="center" valign="middle"><strong>F</strong></td><td>Cargas domésticas de reserva</td></tr><tr><td align="center"><strong>G</strong></td><td>Generador diésel</td><td align="center"><strong>H</strong></td><td>Cargas inteligentes</td><td align="center" valign="middle"><strong>I</strong></td><td>Red eléctrica</td></tr><tr><td align="center"><strong>J</strong></td><td>mySigen</td><td align="center"><strong>K</strong></td><td>Enrutador</td><td align="center" valign="middle"><strong>L</strong></td><td>Antena</td></tr><tr><td align="center"><strong>M</strong></td><td>CommMod</td><td align="center"></td><td></td><td align="center" valign="middle"></td><td></td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">No pueden utilizarse más de 20 unidades Sigen Hybrid en cascada.</mark>
* <mark style="color:blue;">El sistema de almacenamiento de energía Sigen Hybrid + SigenStor admite la conexión a ambas configuraciones de sistema de almacenamiento de energía Sigen Hybrid + SigenStor y sistemas Sigen Hybrid autónomos.</mark>
* <mark style="color:blue;">Si F (carga doméstica de reserva) sufre una fuga, puede comportar un riesgo de descarga eléctrica. Para evitar este peligro, debe instalarse un dispositivo de corriente residual (RCD) entre D (Gateway) y F (carga doméstica de reserva).</mark>
* <mark style="color:blue;">Como generador de energía de reserva para aplicaciones sin conexión a la red de largo plazo, el generador diésel puede trabajar en tándem con la Gateway para proporcionar una transición suave entre FV, almacenamiento y generación diésel.</mark>
* <mark style="color:blue;">Todos los equipos eléctricos del hogar del propietario pueden conectarse como cargas inteligentes. Para asegurar que este producto maximiza los beneficios a los usuarios, se recomienda conectar como cargas inteligentes los equipos de alta potencia (bombas de calor, calentadores de piscina, secadoras, etc.) que pueden desconectarse si el sistema de almacenamiento de energía tiene poca energía. Otros equipos de baja potencia (luces, enrutadores, etc.) se conectan como cargas domésticas.</mark>
* <mark style="color:blue;">Se recomienda utilizar Fast Ethernet y WLAN para la comunicación con los inversores. Cuando el tráfico 4G gratuito de CommMod se agote, los usuarios deben ampliar sus cuentas o sustituir la tarjeta SIM.</mark>

### **Diagrama de cableado de un sistema de reserva doméstico parcial**

<figure><img src="../../.gitbook/assets/SHA1OV00010-es.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="59.11114501953125" align="center">N.º</th><th width="142">Descripción</th><th width="60.22216796875" align="center">N.º</th><th width="151">Descripción</th><th width="60.22216796875" align="center">N.º</th><th>Descripción</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>Panel FV</td><td align="center"><strong>B</strong></td><td>Sigen Hybrid</td><td align="center"><strong>C</strong></td><td>Sistema de almacenamiento de energía SigenStor (SigenStor BC + SigenStor BAT)</td></tr><tr><td align="center"><strong>D</strong></td><td>Gateway</td><td align="center"><strong>E1</strong></td><td>Panel de distribución de reserva</td><td align="center"><strong>E2</strong></td><td>Panel de distribución de energía sin reserva</td></tr><tr><td align="center"><strong>F1</strong></td><td>Cargas domésticas de reserva</td><td align="center"><strong>F2</strong></td><td>Cargas domésticas sin reserva</td><td align="center"><strong>G</strong></td><td>Generador diésel</td></tr><tr><td align="center"><strong>H</strong></td><td>Cargas inteligentes</td><td align="center"><strong>I</strong></td><td>Sensor de energía</td><td align="center"><strong>J</strong></td><td>Sensor de energía</td></tr><tr><td align="center"><strong>K</strong></td><td>mySigen</td><td align="center"><strong>L</strong></td><td>Enrutador</td><td align="center"><strong>M</strong></td><td>Antena</td></tr><tr><td align="center"><strong>N</strong></td><td>CommMod</td><td align="center"></td><td></td><td align="center"></td><td></td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">No pueden utilizarse más de 20 unidades Sigen Hybrid en cascada.</mark>
* <mark style="color:blue;">El sistema de almacenamiento de energía Sigen Hybrid + SigenStor admite la conexión a ambas configuraciones de sistema de almacenamiento de energía Sigen Hybrid + SigenStor y sistemas Sigen Hybrid autónomos.</mark>
* <mark style="color:blue;">Si E2 (panel de distribución de energía sin reserva) cuenta con protección contra fugas, se recomienda que la corriente de funcionamiento residual nominal sea mayor o igual al número de inversores x 100 mA.</mark>
* <mark style="color:blue;">Si F1 (carga doméstica de reserva) sufre una fuga, puede comportar un riesgo de descarga eléctrica. Para evitar este peligro, debe instalarse un dispositivo de corriente residual (RCD) entre D (Gateway) y F1 (carga doméstica de reserva).</mark>
* <mark style="color:blue;">Como generador de energía de reserva para aplicaciones sin conexión a la red de largo plazo, el generador diésel puede trabajar en tándem con la Gateway para proporcionar una transición suave entre FV, almacenamiento y generación eléctrica diésel.</mark>
* <mark style="color:blue;">Todos los equipos eléctricos del hogar del propietario pueden conectarse como cargas inteligentes. Para asegurar que este producto maximiza los beneficios a los usuarios, se recomienda conectar como cargas inteligentes los equipos de alta potencia (bombas de calor, calentadores de piscina, secadoras, etc.) que pueden desconectarse si el sistema de almacenamiento de energía tiene poca energía. Otros equipos de baja potencia (luces, enrutadores, etc.) se conectan como cargas domésticas.</mark>
* <mark style="color:blue;">El sensor de energía tiene la función de adquisición de datos para los puntos de conexión a la red que permiten la conexión a la red de suministro cero. Para cablear un sistema de reserva doméstica parcial no es necesario configurar el sensor de energía. Al cablear un sistema de red de reserva parcial y conexión a la red con conexión a la red eléctrica con potencia cero, se configura el sensor de energía.</mark>
* <mark style="color:blue;">Se recomienda utilizar Fast Ethernet y WLAN para la comunicación con los inversores. Cuando el tráfico 4G gratuito de CommMod se agote, los usuarios deben ampliar sus cuentas o sustituir la tarjeta SIM.</mark>

### **Diagrama de cableado de un sistema sin reserva**

<figure><img src="../../.gitbook/assets/SHA1OV00011-es.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="91">N.º</th><th width="149">Descripción</th><th width="74">N.º</th><th>Descripción</th><th width="82">N.º</th><th>Descripción</th></tr></thead><tbody><tr><td><strong>A</strong></td><td>Panel FV</td><td><strong>B</strong></td><td>Sigen Hybrid</td><td><strong>C</strong></td><td>Sistema de almacenamiento de energía SigenStor (SigenStor BC + SigenStor BAT)</td></tr><tr><td><strong>D</strong></td><td>Interruptor de CA</td><td><strong>E</strong></td><td>Panel de distribución</td><td><strong>F</strong></td><td>Cargas domésticas</td></tr><tr><td><strong>G</strong></td><td>Sensor de energía</td><td><strong>H</strong></td><td>Red eléctrica</td><td><strong>I</strong></td><td>mySigen</td></tr><tr><td><strong>J</strong></td><td>Enrutador</td><td><strong>K</strong></td><td>Antena</td><td><strong>L</strong></td><td>CommMod</td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">No pueden utilizarse más de 20 unidades SigenStor en cascada.</mark>
* <mark style="color:blue;">El sistema de almacenamiento de energía Sigen Hybrid + SigenStor admite la conexión a ambas configuraciones de sistema de almacenamiento de energía Sigen Hybrid + SigenStor y sistemas Sigen Hybrid autónomos.</mark>
* <mark style="color:blue;">El voltaje nominal del conmutador de CA conectado a cada</mark> <mark style="color:blue;">inversor de la serie Sigen Hybrid (2.0-6.0) SP2</mark> <mark style="color:blue;">debe ser ≥ 240 Vca y se recomienda la siguiente corriente nominal:</mark>
  * <mark style="color:blue;">Sigen Hybrid (2.0-4.0) serie SP2: La corriente nominal es de 25 A.</mark>
  * <mark style="color:blue;">Sigen Hybrid (4.6-6.0) serie SP2: La corriente nominal es de 40 A.</mark>
* <mark style="color:blue;">El voltaje nominal del conmutador de CA conectado a cada</mark> <mark style="color:blue;">inversor de la serie Sigen Hybrid (3.0-12.0) TP2</mark> <mark style="color:blue;">debe ser ≥ 415 Vca y se recomienda la siguiente corriente nominal:</mark>
  * <mark style="color:blue;">Sigen Hybrid (3.0-4.0) serie TP2: La corriente nominal es de 10 A.</mark>
  * <mark style="color:blue;">Sigen Hybrid (5.0, 6.0) serie TP2: La corriente nominal es de 16 A.</mark>
  * <mark style="color:blue;">Sigen Hybrid (7.5-8.0) serie TP2: La corriente nominal es de 25 A.</mark>
  * <mark style="color:blue;">Sigen Hybrid (10.0-12.0) serie TP2: La corriente nominal es de 32 A.</mark>
* <mark style="color:blue;">Si E (panel de distribución) cuenta con protección contra fugas, se recomienda que la corriente de funcionamiento residual nominal sea mayor o igual al número de inversores x 100 mA.</mark>
* <mark style="color:blue;">El interruptor de CA del panel de distribución debe tener un voltaje nominal ≥ 240 Vca y una corriente nominal ≥ (corriente máxima de salida del inversor x número de unidades en paralelo x 1,25)</mark><sup><mark style="color:blue;">\[1]<mark style="color:blue;"></sup>
* <mark style="color:blue;">Se recomienda utilizar Fast Ethernet y WLAN para la comunicación con los inversores. Cuando el tráfico 4G gratuito de CommMod se agote, los usuarios deben ampliar sus cuentas o sustituir la tarjeta SIM.</mark>

<mark style="color:blue;">Nota \[1]: La corriente máxima de salida de un inversor se indica en la correspondiente ficha técnica.</mark>
