## Configurar Grafana con Wazuh.

Paso 1. Añaidr una nueva base de datos Elasticsearch.

![image](https://github.com/Buzziex/FULLSIEMBuzzi/assets/114906778/adc94f5b-a8de-417c-9a28-4468665f8c40)

Paso 2. Configurar Elasticsearch. 

![image](https://github.com/Buzziex/FULLSIEMBuzzi/assets/114906778/45b9507d-2dd7-4c57-a12f-8d6f34a09276)

En la url tienes que poner **https**, y añadir un usuario con permisos de **administrador**
- Ejemplo:
  <code>https://administrador:contraseña@ip-de-tu-wazuh:9200</code>


En la configuracion de la Autenticación configurar así:

![image](https://github.com/Buzziex/FULLSIEMBuzzi/assets/114906778/0b8bd526-6dac-4743-99ab-ce1058215fc1)

- Marcamos **Basic Authentication** y **Skip TLS certificate validation**. 
- Añadimos nuestro usuario administrador y la contraseña ( Es la misma que para entrar en el Dashboard de Wazuh )


![image](https://github.com/Buzziex/FULLSIEMBuzzi/assets/114906778/46200ceb-d16f-4bd2-bced-aeb0fde9c0d5)

En **Index name** añadimos <code>wazuh-alert*<code> para añadir todos los index con alertas. 
