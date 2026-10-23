1. ¿Qué tipo de problema podrías resolver consultando la documentación de GNS3?
Problemas relacionados con la configuración del entorno de simulación, como la integración de máquinas virtuales con adaptadores de red locales, la instalación y arranque de appliances (routers Cisco IOS, switches, contenedores), la resolución de errores de hipervisores (como fallos en QEMU o KVM) y la correcta asignación de enlaces virtuales y nubes (Cloud).

2. ¿Qué diferencia existe entre la documentación de una herramienta y el repositorio de una biblioteca?
Documentación de una herramienta (ej. GNS3): Está diseñada para explicar cómo instalar, configurar y operar un software de uso general o interfaz gráfica, detallando guías de usuario, arquitectura y resolución de problemas (troubleshooting).

Repositorio de una biblioteca (ej. GitHub de Netmiko): Es el espacio donde se almacena el código fuente abierto del paquete de programación. Incluye el historial de versiones, control de cambios (commits), el archivo README con instrucciones de instalación por consola (pip), el registro de errores abiertos (issues) y contribuciones de la comunidad de desarrolladores.

3. ¿Qué información revisarías antes de utilizar una biblioteca de automatización?
Compatibilidad de versiones: Qué versiones de Python soporta.

Dispositivos soportados: Qué fabricantes y modelos de equipos de red maneja (Cisco, Juniper, HP, Arista, etc.).

Documentación y ejemplos de código: Si cuenta con guías claras de inicio rápido para establecer conexiones SSH y manejo de excepciones.

Mantenimiento activo: Fecha de los últimos commits y frecuencia de actualizaciones para garantizar seguridad y soporte actual.

4. ¿Por qué es importante comprobar qué plataformas y funciones admite una biblioteca?
Porque los dispositivos de red de distintos fabricantes (y a veces distintas familias de un mismo fabricante) utilizan sintaxis de comandos CLI diferentes, métodos de autenticación particulares o respuestas de terminal dispares. Saber qué plataformas admite garantiza que la biblioteca sabrá manejar adecuadamente el canal interactivo (channel) sin bloquearse o enviar comandos no compatibles.

5. ¿Cómo podrían utilizarse estos recursos en las siguientes prácticas?
GNS3: Se utilizaría para diseñar, levantar y probar el esquema físico/lógico de la red (por ejemplo, interconectar routers con protocolos de enrutamiento OSPF o EIGRP).

Netmiko (u otras bibliotecas de automatización): Se utilizaría para escribir scripts en Python que se conecten de manera programática a los routers simulados en GNS3 para extraer tablas de enrutamiento, respaldar archivos de configuración (running-config) o aplicar cambios masivos de manera simultánea.

Parte 2: Registro de Recursos Técnicos
Recurso 1: GNS3 Documentation
Nombre del recurso: GNS3 Documentation & User Guide

URL: https://docs.gns3.com/

Tema que aborda: Arquitectura, instalación, configuración de topologías complejas e integración de dispositivos de red virtuales y reales.

Tipo de información que ofrece: Guías técnicas oficiales paso a paso, manuales de configuración de appliances (Cisco IOS, IOU, Docker), solución de errores de rendimiento y configuración de adaptadores de red (uBridge).

Utilidad para el proyecto integrador: Permite estructurar y validar la correcta implementación del escenario de red simulado, asegurando que las interfaces y los protocolos de red funcionen antes de aplicar scripts de automatización.

Ejemplo de una situación en la que lo consultarías: Lo consultaría si al arrancar un router Cisco IOS en GNS3 el consumo de CPU se dispara al 100% y necesito configurar la variable de ralentización de CPU (idle-pc) recomendada oficialmente.

Recurso 2: Netmiko (Repositorio y Documentación)
Nombre del recurso: Netmiko GitHub Repository / ReadTheDocs

URL: https://github.com/ktbyers/netmiko (o https://netmiko.readthedocs.io/)

Tema que aborda: Automatización de conexiones SSH y ejecución de comandos CLI en dispositivos de red multi-vendor mediante Python.

Tipo de información que ofrece: Código fuente oficial, métodos de la clase ConnectHandler, parámetros de conexión (IP, usuario, contraseña, tipo de dispositivo como cisco_ios), ejemplos prácticos de envío de comandos y manejo de sesiones interactivas.

Utilidad para el proyecto integrador: Es la base fundamental para desarrollar los scripts en Python orientados a interactuar de forma automatizada con los dispositivos de red configurados en el laboratorio.

Ejemplo de una situación en la que lo consultarías: Lo consultaría para verificar el argumento exacto del diccionario device_params necesario para conectarse a un switch Cisco mediante SSH especificando un puerto personalizado.

Recurso 3: Cisco DevNet
Nombre del recurso: Cisco DevNet (Network Automation Learning Labs)

URL: https://developer.cisco.com/learning/

Tema que aborda: Programabilidad de redes, uso de APIs, Netconf/YANG, Python aplicado a infraestructura y herramientas de automatización.

Tipo de información que ofrece: Laboratorios guiados, tutoriales de programación para ingenieros de redes, ejemplos de scripts y documentación técnica avalada por desarrolladores de infraestructura.

Utilidad para el proyecto integrador: Funciona como guía de buenas prácticas y fuente de inspiración para estructurar scripts robustos que cumplan con estándares de la industria en la gestión de redes.

Ejemplo de una situación en la que lo consultarías: Lo consultarías para aprender la estructura recomendada al parsear la salida de un comando de estado de interfaces (show ip interface brief) utilizando expresiones regulares dentro de un script de automatización.
