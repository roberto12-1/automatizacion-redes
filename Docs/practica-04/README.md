TABLA

[Tabla Criterios.pdf](https://github.com/user-attachments/files/33849887/Tabla.Criterios.pdf)

1. ¿Cuál de los recursos consideras más útil para resolver dudas de Python? ¿Por qué?
Considero que el recurso más útil es la Documentación Oficial de Python. Es el estándar definitivo porque está creada y mantenida por la propia Python Software Foundation, lo que garantiza que la información sobre sintaxis, parámetros y métodos integrados sea completamente precisa, esté actualizada a la versión más reciente del lenguaje y no contenga malas prácticas o errores lógicos comunes que a menudo se encuentran en foros informales.

2. ¿Cuál consultarías para resolver un problema relacionado con GNS3?
Consultaría la Documentación Oficial de GNS3 (junto con su sitio de soporte y comunidad técnica oficial). Es la fuente ideal porque ofrece guías específicas sobre la configuración de appliances, integración de hipervisores (como QEMU o KVM), solución de problemas de rendimiento (como el uso de CPU) y la correcta interconexión de nubes virtuales y adaptadores de red.

3. ¿Por qué no conviene copiar directamente una solución sin comprobar que funciona en el entorno de trabajo?
Porque cada entorno de trabajo tiene particularidades únicas (como versiones específicas de software, dependencias instaladas, sistemas operativos distintos, topologías de red diferentes o restricciones de permisos). Copiar código o configuraciones a ciegas suele provocar fallos de compatibilidad, errores de ejecución (bugs) o comportamientos inesperados que son muy difíciles de depurar si no se comprende exactamente qué hace la solución y cómo interactúa con el resto del proyecto.

TABLA 2

[Tabla 2.pdf](https://github.com/user-attachments/files/33849987/Tabla.2.pdf)


1. Propósito de la práctica
El propósito de esta práctica es desarrollar habilidades para la investigación técnica eficiente, el análisis crítico de fuentes de información y la evaluación de recursos digitales (documentación oficial, repositorios y comunidades colaborativas). Asimismo, busca establecer estrategias estructuradas de solución de problemas (troubleshooting) aplicadas al desarrollo de scripts en Python y a la simulación e ingeniería de redes.

2. Relación con el proyecto integrador
Esta práctica se vincula directamente con el proyecto integrador al proporcionar la base metodológica para seleccionar y utilizar herramientas fundamentales como Python, GNS3 y Netmiko. La capacidad de consultar documentación oficial y entornos colaborativos permite al equipo:

Diseñar y validar la topología de red simulada en GNS3 sin errores de rendimiento o compatibilidad.

Desarrollar scripts de automatización con Netmiko utilizando sintaxis correcta y buenas prácticas de programación.

Resolver incidencias técnicas en el código o en la infraestructura simulada de forma autónoma y estructurada.

3. Recursos consultados: síntesis y enlaces
Documentación Oficial de Python (Sección: Estructuras de Datos)

URL: https://docs.python.org/es/3/tutorial/datastructures.html

Síntesis: Aborda la manipulación avanzada de listas, diccionarios y colecciones integradas en Python, detallando métodos como .append(), .pop(), .get() e iteración de elementos.

Documentación Oficial de GNS3

URL: https://docs.gns3.com/

Síntesis: Ofrece guías técnicas sobre la instalación de la GNS3 VM, integración de appliances (Cisco IOS, IOU, Docker), gestión del hipervisor y configuración de adaptadores de red (uBridge).

Repositorio Oficial de Netmiko (GitHub / ReadTheDocs)

URL: https://github.com/ktbyers/netmiko

Síntesis: Proporciona el código fuente, parámetros de la clase ConnectHandler y ejemplos prácticos para automatizar conexiones SSH y ejecución de comandos CLI en dispositivos de red multi-vendor.

4. Evaluación de confiabilidad de los recursos
Recurso 1: Documentación Oficial de Python
¿Quién publica o mantiene el recurso?: La Python Software Foundation (PSF) y la comunidad oficial de desarrollo del lenguaje.
¿La información corresponde al tema investigado?: Sí, corresponde al uso de estructuras de datos, lógica de programación y sintaxis en Python.
¿Incluye ejemplos o instrucciones verificables?: Sí, proporciona bloques de código ejecutables, sintaxis oficial y salidas esperadas de consola.
¿Se identifica la versión o fecha de actualización cuando corresponde?: Sí, permite seleccionar explícitamente la versión del lenguaje (ej. Python 3.10, 3.11, 3.12).
¿Es posible comprobar la información con otra fuente?: Sí, es verificable mediante ejecución directa en el intérprete de Python y estándares PEP.
¿Qué utilidad tiene para el proyecto integrador?: Sirve como base para escribir código limpio, eficiente y sin errores sintácticos para el procesamiento de datos.
Recurso 2: Documentación Oficial de GNS3
¿Quién publica o mantiene el recurso?: GNS3 Technologies Inc. y el equipo principal de desarrollo de la herramienta.
¿La información corresponde al tema investigado?: Sí, aborda la construcción, simulación, rendimiento y configuración de topologías de red.
¿Incluye ejemplos o instrucciones verificables?: Sí, contiene guías paso a paso, capturas de interfaz, parámetros de rendimiento y comandos de terminal.
¿Se identifica la versión o fecha de actualización cuando corresponde?: Sí, especifica la versión del cliente GNS3, GNS3 VM y compatibilidad con hipervisores.
¿Es posible comprobar la información con otra fuente?: Sí, es comprobable mediante la comunidad oficial de GNS3, foros técnicos y pruebas de laboratorio.
¿Qué utilidad tiene para el proyecto integrador?: Permite diseñar, levantar y solucionar fallos en la topología de red simulada antes de automatizarla.

Recurso 3: Repositorio Netmiko (GitHub)
¿Quién publica o mantiene el recurso?: Kirk Byers (creador principal) junto con la comunidad open source de automatización de redes.
¿La información corresponde al tema investigado?: Sí, está enfocado específicamente en la automatización de conexiones SSH y gestión CLI de equipos de red mediante Python.
¿Incluye ejemplos o instrucciones verificables?: Sí, ofrece fragmentos de código (snippets), scripts de prueba y ejemplos del objeto ConnectHandler.
¿Se identifica la versión o fecha de actualización cuando corresponde?: Sí, mediante registros de lanzamientos (releases), etiquetas (tags) e historial de commits con fecha exacta.
¿Es posible comprobar la información con otra fuente?: Sí, es comprobable mediante la documentación en ReadTheDocs y pruebas de conectividad SSH en routers/switches.
¿Qué utilidad tiene para el proyecto integrador?: Facilita la creación de scripts en Python que se conectan y configuran los routers/switches de la topología.

5. Estrategia de solución del problema (Situación hipotética)
Caso a resolver: El script dispositivos.py muestra correctamente la información de R1 y R2, pero al intentar buscar un dispositivo por su nombre, el programa no identifica el equipo solicitado.
Problema identificado: El script dispositivos.py muestra la información general de los routers, pero la función o bloque de búsqueda no logra hacer coincidir el parámetro ingresado con los registros guardados (falla en la lógica de filtrado o sensibilidad a mayúsculas/minúsculas).
Palabras clave para realizar la búsqueda: python dictionary search by key, python filtrar lista de diccionarios por atributo, python match string case-insensitive, python function find element in list.
Documentación o comunidad que consultarían primero: La Documentación Oficial de Python (métodos de listas, diccionarios y cadenas) y Stack Overflow para identificar patrones estándar de búsqueda.

Información que revisarían en el código:
La estructura de datos donde se almacenan los equipos (listas de diccionarios vs. diccionarios anidados).

La comparación de cadenas (verificar el uso de .lower() o .strip() para evitar fallos por espacios o mayúsculas).

Tipo de ejemplo o solución que buscarían: Ejemplos de comprensión de listas (list comprehension) o funciones iterativas de búsqueda segura dentro de colecciones de diccionarios en Python.

Cómo comprobarían que la solución funciona: Ejecutando pruebas unitarias con nombres válidos (R1, r1), variaciones con espacios y nombres inexistentes (R3) para verificar la correcta respuesta del programa.

Cómo documentarían la solución encontrada: Agregando comentarios explicativos en el bloque corregido dentro del script y registrando el ajuste en el historial de cambios (commits) del repositorio.

6. Aprendizajes obtenidos
Comprender la importancia de priorizar la documentación oficial sobre fuentes informales para garantizar el uso de sintaxis actualizada y evitar malas prácticas de programación.

Identificar las diferencias operativas entre la documentación de software de simulación (GNS3) y el repositorio de una biblioteca de código (Netmiko en GitHub).

Desarrollar un criterio estructurado para formular preguntas técnicas claras y precisas en comunidades de desarrollo, incluyendo contextos, código mínimo reproducible y errores observados.

Fortalecer el análisis crítico al evaluar la confiabilidad, actualización y aplicabilidad de recursos en línea antes de integrar soluciones al entorno de trabajo.

7. Conclusión individual
CABAÑAS CARDENAS ROBERTO DEL ANGEL
Durante el desarrollo de esta práctica, comprendí que la documentación oficial y las comunidades colaborativas son pilares indispensables para la formación en ingeniería. Consultar fuentes oficiales garantiza que los conceptos técnicos se apliquen de forma correcta y bajo los estándares de la industria, evitando soluciones temporales o ineficientes. Por otro lado, las comunidades técnicas como Stack Overflow o GitHub facilitan el intercambio de conocimiento ante problemas complejos, permitiendo analizar cómo otros desarrolladores han abordado situaciones similares. Sin embargo, aprendí que no basta con copiar una solución encontrada en un foro; es fundamental analizarla, probarla en nuestro propio entorno y entender su funcionamiento antes de integrarla. Saber buscar información de manera estructurada reduce significativamente los tiempos de desarrollo y resolución de fallos, lo que resulta vital para el éxito de proyectos integradores y la gestión de infraestructura en escenarios reales.
