
<h1 align="center">🚦   FULLSIEMBuzzi  🚦 </h1>




![buzzi](/img/buzzi.png)

<h2 align="center">  ÍNDICE  </h2>

- 1.-Descripción del proyecto.
- 2.-Mapa.
- 3.-Introducción teórica
- 4.-Herramientas utilizadas.
- 5.-Desarrollo del proyecto con detalle.
- 6.-Conclusiones y dificultades encontradas en el proyecto.
- 7.-Referencias utilizadas.

<h2 align="center">  DESCRIPCIÓN DEL PROYECTO  </h2>

FULLSIEMBuzzi es una solución integral de gestión de información y eventos de seguridad (SIEM) que combina varias herramientas avanzadas de monitoreo, visualización y análisis de seguridad. El objetivo del proyecto es proporcionar una plataforma robusta que permita a las organizaciones detectar, analizar y responder a incidentes de seguridad de manera eficiente.

Las principales características del proyecto incluyen:

- **Wazuh:** Plataforma de SIEM y monitorización de seguridad que permite la detección de intrusiones, análisis de integridad de archivos, monitorización de logs y gestión de vulnerabilidades.

- **Grafana:** Herramienta de visualización de datos que permite crear dashboards interactivos para la visualización en tiempo real de métricas y datos de seguridad.

- **Suricata:** Motor de detección y prevención de intrusiones que analiza el tráfico de red en busca de patrones maliciosos.

- **Alertas a través de Telegram:** Envío de alertas de seguridad directamente a un canal o grupo de Telegram para una comunicación inmediata.

- **VirusTotal y Maltiverse:** Análisis automatizado de archivos y URLs contra bases de datos de amenazas conocidas para mejorar la detección de malware y sitios maliciosos.

- **ManoliBot:** Bot de Telegram que permite la ejecución de comandos en el servidor desde la plataforma de mensajería, facilitando la administración remota y la respuesta rápida a incidentes.

FULLSIEMBuzzi proporciona una solución completa y eficiente para la gestión de la seguridad en redes, integrando tecnologías avanzadas y facilitando una respuesta rápida y efectiva a los incidentes de seguridad.



<h2 align="center">  MAPA </h2>


![mapa](/img/map.png)

<h2 align="center">  INTRODUCCIÓN TEÓRICA  </h2>

**TL;DR**: Este proyecto integra múltiples herramientas de seguridad como Wazuh, Grafana, Suricata, y más, para crear un sistema de monitoreo y respuesta a incidentes de seguridad eficiente y completo. 

 - [Descripción detallada](/Guia/descripcion-detallada.md)



<h2 align="center">  DESARROLLO DEL PROYECTO  </h2>

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

