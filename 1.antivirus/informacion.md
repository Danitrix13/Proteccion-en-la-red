# *Modulo de antivirus*

*`Url de las paginas web que utilize en este modulo`*

1. [***av-test***](https://www.av-test.org/es/ "https://www.av-test.org/es/")

2. [***av-comparatives***](https://www.av-comparatives.org/consumer/ "https://www.av-comparatives.org/consumer/")

3. [***virustotal***](https://www.virustotal.com/gui/home/upload "https://www.virustotal.com/gui/home/upload")

4. [***hybrid-analysis***](https://www.hybrid-analysis.com/?lang=es "https://www.hybrid-analysis.com/?lang=es")

5. [***malwarebytes***](https://www.malwarebytes.com/ "https://www.malwarebytes.com/")

6. [***kaspersky***](https://www.kaspersky.es/resource-center/threats/what-is-a-security-breach "https://www.kaspersky.es/resource-center/threats/what-is-a-security-breach")

7. [***haveibeenpwned***](https://haveibeenpwned.com/ "https://haveibeenpwned.com/")

> [!IMPORTANT]
> *La pagina de Hybrid Analytics cuando hace un escaneo de los archivo que subamos luego de hacer el analisis el docuemnte lo hace publico asi que no subamos archivos confidenciales por que si no se filtra*

---

## *Configurar el programador de taresas para hacer un escaneo del dispositivo en windows*

1. [***Programar tu propio examen windows defender***](https://support.microsoft.com/es-es/topic/programar-un-examen-en-el-antivirus-de-microsoft-defender-54b64e9c-880a-c6b6-2416-0eb330ed5d2d "https://support.microsoft.com/es-es/topic/programar-un-examen-en-el-antivirus-de-microsoft-defender-54b64e9c-880a-c6b6-2416-0eb330ed5d2d")

2. [***Configurar Firewall Windows***](#configurar-firewall-windows)

# **Configurar-Firewall-Windows**

##### *Busca <kbd>*Firewall*</kbd> en la barra de busqueda de Windows luego ve a configuraciones avanzadas luego selecciones reglas de salida, crear nueva regla, darle click ala opcion del programa luego dar la ruta absoluta del programa que queremos configurar con el firewall luego segun lo que queramos hacer con el programa podemos bloquear la conexion y permitir la conexion luego configuramos para que el firewall aplique sobre esto 3 aspectos que son: Dominio, Privado, Publico, luego de eso ponerle un nombre ala regla y una breve descripcion y listo. Podemos activar y desactivar la regla cuando queramos*
---
> **Comando PowerShell:** *Set-MpPreference -DisableRemovableDriveScanning 0*

##### *El comando PowerShell "Set-MpPreference -DisableRemovableDriveScanning 0" se utiliza para habilitar el escaneo de unidades extraíbles en Windows Defender. Al establecer el valor en "0", se permite que Windows Defender escanee dispositivos de almacenamiento extraíbles como unidades flash USB, discos duros externos y tarjetas de memoria SD en busca de posibles amenazas de seguridad. Si se establece en "1", se deshabilita el escaneo de unidades extraíbles.*

<!-- - [Meta](#meta) -->

<!-- > [!NOTE]
> *La pagina*

> [!TIP]
> *La pagina*

> [!IMPORTANT]
> *La pagina*

> [!CAUTION]
> *La pagina*

> [!WARNING]
> *La pagina* -->
