# <center>  FULLSIEMBuzzi </center>

![buzzi](/img/buzzi.png)

# ÍNDICE

- 1.-Descripción del proyecto.
- 2.-Introducción teórica
- 3.-Mapa.
- 4.-Herramientas utilizadas.
- 5.-Desarrollo del proyecto con detalle.
- 6.-Conclusiones y dificultades encontradas en el proyecto.
- 7.-Referencias utilizadas.

## Mapa


![mapa](/img/map.png)


## Desarrollo del Proyecto:

   1.- **Instalación Wazuh**.- [Click Aquí](https://documentation.wazuh.com/current/installation-guide/index.html)

   - 1.1.- Configuración Agente Wazuh - [Click Aquí](https://documentation.wazuh.com/current/installation-guide/wazuh-agent/index.html)
 

   2.- **Instalación Grafana** - [Click Aquí](Guia/conf-grafana)
   
   - 2.1 Dashboard - [Click Aquí](Guia/Dashboard.json)
     
   3.- **Integraciones:**

   - 3.1.- Integración con Alertas Telegram - [Click Aquí](Guia/conf-telegram.md)

   - 3.2.- Integración Virus Total - [Click Aquí](https://documentation.wazuh.com/current/user-manual/capabilities/malware-detection/virus-total-integration.html)
   - 3.3.- Integracion con Maltiverse - [Click Aquí](https://documentation.wazuh.com/current/user-manual/manager/manual-integration.html#maltiverse)
   - 3.4.- Instalación Suricata - [Click Aquí](https://github.com/Scosrom/Suricata-Telegram/blob/main/README.md)  - ¡(No realizar el paso 3 marcado como Opcional)!
      - 3.4.1- Configuración suricata Agente - [Click Aquí](Guia/conf-suricata.md)
   - 3.5.- Integración con ManoliBot Telegram - [Click Aquí](https://github.com/Scosrom/ManoliBot-Telegram)  - ¡(No instalar DLCs, están integrados en Wazuh)! 
