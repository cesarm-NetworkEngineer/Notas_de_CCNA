Resumen de conceptos importantes del CCNA

El CCNA es una certificación reconocida internacionalmente que valida conocimientos fundamentales sobre redes. A continuación, se presenta un resumen con los puntos esenciales que abarca esta certificación:
1. Fundamentos de Redes
1.1. Modelo OSI y TCP/IP
Modelo OSI (Open Systems Interconnection): Un marco conceptual de 7 capas para entender cómo los datos viajan a través de una red. Las capas son:
  * Física.
  * Enlace de datos.
  * Red.
  * Transporte.
  * Sesión.
  * Presentación.
  * Aplicación.

Modelo TCP/IP: Similar al modelo OSI, pero más práctico con 4 capas:
  * Acceso a la red (equivalente a las capas Física y Enlace de datos del OSI).
  * Internet (equivalente a la capa de Red del OSI).
  * Transporte.
  * Aplicación (equivalente a las capas de Sesión, Presentación y Aplicación del OSI).
1.2. Direcciones IP
IPv4: Dirección de 32 bits dividida en 4 octetos. Clases de dirección (A, B, C, D, E). Subnetting (creación de subredes para optimizar el uso de direcciones).
IPv6: Dirección de 128 bits diseñada para reemplazar IPv4, con mayor capacidad y sin necesidad de NAT.
1.3. Protocolos de red comunes
ARP (Address Resolution Protocol): Traduce direcciones IP a direcciones MAC.
DNS (Domain Name System): Resuelve nombres de dominio a direcciones IP.
DHCP (Dynamic Host Configuration Protocol): Asigna direcciones IP automáticamente a dispositivos.
HTTP/HTTPS: Protocolos de transferencia de datos web.
2. Equipos de Red y Configuración Básica
2.1. Dispositivos comunes
Switches: Operan en la capa 2 del modelo OSI, permitiendo la comunicación dentro de una red local (LAN).
Routers: Operan en la capa 3, conectando redes diferentes y determinando las mejores rutas para el tráfico.
Access Points (AP): Facilitan conexiones inalámbricas en una red.
2.2. Conceptos clave sobre switches y routers
VLANs (Virtual LANs): Segmentación lógica dentro de un switch para separar el tráfico.
Trunking: Permite que múltiples VLANs se transmitan a través de un solo enlace entre switches.
Routing estático vs dinámico:
  Estático: El administrador define rutas manualmente.
  Dinámico: Usa protocolos como OSPF, EIGRP o RIP para aprender rutas automáticamente.
2.3. Configuración básica con Cisco IOS
Modos de configuración:
  Modo usuario: Acceso básico (sin configuraciones).
  Modo privilegiado: Acceso avanzado (`enable`).
  Modo de configuración global: Configuración de dispositivos (`configure terminal`).

* Comandos básicos:
```
# Configuración de una dirección IP en una interfaz
interface GigabitEthernet0/1
ip address 192.168.1.1 255.255.255.0
no shutdown
```
3. Protocolos de Enrutamiento
RIP (Routing Information Protocol):
  Protocolo de enrutamiento basado en la distancia. Limita las rutas a un máximo de 15 saltos.
EIGRP (Enhanced Interior Gateway Routing Protocol):
  Protocolo híbrido desarrollado por Cisco, que combina características de enrutamiento basado en distancia y estado de enlace.
OSPF (Open Shortest Path First):
  Protocolo de estado de enlace que utiliza el algoritmo SPF (Shortest Path First) para determinar las rutas más rápidas.
4. Seguridad en Redes
4.1. Principios básicos de seguridad
Control de acceso: Uso de ACLs (Access Control Lists) para filtrar tráfico no deseado.
Autenticación y autorización: Implementación de protocolos como RADIUS y TACACS+ para validar usuarios.
Encriptación: Protección de datos en tránsito mediante protocolos como IPsec y SSL/TLS.
4.2. Seguridad en switches y routers
Port Security: Restringe qué dispositivos pueden conectarse a los puertos del switch.
SSH (Secure Shell): Sustituto seguro de Telnet para acceso remoto.
5. Redes Inalámbricas (Wireless)
5.1. Tecnologías Wi-Fi
Estándares IEEE 802.11: Varían en velocidad, frecuencia y alcance (802.11a/b/g/n/ac/ax).
5.2. Configuración básica de redes inalámbricas
SSID (Service Set Identifier): Identificador de la red.
Seguridad: Uso de WPA2 o WPA3 para proteger conexiones inalámbricas.
6. Resolución de Problemas en Redes
6.1. Enfoque estructurado
* Identificar el problema.
* Establecer una hipótesis.
* Probar soluciones.
* Documentar los resultados.
6.2. Comandos comunes de diagnóstico
* `ping`: Verifica conectividad.
* `traceroute`: Muestra la ruta hacia un destino.
* `show`: Examina el estado de configuración en dispositivos Cisco.
* `debug`: Muestra información en tiempo real sobre eventos en el dispositivo.
7. Automatización y Virtualización de Redes
7.1. Conceptos básicos de automatización
* Uso de herramientas como Python y Ansible para automatizar tareas de red.
7.2. Virtualización de redes
* Implementación de redes definidas por software (SDN).
* Uso de plataformas virtuales como GNS3 o Packet Tracer para simulación.
