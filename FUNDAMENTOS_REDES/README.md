**98 Bienvenido al primer escalón de la anticipación de amenazas cibernéticas.**

 Para anticiparse a las amenazas, no basta con entender el terreno de juego; hay que saber cómo mover las piezas, tender emboscadas y, sobre todo, anticipar los movimientos del adversario. Aquí tienes tu manual esencial de redes, ahora con enfoque ofensivo y defensivo.

---

## 1. ¿Qué es una Red? La topografía del campo de batalla

En términos simples, una red es un conjunto de dispositivos interconectados. Pero para un Red Team, la red es un **sistema circulatorio** que puede ser pinzado, redirigido o drenado. Cada dispositivo, cada cable, cada onda de radio es un posible punto de entrada o exfiltración.

![](osi.png)

### Tipos de Redes según su alcance (y cómo atacarlas)

* **LAN (Local Area Network):** Una red pequeña, como tu casa o una oficina.  
  * **Enfoque Red Team:** Aquí se realizan ataques de **ARP spoofing**, **DNS poisoning** y **escaneo de puertos** para moverse lateralmente. La cercanía física (o acceso a la red cableada/Wi-Fi) es clave.

* **WAN (Wide Area Network):** Redes que cubren grandes distancias, como Internet.  
  * **Enfoque Red Team:** El perímetro se vuelve difuso. Se ataca desde fuera: **fuerza bruta a servicios expuestos**, **phishing** para obtener acceso inicial, o explotación de vulnerabilidades en aplicaciones web.

* **WLAN (Wireless LAN):** La versión sin cables.  
  * **Enfoque Red Team:** Ataques a Wi-Fi: **deautenticación**, **creación de evil twins**, **cracking de contraseñas WPA/WPA2** (PMKID, handshake capture). La movilidad y la falta de control físico son ventajas para el atacante.

---

## 2. La Dirección IP: La matrícula que puedes falsificar

La **dirección IP** es la identidad lógica de un dispositivo en la red. Pero en el mundo del Red Team, las IPs son pistas, señuelos y armas.

### Estructura de una IPv4 y su utilidad ofensiva

* **Ejemplo:** `192.168.1.15/24`  
  La máscara de subred (`/24` o `255.255.255.0`) define qué dispositivos están en tu misma red local.  
  * **Para el atacante:** Saber la máscara permite **descubrir el rango de IPs a escanear**. Si estás dentro de la LAN, puedes lanzar un escaneo a todo el rango (`nmap -sP 192.168.1.0/24`) para encontrar hosts vivos.

* **IP pública vs. privada:**  
  Las IPs privadas (como `10.0.0.0/8`, `172.16.0.0/12`, `192.168.0.0/16`) no son enrutables en Internet.  
  * **Anticipación de amenazas:** Si un servicio interno está usando una IP privada pero es accesible desde fuera mediante **NAT** (Port Forwarding), el atacante puede descubrir ese servicio con un escaneo de puertos a la IP pública. Herramientas como **Shodan** (el Google de los dispositivos conectados) indexan estos servicios expuestos involuntariamente.

* **IPv6:** Aunque más complejo, el Red Team debe considerarlo. Muchas configuraciones descuidan la seguridad en IPv6, dejando puertas traseras abiertas. Herramientas como `thc-ipv6` permiten ataques como **fake router advertisements** para redirigir tráfico.

---

## 3. Dirección MAC: El ADN que puedes clonar

La **MAC address** es única de fábrica, pero no inalterable. En sistemas Linux, puedes cambiarla con `macchanger` o `ifconfig`. ¿Para qué?

* **Bypass de filtrados:** Algunas redes Wi-Fi usan filtrado por MAC. Si obtienes una MAC válida (por ejemplo, capturando tráfico con un sniffer), puedes suplantarla.
* **Ataques de "MAC flooding":** En switches, puedes saturar la tabla CAM enviando miles de MACs falsas, haciendo que el switch entre en modo "hub" y puedas espiar tráfico entre otros dispositivos (ataque con `macof` de la suite dsniff).
* **Evadir restricciones de tiempo/acceso:** En redes universitarias o empresariales que limitan el acceso por MAC, la suplantación es clave.

---

## 4. Comandos Básicos de Diagnóstico e Identificación (Ahora con enfoque ofensivo)

Estos comandos no solo diagnostican, sino que son el punto de partida de cualquier ataque.

### En Windows (CMD o PowerShell)

| Comando | Función ofensiva |
| --- | --- |
| `ipconfig` | Determinar tu propia IP y puerta de enlace (el router). La puerta de enlace es un objetivo principal para ataques MITM. |
| `ipconfig /all` | Revela la **MAC**, los servidores DNS (para posibles ataques de DNS spoofing) y si DHCP está habilitado. |
| `ping [IP/Dominio]` | Verificar conectividad y estimar tiempos de respuesta (para ataques de temporización). Un ping exitoso indica que el host está vivo. |
| `tracert [IP/Dominio]` | Mapear la ruta de red. Útil para identificar firewalls, routers intermedios y posibles puntos de inspección. |
| `arp -a` | Muestra la caché ARP local. Si estás en la misma red, puedes ver qué dispositivos se han comunicado recientemente. Esto te da un mapa de relaciones IP-MAC. |

### En Linux y macOS (Terminal)

