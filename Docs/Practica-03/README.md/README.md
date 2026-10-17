Que se hizo? Se desarrolló un programa en Python para representar, almacenar y gestionar la información de dispositivos de red de una infraestructura (como routers y switches). Para ello, se aplicaron estructuras de datos como listas y diccionarios, se automatizó su recorrido mediante ciclos, se evaluó su condición operativa con estructuras condicionales, y se modularizó el código utilizando funciones para facilitar su mantenimiento y visualización en consola

Que se Utilizo?  
Variables: Espacios de memoria utilizados para almacenar valores individuales (como el nombre de un dispositivo, su dirección IP o su estado).  
Tipos de datos: La clasificación de los valores que maneja el programa; en esta práctica se utilizaron principalmente cadenas de texto (str) para describir las características de los equipos de red.  
print(): Función integrada en Python que permite enviar mensajes y mostrar los valores de las variables o resultados en la pantalla de la terminal. 
Diccionarios: Estructuras de datos que almacenan información en formato de pares clave-valor ("clave": "valor"), permitiendo agrupar de forma ordenada los atributos de cada dispositivo (nombre, tipo, IP, estado, fabricante y protocolo).  
Listas: Estructuras ordenadas que permiten agrupar múltiples elementos (en este caso, los diccionarios de cada equipo) para representar de forma conjunta toda la infraestructura de red.  
Ciclo for: Estructura de control iterativa que permite recorrer elemento por elemento la lista de dispositivos para procesarlos o imprimirlos de manera automatizada.  
Condicional if: Estructura de decisión lógica que evalúa si una condición se cumple (por ejemplo, verificar si el estado de un dispositivo es "Activo") para ejecutar bloques de código específicos.   
Funciones: Bloques de código reutilizables y con un nombre específico (como mostrar_dispositivo()) que encapsulan tareas repetitivas para evitar la duplicación de código y mejorar la organización del programa.

Dispositivo | Tipo   |  Direccion ip |   Estado                   |  Funcion
R1          | Router | 10.1.1.1      |  Activo                    |Enrutamiento
R2          | Router | 10.1.1.2      | Activo/Fuera de Servicio   |Enrutamiento
R3          | Switch | 10.1.1.3      | Activo                     |Conectividad

Problema                       | Causa                                              | Solucion
IndentationError en la         |Desalineación en los espacios                       | Ajustar el nivel de sangría de manera uniforme en 
terminal al ejecutar el script |o tabulaciones dentro de la función o del ciclo for.|Visual Studio Code utilizando la tecla Tab.
                               |                                                    |
Los nuevos datos de los        |La función mostrar_dispositivo() aún no contenía    |Actualizar la función incorporando 
dispositivos no se imprimían   |las instrucciones print() para las nuevas claves    |las líneas correspondientes a las 
en pantalla.                   |agregadas.                                          |nuevas claves del diccionario.   

Conclusion: Aprendizajes: Durante el desarrollo de la práctica se aprendió a modelar y estructurar información de una infraestructura de red utilizando colecciones en Python, como listas y diccionarios. Asimismo, se afianzó el uso de ciclos iterativos for, estructuras de control condicionales if-else y la modularización de código mediante funciones para optimizar la lógica de programación.   Base para la automatización: Este tipo de programas constituye la base esencial para la automatización de redes, ya que permite almacenar topologías de forma estructurada que posteriormente pueden integrarse con archivos de configuración externos (como JSON o YAML), bases de datos, o librerías especializadas (por ejemplo, Netmiko o Paramiko) para administrar y desplegar comandos de manera masiva en equipos reales.
