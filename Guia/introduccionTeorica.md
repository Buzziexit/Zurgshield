En un entorno de TI moderno, la seguridad de la información es una preocupación crítica para las organizaciones. Los SIEMs son sistemas diseñados para recopilar, analizar y presentar datos de eventos de seguridad en tiempo real, facilitando la detección y respuesta a amenazas. A continuación, se detalla la teoría detrás de cada componente clave del proyecto FULLSIEMBuzzi:

### **Wazuh**

**Wazuh** es una plataforma de SIEM y monitorización de seguridad que permite la detección de intrusiones, el análisis de integridad de archivos, la monitorización de logs y la gestión de vulnerabilidades. Su arquitectura se basa en agentes que se instalan en los sistemas monitorizados y un servidor central que recopila y analiza los datos.

- **Instalación y Configuración de Wazuh:** La instalación de Wazuh implica la configuración de un servidor maestro que recopila datos de seguridad desde múltiples agentes instalados en diferentes hosts. La configuración del agente Wazuh se realiza en cada sistema objetivo para asegurar que los datos relevantes se envíen al servidor maestro.
  
### **Grafana**

- **Grafana** es una herramienta de visualización de datos que permite crear y compartir dashboards interactivos. En el contexto de un SIEM, Grafana se utiliza para visualizar métricas y datos de seguridad en tiempo real, lo que facilita la identificación y análisis de incidentes.

- **Dashboards en Grafana:** Los dashboards personalizados en Grafana muestran datos críticos de seguridad y ayudan a los administradores a entender rápidamente el estado de seguridad de la red.
Integraciones de Alertas y Análisis de Amenazas
Las integraciones adicionales mejoran la funcionalidad del SIEM al proporcionar capacidades avanzadas de alerta y análisis:

- **Alertas a través de Telegram:** Integrar Wazuh con Telegram permite que las alertas de seguridad sean enviadas directamente a un canal o grupo de Telegram, facilitando la comunicación inmediata de incidentes críticos.

- **VirusTotal y Maltiverse:** Estas integraciones permiten el análisis automatizado de archivos y URLs contra bases de datos de amenazas conocidas, mejorando la capacidad de detección de malware y sitios maliciosos.

### **Suricata**

Suricata es un motor de detección de intrusiones (IDS) y prevención de intrusiones (IPS) que analiza el tráfico de red en busca de patrones maliciosos.

- **Instalación y Configuración de Suricata:** La integración de Suricata con Wazuh permite la detección avanzada de amenazas en la red, aportando una capa adicional de seguridad al entorno.

### **ManoliBot**

**ManoliBot** es un bot de Telegram que permite la ejecución de comandos en el servidor desde la plataforma de mensajería. Esta funcionalidad es crucial para la administración remota y la respuesta rápida a incidentes.
