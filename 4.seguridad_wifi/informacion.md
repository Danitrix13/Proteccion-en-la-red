## ***Seguridad Wifi***

## *Indice del modulo

- [**MAC (Media Access Control) Control de acceso a los medios**](#mac-media-access-control-control-de-acceso-a-los-medios)
- [***Router-Configuracion***](#router-configuracion)

---
# **MAC (Media Access Control) Control de acceso a los medios**

![img](https://cdn.computerhoy.com/sites/navi.axelspringer.es/public/styles/480/public/media/image/2018/10/que-es-direccion-mac-tu-ordenador-movil-que-sirve.jpg?itok=R6pZrxf5 "https://cdn.computerhoy.com/sites/navi.axelspringer.es/public/styles/480/public/media/image/2018/10/que-es-direccion-mac-tu-ordenador-movil-que-sirve.jpg?itok=R6pZrxf5")

> *Las direcciones MAC (Media Access Control) son identificadores únicos asignados a las interfaces de red para dispositivos de red, como tarjetas de red y adaptadores inalámbricos. Cada dispositivo tiene una dirección MAC única, que se utiliza para identificar y comunicarse en una red.*
> [!NOTE]
> *Las direcciones MAC se representan comúnmente como una serie de caracteres hexadecimales.*

---
# ***Router-Configuracion***

**La puerta de enlace predeterminada, también conocida como gateway, es el dispositivo en una red que actúa como punto de salida para el tráfico destinado a redes fuera de la red local.**

1. ***LINUX***
   1. > *Para encontrar la puerta de enlace predeterminada en sistemas basados en Linux*

   2. ```bash
        ip route | grep default
        ```

   3. > *Para obtener información más detallada sobre la configuración de la puerta de enlace y otras rutas*

        1. ```bash
            ip route show
            ```

        2. ```bash
            ip route
            ```

2. ***WINDOWS***
    1. > *Para encontrar la puerta de enlace*

        1. ```Powershell
            ipconfig
            ```

> **Pegamos la direccion ip en el navegador en mi caso es <kbd>192.168.1.1</kbd>** nos va a pedir las credenciales como nombre y contraseña mas informacion 
[*KAON Media Model CG220*](https://portforward.com/kaon-media/passwords/ "https://portforward.com/kaon-media/passwords/").

**Despues de colocar las credenciales correctamente se nos abrira este pagina**

![*img Router Configuracion #1*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion1.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion1.png?raw=true")

> *Una vez dentro podemos configurar muchas cosas*

1. **Desactivar WPS (Wi-Fi Protected Setup)**
   1. > *WPS significa (Configuración Wi-Fi protegida, en español). es un estándar diseñado para simplificar la configuración segura de redes Wi-Fi en hogares y pequeñas empresas. Facilita la conexión de dispositivos sin ingresar manualmente la contraseña, utilizando métodos como PIN o botones físicos en el enrutador y el dispositivo. Sin embargo, WPS ha demostrado ser vulnerable a ataques de seguridad. En algunos dispositivos Xiaomi con Android 9.0 o versiones posteriores, es posible que el botón físico asociado con WPS haya sido eliminado. Dado que WPS puede representar riesgos de seguridad, algunos expertos recomiendan desactivarlo para mejorar la seguridad de la red Wi-Fi [Mas informacion]("")*

   2. ![img Router Configuracion #2](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion2.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion2.png?raw=true")

2. **Ocultar Nombre de Red (SSID) y Aislar un Access Point (AP)**
    1. > *SSID son las siglas de "Service Set Identifier" (Identificador de Conjunto de Servicios, en español). Un SSID es un nombre único que identifica a una red inalámbrica (Wi-Fi). Cada red Wi-Fi tiene un SSID único, y los dispositivos inalámbricos utilizan este nombre para conectarse a la red deseada.*

    2. > *Aislar un Access Point (AP) Punto de acceso se refiere a la configuración de la red para limitar o restringir la comunicación directa entre los dispositivos conectados a la misma red inalámbrica. En otras palabras, cuando se activa el aislamiento del AP, los dispositivos en la red no pueden comunicarse directamente entre sí, lo que añade una capa de seguridad a la red inalámbrica. Esta función también se conoce como "isolation" o "cliente aislado".*
       1. **La activación del aislamiento del AP es importante por varias razones**

          1. **Seguridad de la red:**
              1. > *Al aislar los dispositivos en una red inalámbrica, se reduce el riesgo de que un dispositivo comprometido pueda atacar directamente a otros dispositivos en la misma red. Esto es particularmente útil en entornos donde la seguridad es crítica, como en redes empresariales o en redes públicas, como las utilizadas en hoteles o cafeterías.*

          2. **Protección contra ataques internos**
               1. > *El aislamiento del AP puede proteger contra amenazas internas, donde un dispositivo malicioso intenta comprometer la seguridad de otros dispositivos en la misma red. Al limitar la comunicación directa, se reduce la superficie de ataque potencial.*

          3. **Privacidad del usuario**
               1. > *El aislamiento del AP contribuye a la privacidad de los usuarios al evitar que sus dispositivos compartan información directamente con otros dispositivos en la red. Esto puede ser especialmente relevante en redes públicas o en situaciones donde la separación de tráfico es deseable.*

          4. **Control de tráfico y rendimiento**
               1. > *El aislamiento del AP puede ayudar a optimizar el rendimiento de la red al limitar la cantidad de tráfico entre dispositivos. Esto es útil en entornos donde se busca un mejor control del tráfico para mejorar la eficiencia y la calidad de la conexión.*

    3. ![img Router Configuracion #3](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion3.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion3.png?raw=true")

3. **Crear una red de inviatdos publica**
    1. > *Crear una red de invitados pública se refiere a configurar una red inalámbrica específicamente diseñada para ofrecer acceso limitado y temporal a usuarios no autorizados o visitantes.*
       1. **Algunas características típicas de una red de invitados pública incluyen**
          1. **Acceso limitado**
             1. >*Los usuarios de la red de invitados suelen tener acceso a Internet, pero se les restringe el acceso a otros dispositivos en la red local. Esto se hace para proteger la seguridad de la red principal y la información almacenada en otros dispositivos conectados a ella.*
       2. **Contraseñas temporales**
          1. >*Para acceder a la red de invitados, se proporciona a los usuarios una contraseña temporal o un código de acceso. Esto facilita el control sobre quién puede conectarse y durante cuánto tiempo.*
       3. **Ancho de banda limitado**
          1. >*En algunos casos, se puede limitar el ancho de banda disponible para la red de invitados para asegurar que no afecte negativamente el rendimiento de la red principal.*
       4. **Aislamiento del AP**
          1. > *Puede activarse la función de aislamiento del Access Point (AP) para impedir la comunicación directa entre los dispositivos conectados a la red de invitados. Esto mejora la seguridad y la privacidad entre los usuarios temporales.*

    2. ![img Router Configuracion #4](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion4.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion4.png?raw=true")

4. **Crear una red de invitados privada**
   1. > Es el mismo procedimiento que crear una red de invitados publica exceptuando que ocultamo el SSID osea el nombre de la red*

5. **Control de acceso por filtros MAC**
   1. > *El control de acceso por filtros MAC (Media Access Control) es una función de seguridad utilizada en redes para limitar el acceso a la red inalámbrica a dispositivos específicos. Cada dispositivo con capacidad de red, como computadoras, teléfonos inteligentes o impresoras, tiene una dirección MAC única asignada a su tarjeta de red. El control de acceso por filtros MAC aprovecha estas direcciones MAC para permitir o denegar la conexión de dispositivos a una red.*

   2. ![img Router Configuracion #5](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion5.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/PNG/img-Configuracion-Router/Router-Configuracion5.png?raw=true")

6. **Control parental**
   1. > *Esta opcion te permite personalizar el tiempo en el que un dispositivo de nuestra red local puede estar conectado,que dia puede acceder al red, tambien hay una opcion la cual podemos bloquear para que no visite ciertas paginas entre otras cosas.*

   2. ![img Router Configuracion #6]("")

7. **Cambiar la contraseña**
   1. > *Podemos cambiar la contraseña del router desde la interfaz*

   2. ![img Router Configuracion #7]("")

8. *Cifrados*
   1. > *Existen muchos protocolo de seguridad*
      1. |**Algoritmo**|**Traduccion**|**Caracteristicas**|**Concepto**|
         |:---:|:---:|:-:|:-:|
         |*WEP (Wired Equivalent Privacy)*|*(Privacidad Equivalente a la de una Red Cableada)*|*Primer cifrado clave de 64 y 128 bits, cifrado RC34*|*es un protocolo de seguridad para redes inalámbricas que fue diseñado para proporcionar un nivel de seguridad similar al de las redes cableadas convencionales. Sin embargo, WEP ha quedado obsoleto y se considera inseguro debido a vulnerabilidades significativas.*|
         |*WPA (Wi-Fi Protected Access) y WPA2*|*Acceso Wi-Fi protegido*|*Clave de cifrado 128 bits, PSK, WPA -> TKIP(RC34), WPA -> (AES),Enterprise*|***WPA** fue introducido como una mejora de seguridad sobre el protocolo WEP (Wired Equivalent Privacy), que tenía importantes vulnerabilidades. WPA mejoró significativamente la seguridad mediante la implementación de un cifrado más fuerte y la introducción de funciones como TKIP (Temporal Key Integrity Protocol) para reforzar la seguridad de las claves de cifrado.**WPA2 (Wi-Fi Protected Access 2):** WPA2 es la evolución natural de WPA y representa un estándar de seguridad más avanzado. Fue introducido para abordar algunas debilidades potenciales en WPA y ofrece un cifrado más robusto mediante el uso del protocolo AES (Advanced Encryption Standard) en lugar de TKIP. WPA2 es actualmente el estándar de seguridad más ampliamente utilizado en las redes inalámbricas y se considera mucho más seguro que su predecesor*|
         |*WPA3*|*Acceso Wi-Fi protegido*|*Clave de 128 bits y 192 bits, mejora el compartir claves, Downgrade*|*WPA3 (Wi-Fi Protected Access 3) es la última iteración del protocolo de seguridad para redes inalámbricas. WPA3 fue diseñado para abordar las debilidades de seguridad conocidas en versiones anteriores como WPA y WPA2.*|

      2. **Conceptos importantes**
         1. **RC4 Rivest Cipher 4 (Cifrado Rivest 4)**
            1. *Flujo de Cifrado: RC4 es un cifrado de flujo, lo que significa que cifra los datos en tiempo real mientras se transmiten o procesan. Funciona generando una secuencia de claves de cifrado pseudoaleatorias (flujo de bits) y combinándolas con los datos originales.*

            2. Problemas de Seguridad: A lo largo de los años, se han descubierto diversas vulnerabilidades en el diseño y la implementación de RC4. Estos problemas de seguridad han llevado a que se desaconseje su uso en protocolos criptográficos modernos.

            3. *Uso en WEP y WPA: RC4 fue utilizado inicialmente en el protocolo de seguridad WEP (Wired Equivalent Privacy) para proteger las comunicaciones en redes inalámbricas. Sin embargo, WEP resultó ser vulnerable y fue reemplazado por protocolos más seguros como WPA y WPA2.*
            4. *Ataques WEP y RC4: En el contexto de WEP, se descubrieron ataques específicos, como el ataque Fluhrer-Mantin-Shamir (FMS), que explotaban debilidades en la implementación de RC4. Esto contribuyó al declive de la popularidad de WEP y RC4 en entornos de redes inalámbricas.*

         2. **PSK**
            1. *PSK significa "Pre-Shared Key" en inglés, y su traducción al español es "Clave Precompartida"*

            2. *La idea básica es que tanto el punto de acceso como los dispositivos clientes comparten una clave secreta común, la cual se utiliza para autenticar y cifrar las comunicaciones entre ellos. Esta clave precompartida es ingresada manualmente en los dispositivos clientes y en el punto de acceso. Por lo general, se presenta como una contraseña o clave de acceso al conectarse a la red inalámbrica.*

         3. **Enterprise**
            1. *Enterprise emplea la autenticación basada en un servidor RADIUS (Remote Authentication Dial-In User Service) Servicio de Usuario de Marcación de Autenticación Remota.*

            2. ***EAP** (Extensible Authentication Protocol): WPA2-Enterprise utiliza EAP, que es un marco de autenticación extensible, para establecer la conexión segura entre dispositivos y puntos de acceso.*

            3. **Servidor RADIUS:** En lugar de depender de una clave precompartida, WPA2-Enterprise utiliza un servidor RADIUS para gestionar y autenticar usuarios. El servidor RADIUS almacena la información de autenticación y verifica las credenciales de los usuarios que intentan conectarse a la red.
         4. **TKIP -> WPA**
            1. *TKIP significa "Temporal Key Integrity Protocol" en inglés, y su traducción al español sería "Protocolo Temporal de Integridad de Clave".*

            2. *Dinamismo de las Claves: TKIP utiliza claves temporales y dinámicas en lugar de claves estáticas, como las utilizadas en WEP. Esto significa que las claves cambian con el tiempo, lo que hace más difícil para los atacantes predecir y descifrar las comunicaciones.*

            3. *Integridad del Paquete: TKIP proporciona integridad de paquetes, lo que significa que puede detectar si los datos han sido manipulados durante la transmisión. Si se detecta algún intento de alteración, el paquete se descarta, mejorando la seguridad de las comunicaciones.*

            4. *Utilización de un Vector de Inicialización (IV) Más Largo: TKIP utiliza un vector de inicialización más largo que WEP, lo que reduce las posibilidades de ciertos tipos de ataques criptoanalíticos.*

         5. **AES -> WPA2**
            1. *AES significa "Advanced Encryption Standard" en inglés y su traducción al español sería "Estándar de Cifrado Avanzado". AES es un algoritmo de cifrado simétrico*

            2. *Bloques y Claves: AES opera en bloques de datos y utiliza claves de cifrado simétrico. Los tamaños de bloque y las longitudes de clave pueden ser de 128, 192 o 256 bits.*

            3. *Estructura Ronda: AES utiliza un diseño de rondas para realizar la cifra. La cantidad de rondas depende de la longitud de la clave: 10 rondas para claves de 128 bits, 12 rondas para claves de 192 bits y 14 rondas para claves de 256 bits.*

            4. *Confidencialidad y Seguridad: AES es altamente resistente a diversos ataques criptoanalíticos y se considera seguro para proteger información clasificada a nivel gubernamental.*

            5. *Eficiencia en Hardware y Software: AES ha sido diseñado para ser eficiente tanto en implementaciones de hardware como en software, lo que facilita su implementación en una variedad de dispositivos.*

            6. *Amplia Adopción: AES es ampliamente utilizado y es el estándar de cifrado preferido en una variedad de aplicaciones, desde la seguridad de Wi-Fi (WPA2 y WPA3) hasta el cifrado de datos en sistemas operativos y aplicaciones.*

         6. *El término "downgrade" en el contexto de redes inalámbricas se refiere a cambiar la seguridad de una red de un protocolo más seguro a uno menos seguro.*