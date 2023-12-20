***Anonimato en la red***

- [***Email-Temporales***](#email-temporales)
- [***Protonmail***](#protonmail)
- [***HTTP-HTTPS***](#http-https)
- [***Herramientas SSLSCAN y TESTSSL.SH***](#herramientas-sslscan-y-testsslsh)
- [***Configuraciones segura para navegadores***](#configuraciones-segura-para-navegadores)
  - [\[^4\]:Configuraciones personales](#4configuraciones-personales)

[***HTTP VS HTTPS***](#http-vs-https)

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

![*Img*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img1.png?raw=true)

![*Img dos*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img2.png?raw=true)

![*Img tres*](https://github.com/Danitrix13/Proteccion-en-la-red/blob/master/img/img3.png?raw=true)

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

# ***Configuraciones segura para navegadores***

1. **Firefox** [^1]
2. **Chrome** [^2]
3. **Motor de busqueda DuckDuckGo** [^3]
4. **Brave** [^4]

[^1]:Configuraciones del navegador Firefox

[^2]:Configuraciones del navegador Chrome

[^3]:DuckDuckGo

[^4]:Configuraciones personales
---

>*Extensiones para el navegador*

1. [Cookie editor Mozilla](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/ "https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/")
2. [Cookie editor Brave](https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg "https://chromewebstore.google.com/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg")

<!-- criptomineros es un malware que se instala en tu navegador y que consume recurso y lo utiliza para minar criptomoneas haciendo que el ordenador este lente -->

<!-- fingerprinters -->
