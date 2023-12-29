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
