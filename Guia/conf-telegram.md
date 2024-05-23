## Paso 1: Creación del bot en Telegram

- **Crear un bot en Telegram:** Abre Telegram y busca el bot llamado @BotFather. Inicia una conversación con él enviando el comando /start.

- **Crear un nuevo bot:** Envía el comando /newbot para crear un nuevo bot. Sigue las instrucciones para elegir un nombre y un nombre de usuario para tu bot.

- **Obtener el token del bot:** Después de crear el bot, @BotFather te dará un token de acceso único para tu bot. Guarda este token, lo necesitarás más adelante.


## Paso 2: Escritura del script

- **Obtener el ID del chat:** Necesitamos el ID del chat, que es el identificador de la conversación que tenemos con el bot. Para obtenerlo, accedemos a la siguiente página web: https://api.telegram.org/bot<YOUR-BOT-TOKEN>/getUpdates. Esto nos dará el ID del chat, que necesitaremos más adelante en el script.

- **Instalar el paquete requests:** Utilizaremos el paquete requests para enviar solicitudes a los servidores de Telegram. Instálalo usando el siguiente comando: pip3 install requests.

- **Crear el script Python:**

```
#!/usr/bin/env python3

import requests
import sys

def send_telegram_message(alert_file, hook_url, chat_id):
    # Leer el archivo de alerta
    with open(alert_file, 'r') as file:
        alert_data = file.read()

    # Generar el mensaje
    message = f"**Nuevo Alerta de Wazuh:**\n\n{alert_data}"

    # Enviar el mensaje a Telegram
    requests.post(f"https://api.telegram.org/bot{hook_url}/sendMessage", data={"chat_id": chat_id, "text": message, "parse_mode": "Markdown"})

if __name__ == "__main__":
    # Obtener los argumentos del script
    alert_file = sys.argv[1]
    hook_url = sys.argv[2]
    chat_id = sys.argv[3]

    # Llamar a la función para enviar el mensaje
    send_telegram_message(alert_file, hook_url, chat_id)
```

## Paso 3: Configuración de Wazuh para enviar alertas a Telegram

- **Copiar el script al servidor de Wazuh:** Copia el script Python a la carpeta /var/ossec/integrations/ en el servidor donde está instalado el gestor de Wazuh.

- **Dar permisos al script:** Ejecuta los siguientes comandos para dar los permisos adecuados al script y asignarlo al usuario adecuado:

```
chmod 750 /var/ossec/integrations/custom-telegram
chown root:ossec /var/ossec/integrations/custom-telegram
```
- **Configurar Wazuh para enviar alertas a Telegram:**

Abre el archivo de configuración ossec.conf ubicado en **/var/ossec/etc/ossec.conf.**

Agrega la siguiente configuración en la sección <ossec_config>:

```
<integration>
    <name>telegram</name>
    <hook_url>YOUR-BOT-TOKEN</hook_url>
    <level>12</level> <!-- Cambiar si es necesario -->
    <format>json</format>
    <options>chat_id=YOUR-CHAT-ID</options>
    <command>custom-telegram</command>
    <path>etc/integrations</path>
    <frequency>360</frequency>
</integration>
```

* Reemplaza YOUR-BOT-TOKEN con el token de tu bot y YOUR-CHAT-ID con el ID del chat que obtuviste anteriormente.

- **Reiniciar el gestor de Wazuh:** Reinicia el gestor de Wazuh para que los cambios surtan efecto:


```
sudo systemctl restart wazuh-manager
```

¡Con estos pasos, habrás configurado con éxito Wazuh para enviar alertas a Telegram!

- - - 

Si quieres añadir el bot a un grupo, entra en el siguiente enlace:

https://sean-bradley.medium.com/get-telegram-chat-id-80b575520659

Pega el token de tu BOT y te responderá con un nuevo ID. 

Utiliza ese nuevo ID para configurar las notificaciones. 
