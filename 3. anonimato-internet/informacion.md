***Anonimato en la red***

- [***Email-Temporales***](#email-temporales)
- [***Protonmail***](#protonmail)
- [***HTTP-HTTPS***](#http-https)
- [***Herramientas SSLSCAN y TESTSSL.SH***](#herramientas-sslscan-y-testsslsh)
- [***Configuraciones segura para navegador Firefox***](#configuraciones-segura-para-navegador-firefox)
- [***Configuraciones segura para navegador Chrome***](#configuraciones-segura-para-navegador-chrome)
- [***Motor de busqueda DuckDuckGo***](#motor-de-busqueda-duckduckgo)
- [***Configuraciones segura para navegador Brave***](#configuraciones-segura-para-navegador-brave)
- [***IP-Publica***](#ip-publica)
- [***IP-Privada***](#ip-privada)
- [***The Onion Router (TOR)***](#the-onion-router-tor)

---

# ***Email-Temporales***

> *Los correos temporales, también conocidos como correos desechables o temporales, son direcciones de correo electrónico que se crean para un solo uso y luego se eliminan automáticamente. Se utilizan a menudo para registrarse en sitios web o servicios que no requieren una dirección de correo electrónico permanente, o para proteger la privacidad al evitar que los correos electrónicos personales sean rastreados o recogidos por terceros.*

**Paginas web que brindan este servicio**

- [*temp-mail.io*](https://temp-mail.io/en "https://temp-mail.io/en")
- [*temp-mail.org*](https://temp-mail.org/en/ "https://temp-mail.org/en/")

# ***Protonmail***

> *ProtonMail es un servicio de correo electrónico seguro con sede en Suiza. Fue fundado en 2013 por un grupo de científicos del CERN, entre ellos Andy Yen, Jason Stockman y Wei Sun. ProtonMail se basa en el cifrado de extremo a extremo, lo que significa que los mensajes se cifran antes de salir del dispositivo del remitente y solo se pueden descifrar en el dispositivo del destinatario. Esto hace que ProtonMail sea una opción muy segura para enviar y recibir correos electrónicos confidenciales.*

- [*Web de protonmail*](https://proton.me/mail "https://proton.me/mail")

> [!NOTE]
> *Tambien tiene aplicaciones tanto para desktop como para moviles*

---

# ***HTTP-HTTPS***

> **HTTP:** *significa Protocolo de Transferencia de Hipertexto (Hypertext Transfer Protocol en inglés). Es el protocolo de comunicación que permite las transferencias de información en la web. HTTP define cómo se transmiten los mensajes a través de la web y qué acciones pueden tomar los navegadores web y los servidores web al hacer una solicitud o dar una respuesta. Por ejemplo, cuando escribes una URL en tu navegador, en realidad estás enviando una solicitud HTTP al servidor donde se encuentra la página web. El servidor responde con el contenido de la página. Es importante notar que HTTP no es seguro, ya que los datos se transmiten en texto plano, lo que significa que si alguien intercepta la comunicación, puede leer la información. Para solucionar este problema, se utiliza HTTPS (HTTP Seguro), que cifra los datos transmitidos.*
---
> **HTTPS:** *significa Protocolo seguro de transferencia de hipertexto (Hypertext Transfer Protocol Secure en inglés). Es la versión segura de HTTP. HTTPS utiliza un protocolo de seguridad llamado SSL/TLS para cifrar la información que se envía entre el cliente (por ejemplo, tu navegador) y el servidor. Esto significa que incluso si alguien intercepta los datos que se están transmitiendo, no podrá leerlos porque están cifrados. El uso de HTTPS es especialmente importante cuando se transmiten datos sensibles, como contraseñas o información de tarjetas de crédito.*
---
> **Puertos de HTTP y HTTPS:** *HTTP y HTTPS utilizan diferentes puertos por defecto. HTTP utiliza el puerto 80, mientras que HTTPS utiliza el puerto 443. Estos son los puertos predeterminados, pero se pueden configurar para usar otros puertos si es necesario.*

![*Img*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-HTTP-VS-HTTPS/HTTP%20VS%20HTTPS1.png?raw=true)

![*Img dos*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-HTTP-VS-HTTPS/HTTP%20VS%20HTTPS2.png?raw=true)

![*Img tres*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-HTTP-VS-HTTPS/HTTP%20VS%20HTTPS3.png?raw=true)

**`SSL y TLS  a veces denominados «certificados digitales», se utilizan para establecer una conexión cifrada entre un navegador o el ordenador de un usuario y un servidor o un sitio web. Son protocolos de seguridad utilizados en la comunicación de red.`**

> **SSL:** *Significa Secure Sockets Layer (Capa de sockets seguros).SSL es una tecnología estandarizada que permite cifrar el tráfico de datos entre un navegador web y un sitio web (o entre dos servidores web), protegiendo así la conexión. Esto impide que un hacker pueda ver o interceptar la información que se transmite de un punto a otro, la cual puede contener datos personales o financieros.*
___
> **TLS:** *Significa Transport Layer Security (Seguridad de la capa de transporte). TLS es una versión actualizada y más segura de SSL. Es un protocolo que proporciona privacidad y seguridad de datos entre dos aplicaciones que se comunican a través de una red. TLS es el sucesor de Secure Sockets Layer (SSL). Se utiliza comúnmente para proteger las comunicaciones web (HTTP/HTTPS), el correo electrónico (SMTP), la mensajería instantánea (IM) y algunas VPNs.*

# ***Herramientas SSLSCAN y TESTSSL.SH***

> *SSLScan es una herramienta de código abierto diseñada para analizar la configuración de seguridad de servidores que utilizan el protocolo SSL/TLS. Esta herramienta escanea un servidor en busca de configuraciones débiles o vulnerabilidades relacionadas con SSL/TLS. Proporciona información detallada sobre la suite de cifrado utilizada, versiones de protocolos SSL/TLS admitidas, configuraciones de cifrado débiles y posibles amenazas a la seguridad. SSLScan se utiliza comúnmente para evaluar la seguridad de servidores web y asegurarse de que estén configurados de manera segura para proteger la comunicación en línea. Al analizar la configuración SSL/TLS de un servidor, los administradores pueden identificar y corregir posibles vulnerabilidades antes de que sean explotadas por posibles atacantes.*

**Para instalar Sslscan en Ubuntu**

1. Abrimos la terminal con <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>t</kbd>

2. *Actualizamos los paquetes*

    ```bash
    sudo apt-get update
    ```

3. *Comando para instalar sslscan*

    ```bash
    sudo apt-get install sslscan
    ```

4. *Comprobamos la version*

    ```bash
    sslscan --version
    ```

5. Analizamos el sitio web < Sitio Web > esto remplazar por la url de la web

    ```bash
    sslscan <Sitio Web>
    ```

> [!IMPORTANT]
> *Al analizar la pagina es recomendable que el `TLS` tengo solo habilitada la version 1.2 y 1.3 **Enabled** y desactivada la version 1.1 y 1.0 **Disabled*** simplemente es mas seguro.

**Segunda Herrmienta para el analizis de paginas web para usar este herramienta tendremos que descargarnos el repositorio de github**

1. ```bash
    git clone git@github.com:drwetter/testssl.sh.git
    ```

2. ```bash
    cd testssl.sh/
    ```

3. ```bash
    ./testssl.sh <Sitio Web>
    ```

---

# ***Configuraciones segura para navegador Firefox***

<!-- 1. **Firefox** [^1] -->
<!-- 2. **Chrome** [^2] -->
<!-- 3. **Motor de busqueda DuckDuckGo** [^3] -->
<!-- 4. **Brave** [^4] -->

<!-- [^1]:Configuraciones del navegador Firefox -->

![configuracion Firefox img #1](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox1.png?raw=true)

![configuracion Firefox img #2](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox2.png?raw=true)

![configuracion Firefox img #3](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox3.png?raw=true)

![configuracion Firefox img #4](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox4.png?raw=true)

![configuracion Firefox img #5](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox5.png?raw=true)

![configuracion Firefox img #6](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox6.png?raw=true)

![configuracion Firefox img #7](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox7.png?raw=true)

![configuracion Firefox img #8](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-firefox/configuracion%20firefox8.png?raw=true)

---

# ***Configuraciones segura para navegador Chrome***
<!-- [^2]:Configuraciones del navegador Chrome -->

![configuracion Chrome img #1](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome1.png?raw=true)

![configuracion Chrome img #2](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome2.png?raw=true)

![configuracion Chrome img #3](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome3.png?raw=true)

![configuracion Chrome img #4](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome4.png?raw=true)

![configuracion Chrome img #5](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome5.png?raw=true)

![configuracion Chrome img #6](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome6.png?raw=true)

![configuracion Chrome img #7](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome7.png?raw=true)

![configuracion Chrome img #8](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome8.png?raw=true)

![configuracion Chrome img #9](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome9.png?raw=true)

![configuracion Chrome img #10](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome10.png?raw=true)

![configuracion Chrome img #11](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome11.png?raw=true)

![configuracion Chrome img #12](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome12.png?raw=true)

---
<!-- [^3]:Motor de busqueda DuckDuckGo -->

# ***Motor de busqueda DuckDuckGo***

> *DuckDuckGo es un motor de búsqueda en línea que se centra en la privacidad del usuario y en no rastrear la información personal durante las búsquedas. Fue lanzado en 2008 con el objetivo de proporcionar una alternativa a los motores de búsqueda más convencionales que a menudo recopilan datos sobre los usuarios para personalizar los resultados y la publicidad.*

**Las principales características de DuckDuckGo incluyen:**

1. **Privacidad:**
   > *DuckDuckGo se compromete a no recopilar información personal del usuario. No almacena direcciones IP, no realiza un seguimiento de las búsquedas del usuario y no utiliza cookies persistentes.*

2. **Resultados imparciales:**
   > *A diferencia de algunos motores de búsqueda que personalizan los resultados según el historial de búsqueda del usuario, DuckDuckGo proporciona resultados objetivos y no sesgados para todos los usuarios.*

3. **Búsquedas encriptadas:**
   > *DuckDuckGo utiliza conexiones encriptadas (HTTPS) para proteger la privacidad del usuario durante las búsquedas.*

4. **Sin burbuja de filtro:**
   > *DuckDuckGo intenta evitar la "burbuja de filtro", que es la personalización extrema de los resultados basada en la información personal del usuario, permitiendo así una experiencia de búsqueda más diversa.*

*En navegadores como brave el motor de busqueda <kbd>**DuckDuckgo**</kbd> esta instalado solo hay que configurarlo como motor de busqueda predeterminado*

*En navegadores como Firefox o Chrome tenemos que instalar una extension*

1. [<kbd>**DuckDuckgo Firefox extension**</kbd>](https://addons.mozilla.org/es/firefox/addon/duckduckgo-for-firefox/ "https://addons.mozilla.org/es/firefox/addon/duckduckgo-for-firefox/")
2. [<kbd>**DuckDuckgo Chrome extension**</kbd>](https://chrome.google.com/webstore/detail/duckduckgo-privacy-essent/bkdgflcldnnnapblkhphbgpggdiikppg "https://chrome.google.com/webstore/detail/duckduckgo-privacy-essent/bkdgflcldnnnapblkhphbgpggdiikppg")

---

# ***Configuraciones segura para navegador Brave***
<!-- [^4]:Configuraciones del navegador Brave -->

>*Extensiones para el navegador*

![configuracion Brave img #1](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave1.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave1.png?raw=true")

![configuracion Brave img #2](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave2.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave2.png?raw=true")

![configuracion Brave img #3](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave3.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave3.png?raw=true")

![configuracion Brave img #4](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave4.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave4.png?raw=true")

![configuracion Brave img #5](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave5.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave5.png?raw=true")

![configuracion Brave img #6](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave6.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave6.png?raw=true")

![configuracion Brave img #7](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave7.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave7.png?raw=true")

![configuracion Brave img #8](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave8.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave8.png?raw=true")

![configuracion Brave img #9](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave9.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave9.png?raw=true")

![configuracion Brave img #10](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave10.png?raw=true "https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-brave/Configuracion%20Brave10.png?raw=true")

1. [Cookie editor Mozilla](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/ "https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/")
2. [Cookie editor Brave](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg "https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg")

> [!TIP]
> ***Las cookies pueden utilizarse para iniciar sesión en una página web. Esto se puede lograr de varias formas, una de ellas es mediante el uso de una extensión que importe y exporte cookies en formato JSON, permitiendo que la página acceda a los datos necesarios para el inicio de sesión.***

---

# ***IP-Publica***
>
> **Dirección IP Pública:** *La dirección IP pública es la dirección única asignada a tu red desde el proveedor de servicios de Internet (ISP). Es la dirección que se utiliza para identificar tu red en Internet. Todas las dispositivos conectados a Internet desde tu red doméstica compartirán la misma dirección IP pública. Esta dirección es necesaria para que los dispositivos se comuniquen con otros dispositivos en Internet. Puedes obtener tu dirección IP pública utilizando servicios en línea o comandos específicos en la terminal.*

1. *Puedes utilizar servicios en línea para obtener tu IP pública. Uno de los servicios comunes es curl para obtener la IP desde un sitio web comando en **Ubuntu es:***

   1. ```bash
        curl ifconfig.me
        ```

   2. ```bash
        curl ifconfig.me/ip
        ```

   3. ```bash
        dig +short myip.opendns.com @resolver1.opendns.com
        ```

2. *Otra opcion seria visitar cualquiera de esta paginas ya que nos brindara nuestra ip publica*

    1. [*IP publica pagina #1*](https://ip-lookup.live/ "https://ip-lookup.live/")
    2. [*IP publica pagina #2*](https://www.cual-es-mi-ip.net/ "https://www.cual-es-mi-ip.net/")
3. **En windows abrimos el cmd con <kbd>Windows</kbd>+<kbd>r</kbd> escribimos cmd**

    1. ```cmd
        nslookup myip.opendns.com resolver1.opendns.com
        ```

---

# ***IP-Privada***

> **Dirección IP Privada:** *La dirección IP privada es la dirección asignada a un dispositivo dentro de una red local (como tu red doméstica o de oficina). Está diseñada para ser única dentro de esa red local. Puedes tener múltiples dispositivos con la misma dirección IP privada en diferentes redes locales, ya que no son únicas en todo Internet. Los routers en la red local asignan direcciones IP privadas a los dispositivos conectados. Las direcciones IP privadas están reservadas y definidas en los rangos específicos, como 192.168.x.x, 10.x.x.x, etc.*

1. *Comandos para obtener las ip privadas de nuestra red en ubuntu cualquiera de las dos podemos usar*

    1. ```bash
        ip a
        ```

    2. ```bash
        ip addr show
        ```

2. *Comando para obtener ip privada de una interfaz especifica en ubuntu remplaza **enp0s3** por la interfaz que quieres monitorear*

   ```bash
   ip addr show <enp0s3>
   ```

3. **En windows abrimos el cmd con <kbd>Windows</kbd>+<kbd>r</kbd> escribimos cmd**

    1. ```cmd
        ipconfig
        ```

**Estructuras de las direcciones ip**

|**Datos**| **IPV4** |**IPV6**|
|:-------:|:------:|:---:|
|**Bits**| *Utiliza direcciones de 32 bits* | utiliza direcciones de 128 bits|
|**Rango de números**|*Va desde 0.0.0.0 hasta 255.255.255.255.*| *Dada la longitud de 128 bits, el rango es enormemente grande, proporcionando un número prácticamente ilimitado de direcciones únicas*|
|**Significado de cada sección**| *Cada sección, separada por puntos, representa un octeto (8 bits) de la dirección. Por ejemplo, en la dirección "192.168.1.1", 192 es el primer octeto, 168 es el segundo, 1 es el tercer y 1 es el cuarto.*|*En lugar de puntos, IPv6 utiliza dos puntos para separar las secciones. Cada sección de 16 bits se representa en notación hexadecimal. Por ejemplo, una dirección IPv6 podría verse así: 2001:0db8:85a3:0000:0000:8a2e:0370:7334.*|

**Datos sobre las direcciones IP**
1. Siglas IP. Internet Protocol (Protocolo de Internet)

Las direcciones IP (Protocolo de Internet) son asignadas y gestionadas por organizaciones específicas a nivel mundial. 

Las direcciones IP públicas son asignadas por organizaciones globales (ICANN y RIR), mientras que las direcciones IP privadas son gestionadas por IANA y se utilizan internamente en redes privadas. Las empresas, proveedores de servicios de Internet (ISP) y otras organizaciones obtienen bloques de direcciones IP públicas a través de los RIR.

---
# ***The Onion Router (TOR)***

> **TOR** *(El Enrutador Cebolla, en español), es un sistema de red anónima diseñado para mejorar la privacidad y seguridad en línea al enrutar el tráfico a través de una serie de servidores distribuidos en todo el mundo. El nombre "cebolla" se refiere a la estructura de capas del sistema, ya que el tráfico se cifra y reenruta a través de múltiples nodos, como las capas de una cebolla.*

1. **Nodos Tor**
   1. **Nodos de Entrada (Entry Nodes):** *El nodo de entrada es el primer nodo en un circuito Tor. Cuando un usuario inicia una conexión Tor, elige aleatoriamente un nodo de entrada.  El tráfico entra en la red a     través de un nodo de entrada. El nodo de entrada sabe la dirección IP del usuario, pero no conoce la identidad del usuario ni su destino final.La comunicación entre el usuario y el nodo de entrada está cifrada mediante el uso de claves asimétricas.*

   2. **Nodos Intermedios (Intermediate Nodes):** *Los  nodos intermedios reciben datos cifrados del nodo de entrada y los envían al siguiente nodo en el circuito.
    Cada nodo intermedio solo conoce el nodo anterior y el siguiente en la cadena, lo que contribuye a la anonimización del tráfico. El tráfico entre nodos intermedios también está cifrado de extremo a extremo*
  
   3. **Nodos de Salida (Exit Nodes):** *El tráfico finalmente sale de la red Tor a través de un nodo de salida, que es consciente del destino final pero no de la identidad del usuario.*

   4. **Circuitos Dinámicos**
        1. **Establecimiento de Circuitos**
            1. *Cuando un usuario inicia una conexión a través de Tor, el software cliente selecciona aleatoriamente una secuencia de nodos (nodo de entrada, nodos intermedios y nodo de salida) para formar un circuito.*
            2. *El usuario y el nodo de entrada establecen una conexión cifrada mediante el uso de claves asimétricas para proteger la comunicación.*
        2. **Duración del Circuito**
            1. *Los circuitos en Tor no son estáticos; en cambio, son circuitos temporales que pueden cambiar a lo largo del tiempo.*
            2. *El tiempo de vida de un circuito se especifica al establecerse y puede ser reconfigurado para mejorar la seguridad y la privacidad.*
        3. **Renovación del Circuito:**
           1. *Tor renueva automáticamente los circuitos en intervalos regulares, lo que significa que el usuario puede estar utilizando diferentes nodos para diferentes partes de su actividad en línea.*
           2. *La renovación frecuente de circuitos dificulta la correlación de tráfico y mejora la seguridad contra ciertos tipos de ataques.*
        4. **Selección Aleatoria de Nodos**
           1. *La selección de nodos para formar circuitos es aleatoria, y Tor intenta distribuir la carga de manera equitativa entre los nodos disponibles.*
           2. *La aleatoriedad en la selección contribuye a la resistencia contra ataques de seguimiento y correlación.*
        5. **Circuitos Múltiples**
           1. *Tor permite que un usuario mantenga múltiples circuitos abiertos simultáneamente.*
           2. *Cada circuito puede utilizarse para una conexión diferente, y la variedad de circuitos aumenta la complejidad para aquellos que intentan rastrear o correlacionar el tráfico.*
        6. **Prevención de Ataques de Correlación**
           1. *Los circuitos dinámicos se utilizan para prevenir ataques de correlación, donde un adversario podría observar patrones de tráfico en los nodos de entrada y salida para intentar identificar a un usuario.*
        7. **Uso de Túneles TLS/SSL**
           1. *Dentro de un circuito, la comunicación entre nodos se realiza mediante túneles TLS/SSL, lo que garantiza la confidencialidad y la integridad de los datos.*

   5. **Selección Aleatoria de Nodos**
        1. *La selección de nodos Tor se realiza de forma aleatoria, lo que dificulta la correlación entre el usuario y su tráfico.*
        2. *La aleatoriedad en la selección de nodos contribuye a la resistencia contra ataques de correlación y seguimiento.*
   6. **Política de No Registro (No Logging)**
      1. *Los nodos Tor no registran información sobre las conexiones. Cada conexión es independiente de las anteriores, mejorando la privacidad del usuario*
   7. **Seguridad contra Ataques**
        1. *Los nodos Tor implementan medidas de seguridad para resistir ataques, como ataques de denegación de servicio (DoS) y ataques que intentan comprometer la identidad de los usuarios.*
   8. **Protección contra Ataques de Correlación**
       1. *Tor utiliza técnicas como la introducción de retardos aleatorios en la transmisión de datos para dificultar la correlación de patrones de tráfico.*

2. **Cifrado de Capas**
   1. *Cada nodo en la cadena descifra solo la capa externa del cifrado, revelando el próximo nodo al que debe enviarse el tráfico.*

   2. *Esto se repite a través de varios nodos, creando múltiples capas de cifrado que se van descifrando secuencialmente.*

3. **Protocolo de Comunicación**
   1. **Protocolo de Enrutamiento Onion (OR)**
      1. *Tor utiliza un protocolo de enrutamiento específico llamado "Protocolo de Enrutamiento Onion" (OR Protocol).*
      2. *Este protocolo se encarga de manejar la formación de circuitos anónimos y la transmisión de datos a través de estos circuitos.*
   2. **Handshake de Claves Asimétricas**
       1. **Claves Asimétricas**
          1. *Tor utiliza un sistema de criptografía de clave pública, que implica el uso de pares de claves asimétricas. **Cada nodo tiene un par de claves: una clave privada y una clave pública.***
          2. *La clave privada se mantiene en secreto y se utiliza para descifrar la información cifrada con la clave pública asociada.*

       2. **Cifrado de Sesión**
          1. *Cuando se establece un circuito en Tor, los nodos negocian claves de sesión para esa conexión específica.*
          2. *Las claves de sesión se utilizan para cifrar y descifrar la información transmitida entre nodos a lo largo del circuito.*
       3. **Protocolo de Handshake (Apretón de manos)**
          1. El proceso de "Handshake de Claves Asimétricas" comienza cuando un nodo desea establecer una conexión con otro nodo.
          2. *Durante el handshake, los nodos intercambian información sobre sus capacidades de cifrado y acuerdan sobre el algoritmo de cifrado y las claves de sesión a utilizar.*
       4. **Autenticación Mutua**
          1. *La criptografía de clave pública permite la autenticación mutua entre nodos.*
          2. *Cada nodo puede verificar la identidad del otro nodo utilizando la clave pública del par de claves asimétricas del otro.*
       5. **Perfect Forward Secrecy**
          1. *Tor implementa el concepto de "Perfect Forward Secrecy" (PFS), lo que significa que, incluso si una clave privada se ve comprometida en el futuro, las comunicaciones pasadas seguirán siendo seguras.*
          2. *Esto se logra mediante la generación de claves de sesión únicas para cada conexión.*
       6. **Algoritmos de Cifrado**
          1. *Tor admite diversos algoritmos criptográficos, como AES (Advanced Encryption Standard) para cifrado simétrico y RSA (Rivest-Shamir-Adleman) y ECC (Elliptic Curve Cryptography) para cifrado asimétrico.*
       7. **Protección contra Ataques Man-in-the-Middle (MitM)**
          1. *El proceso de handshake ayuda a proteger contra ataques de Man-in-the-Middle, ya que un atacante no puede fácilmente falsificar la autenticación de los nodos sin conocer las claves privadas asociadas.*
       8. **Renegociación de Claves**
          1. *A lo largo de la duración de la conexión, los nodos pueden renegociar las claves de sesión para mejorar la seguridad y la resistencia contra amenazas.*

   3. **Cifrado de Extremo a Extremo**
       1. *Los datos transmitidos a través de la red Tor están cifrados de extremo a extremo entre los nodos que forman parte de un circuito.*
       2. *Cada nodo solo puede descifrar la capa de cifrado que le corresponde, manteniendo así la confidencialidad del tráfico.*
   4. **Control de Flujo de Datos**
      1. *El protocolo Tor incluye mecanismos para controlar el flujo de datos y gestionar la congestión en la red.*
      2. *Se implementan técnicas para evitar ataques de denegación de servicio y garantizar un funcionamiento eficiente.*

4. **Enrutamiento Aleatorio:**

   1. *La ruta exacta que toma el tráfico a través de los nodos Tor es seleccionada de forma aleatoria, lo que dificulta la correlación entre el usuario y el destino.*

5. **Acceso a la Dark Web:**

   1. *Tor permite acceder a sitios web con el dominio ".onion" que no son accesibles a través de la **Surface Web** o **web superficial**. Estos sitios a menudo se asocian con la Dark Web.*

***Nodo***
> *En el contexto de las redes, un nodo generalmente se refiere a cualquier dispositivo que forma parte de la red y tiene una dirección única en esa red. Puede ser una computadora, un enrutador, un conmutador u otro dispositivo de red. En el caso específico de la red Tor, se utilizan los términos "nodos" para referirse a los puntos de retransmisión a través de los cuales se enruta el tráfico.*

***Host***
> *Un host es un dispositivo específico, como una computadora o un servidor, que tiene una dirección única en una red. Un host puede ser un nodo, pero no todos los nodos son necesariamente hosts. Por ejemplo, un enrutador puede ser un nodo de la red, pero no es un host en el sentido de ser una estación de trabajo o servidor final.*
> **En resumen, todos los hosts son nodos, pero no todos los nodos son hosts. En la red Tor, los nodos se refieren específicamente a los puntos de retransmisión que forman parte de la red anónima, mientras que los hosts pueden referirse a dispositivos finales que están conectados a la red.**

***Enrutamiento***
> *El enrutamiento se refiere al proceso de dirigir el tráfico de datos desde el origen hasta el destino a través de una red de dispositivos intermedios llamados routers. Los routers toman decisiones sobre cómo enviar los datos basándose en la dirección de destino de los paquetes de datos. Este proceso se realiza para optimizar la eficiencia y la entrega de los datos.*

***Cifrado***
> *El cifrado es el proceso de convertir datos en un formato ilegible (cifrado) utilizando un algoritmo y una clave. La intención es proteger la información de accesos no autorizados. Solo aquellos que posean la clave adecuada podrán descifrar y comprender los datos originales. El cifrado se utiliza para garantizar la confidencialidad de la información.*

***Encriptación***
> *La encriptación es un término que se utiliza de manera intercambiable con el cifrado en muchos contextos. Ambos términos se refieren al mismo concepto de convertir información en un formato cifrado. En general, cuando se habla de comunicaciones seguras en la web, se hace referencia al uso de protocolos como SSL/TLS, que proporcionan tanto cifrado como autenticación.*

<!-- Puedes ajustar la alineación de las celdas utilizando dos puntos (:) dentro de las barras verticales. Por ejemplo, |:--|:--:|--:| alinea las celdas a la izquierda, al centro y a la derecha respectivamente. -->

<!-- criptomineros es un malware que se instala en tu navegador y que consume recurso y lo utiliza para minar criptomoneas haciendo que el ordenador este lente -->

<!-- fingerprinters -->
