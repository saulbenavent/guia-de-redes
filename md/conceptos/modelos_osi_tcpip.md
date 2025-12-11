# Modelos OSI y TCP/IP

TCP/IP es un modelo práctico que aborda desafíos de comunicación específicos y se basa en protocolos estandarizados. Por el contrario, OSI sirve como un marco integral e independiente del protocolo diseñado para abarcar varios métodos de comunicación de red.

---

# Modelo OSI (7 capas)

1. **Física:** Esto consiste en una conexión de datos entre un dispositivo que genera datos y la red.
2. **Enlace de datos:** La capa de enlace de datos es la conexión punto a punto que transmite los datos a la capa de red.
3. **Red:** En la capa de red, los datos obtienen su dirección e instrucciones de enrutamiento para prepararse para su recorrido por la red.
4. **Transporte:** En la capa de transporte, los datos saltan entre diferentes puntos de la red en camino a su destino.
5. **Sesión:** La capa de sesión tiene una conexión que administra las sesiones que ocurren entre aplicaciones.
6. **Presentación:** La capa de presentación es donde los datos se cifran, descifran y convierten en una forma a la que puede acceder la capa de aplicació.
7. **Aplicación:** En la capa de aplicación, una aplicación, como un navegador de Internet, obtiene los datos y un usuario puede interactuar con ellos.

---

### Ejemplo práctico

Cuando abres una web:

- La capa 7 envía la petición (HTTP).
- La capa 4 usa TCP.
- La capa 3 calcula rutas (IP).
- La capa 1 envía bits por el cable o WiFi.

---

# Modelo TCP/IP (4 capas)

1. **Acceso a la red:** La capa de enlace de datos del modelo TCP/IP se corresponde con las capas de enlace de datos y física del modelo OSI y es responsable de las conexiones físicas y lógicas entre dispositivos.  
2. **Internet:** Al igual que la capa roja del modelo OSI, la capa TCP/IP de Internet gestiona el enrutamiento y el reenvío de paquetes.  
3. **Transporte:** La capa de transporte se asigna a la capa de transporte OSI y es responsable de la conectividad de extremo a extremo, la integridad de los datos y el control de flujo.  
4. **Aplicación:** La capa de aplicación combina las capas de aplicación, Presentación y Sesión de OSI y es responsable de los protocolos de aplicación de alto nivel, la representación y la gestión de sesiones.

---

## Comparativa

| Modelo OSI (7 capas)       | Modelo TCP/IP (4 capas) |
|----------------------------|--------------------------|
| 7. Aplicación              | 4. Aplicación            |
| 6. Presentación            | 4. Aplicación            |
| 5. Sesión                  | 4. Aplicación            |
| 4. Transporte              | 3. Transporte            |
| 3. Red                     | 2. Internet              |
| 2. Enlace de datos         | 1. Acceso a la red       |
| 1. Física                  | 1. Acceso a la red       |

---

!!! tip "Consejo"
    El modelo OSI es teórico. TCP/IP es el modelo real que usan las redes hoy.

