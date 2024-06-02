![manolibot](/img/ManoliBot.jpeg)
## **¿Qué es ManoliBot?**
ManoliBot es un bot de Telegram programado en Bash diseñado para simplificar la gestión y control de servidores mediante la ejecución remota de comandos. Integrándose con la plataforma de mensajería Telegram, ManoliBot ofrece una interfaz accesible y fácil de usar que permite a los usuarios enviar comandos y recibir resultados de manera rápida y conveniente.

### **Características Clave de ManoliBot**

- **Interfaz de Telegram:** Permite interactuar con el bot desde la aplicación Telegram.

- **Ejecución de Comandos Remotos:** Permite ejecutar comandos en servidores remotos mediante SSH.

- **Seguridad:** Incluye una lista de comandos prohibidos y solo acepta comandos de usuarios autorizados.

- **Gestión de Hosts:** Los hosts disponibles se gestionan mediante un archivo de texto, facilitando su configuración y ampliación.

### **Funcionalidades y Comandos**

```
/ayuda: Muestra la lista de comandos disponibles.
/ejecutar [comando]: Ejecuta el comando en el servidor local.
/ejecutar_host [host] [comando]: Ejecuta el comando en un host específico.
```
### **Requisitos**

Bash (compatible con sistemas Unix/Linux).
Acceso a Internet para enviar y recibir mensajes desde Telegram.
SSH configurado en los hosts remotos para ejecutar comandos de forma remota.

### **Ejemplo de Uso**
Ejecutar un comando en el servidor local:

```
/ejecutar uname -a
```
Ejecutar un comando en un host específico:

```
/ejecutar_host servidor1 uptime
```

### **Conclusión**
ManoliBot es una herramienta útil para la administración remota de servidores a través de Telegram. Su capacidad para ejecutar comandos de manera segura y remota lo convierte en una opción ideal para administradores de sistemas y equipos de TI que desean simplificar la gestión y el monitoreo de servidores desde una interfaz accesible como Telegram.
