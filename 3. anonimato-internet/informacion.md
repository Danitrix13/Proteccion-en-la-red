***Anonimato en la red***

- [***Email-Temporales***](#email-temporales)
- [***Protonmail***](#protonmail)
- [***HTTP-HTTPS***](#http-https)
- [***Herramientas SSLSCAN y TESTSSL.SH***](#herramientas-sslscan-y-testsslsh)
- [***Configuraciones segura para navegador Firefox***](#configuraciones-segura-para-navegador-firefox)
- [***Configuraciones segura para navegador Chrome***](#configuraciones-segura-para-navegador-chrome)
- [***Motor de busqueda DuckDuckGo***](#motor-de-busqueda-duckduckgo)
- [***Configuraciones segura para navegador Brave***](#configuraciones-segura-para-navegador-brave)

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

**`SSL y TLS son protocolos de seguridad utilizados en la comunicación de red.`**

> **SSL:** *significa Secure Sockets Layer. Es un protocolo de seguridad que se utiliza para establecer enlaces cifrados entre un servidor web y un navegador. Este enlace asegura que todos los datos transmitidos entre el servidor web y el navegador permanezcan privados y seguros. SSL es ampliamente utilizado para proteger las transacciones en línea y para asegurar la transmisión de información confidencial, como los detalles de la tarjeta de crédito durante las transacciones en línea.*
___
> **TLS:** *significa Transport Layer Security. Es un protocolo que proporciona privacidad y seguridad de datos entre dos aplicaciones que se comunican a través de una red. TLS es el sucesor de Secure Sockets Layer (SSL). Se utiliza comúnmente para proteger las comunicaciones web (HTTP/HTTPS), el correo electrónico (SMTP), la mensajería instantánea (IM) y algunas VPNs.*

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

*Al analizar la pagina es recomendable que el `TLS` tengo solo habilitada la version 1.2 y 1.3 **Enabled** y desactivada la version 1.1 y 1.0 **Disabled*** simplemente es mas seguro.

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

![configuracion chrome img #1](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome1.png?raw=true)

![configuracion chrome img #2](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome2.png?raw=true)

![configuracion chrome img #3](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome3.png?raw=true)

![configuracion chrome img #4](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome4.png?raw=true)

![configuracion chrome img #5](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome5.png?raw=true)

![configuracion chrome img #6](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome6.png?raw=true)

![configuracion chrome img #7](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome7.png?raw=true)

![configuracion chrome img #8](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome8.png?raw=true)

![configuracion chrome img #9](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome9.png?raw=true)

![configuracion chrome img #10](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome10.png?raw=true)

![configuracion chrome img #11](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome11.png?raw=true)

![configuracion chrome img #12](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img-chrome/Configuracion%20Chrome12.png?raw=true)

---
<!-- [^3]:Motor de busqueda DuckDuckGo -->

# ***Motor de busqueda DuckDuckGo***

> *DuckDuckGo es un motor de búsqueda en línea que se centra en la privacidad del usuario y en no rastrear la información personal durante las búsquedas. Fue lanzado en 2008 con el objetivo de proporcionar una alternativa a los motores de búsqueda más convencionales que a menudo recopilan datos sobre los usuarios para personalizar los resultados y la publicidad.

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

1. [Cookie editor Mozilla](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/ "https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/")
2. [Cookie editor Brave](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg "https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg")

> [!TIP]
> ***Las cookies pueden utilizarse para iniciar sesión en una página web. Esto se puede lograr de varias formas, una de ellas es mediante el uso de una extensión que importe y exporte cookies en formato JSON, permitiendo que la página acceda a los datos necesarios para el inicio de sesión.***

<!-- criptomineros es un malware que se instala en tu navegador y que consume recurso y lo utiliza para minar criptomoneas haciendo que el ordenador este lente -->

<!-- fingerprinters -->