| Comando | Función ofensiva |
| --- | --- |
| `ip addr` o `ifconfig` | Igual que en Windows, pero además puedes cambiar la MAC con `ifconfig eth0 hw ether 00:11:22:33:44:55`. |
| `ping -c 4 [IP]` | Probar disponibilidad. Un atacante puede hacer un **ping sweep** automático para descubrir hosts. |
| `traceroute [IP]` | Identificar routers intermedios y posibles saltos. Útil para ataques de **TTL expiration** o para evasión de firewalls. |
| `netstat -tunlp` | Ver qué servicios están escuchando en tu propia máquina. Si has comprometido un sistema, este comando te muestra qué otros servicios están abiertos localmente. |
| `whois [dominio]` | Obtener información del objetivo: rango de IPs, contactos administrativos (para phishing), servidores DNS. |

### Herramientas avanzadas de Red Team

* **nmap:** El rey del escaneo. Permite detectar hosts, puertos abiertos, servicios y versiones, e incluso el sistema operativo. Un escaneo sigiloso (`-sS`) puede evadir algunos IDS.
* **Wireshark / tcpdump:** Captura y analiza tráfico. Ideal para ver qué datos viajan en claro, capturar handshakes Wi-Fi, o extraer credenciales de protocolos inseguros (HTTP, FTP, Telnet).
* **Netcat (nc):** La navaja suiza. Permite crear conexiones TCP/UDP, transferir archivos, o establecer reverse shells.
* **Metasploit:** Framework para explotar vulnerabilidades. Integra módulos de reconocimiento, explotación y post-explotación.

---

## 5. El Concepto de Puertos (Las puertas de entrada)

Si la IP es la casa, los puertos son las puertas y ventanas. Un escaneo de puertos revela qué servicios están corriendo y, por tanto, posibles vectores de ataque.

### Puertos comunes y su explotación

| Puerto | Servicio | Uso típico | Ataques comunes |
|--------|----------|------------|-----------------|
| 21 | FTP | Transferencia de archivos | Anónimo permitido, fuerza bruta, FTP bounce |
| 22 | SSH | Acceso remoto seguro | Fuerza bruta, claves débiles, versiones vulnerables |
| 23 | Telnet | Acceso remoto inseguro | Credenciales en texto claro, fácil de esnifar |
| 25 | SMTP | Correo saliente | Spoofing de correo, relay abierto |
| 53 | DNS | Resolución de nombres | Ataques de poisoning, tunneling de datos |
| 80 | HTTP | Web | Inyección SQL, XSS, LFI/RFI, etc. |
| 443 | HTTPS | Web segura | Ataques a SSL/TLS (Heartbleed, etc.) |
| 445 | SMB | Compartición de archivos (Windows) | EternalBlue, enumeración de usuarios, pass-the-hash |
| 1433 | MSSQL | Base de datos SQL Server | Fuerza bruta, ejecución de comandos mediante xp_cmdshell |
| 3306 | MySQL | Base de datos MySQL | Escaneo de versiones vulnerables, fuerza bruta |
| 3389 | RDP | Escritorio remoto | BlueKeep, fuerza bruta, credenciales débiles |

### ¿Cómo usar esta información para anticipar amenazas?

1. **Escaneo proactivo:** Un equipo azul debe escanear su propia red para descubrir puertos abiertos no autorizados (shadow IT) o servicios desactualizados. Herramientas como **Nessus**, **OpenVAS** o **Qualys** automatizan esto.
2. **Honeypots:** Simular servicios en puertos comunes para atraer atacantes y estudiar sus técnicas.
3. **Segmentación:** Aislar sistemas críticos para que, aunque un atacante entre por un puerto, no pueda moverse lateralmente. Por ejemplo, los servidores de bases de datos no deberían aceptar conexiones desde cualquier equipo de la LAN, solo desde las aplicaciones que los necesitan.
4. **Firewalls y listas de control de acceso (ACL):** Limitar el acceso a puertos solo a IPs autorizadas. Un atacante externo no debería poder tocar el puerto 22 de un servidor interno.

---

## 6. Anticipación de Amenazas: El Ciclo del Red Team

El Red Team no solo ataca; también ayuda a anticipar. ¿Cómo?

* **Modelado de amenazas:** Basado en el reconocimiento, se identifican los activos críticos y los posibles caminos hacia ellos. Por ejemplo, si un servidor web está en la DMZ y se comunica con una base de datos interna, un atacante podría explotar una vulnerabilidad web para pivotar hacia la base de datos.
* **Detección de desviaciones:** Conocer el tráfico normal (baselines) ayuda a detectar anomalías. Un atacante que hace un escaneo de puertos o transfiere grandes volúmenes de datos fuera de horario levanta sospechas.
* **Pruebas de penetración periódicas:** Simular ataques reales (con técnicas como las descritas) para validar que los controles funcionan y que el personal de respuesta está preparado.

---

## Conclusión

Entender redes es el primer paso, pero orientarlo a Red Team significa ir más allá: **cada protocolo, cada dirección, cada puerto es una oportunidad para atacar o para defender**. Conocer las herramientas y técnicas ofensivas te permite construir defensas más sólidas, anticipándote a los movimientos del adversario. La red ya no es solo un conducto; es el campo de batalla donde se libra la guerra cibernética.


**Siguiente paso:** Aprende a escanear redes como un atacante con `nmap`, a interceptar tráfico con `Wireshark` y a explotar servicios con `Metasploit`. La práctica es clave.

**BIBLIOGRAFIA**

- https://achirou.com/curso-de-redes-para-hackers-el-modelo-osi/
- https://ciberprisma.org/2024/07/04/como-los-cibercriminales-atacan-cada-una-de-las-capas-del-modelo-osi-1-7/


