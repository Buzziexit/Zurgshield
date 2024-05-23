
<h1 align="center">🛡️   FULLSIEMBuzzi  🛡️ </h1>




![buzzi](/img/buzzi.png)

<h2 align="center"> 🪧 ÍNDICE 🪧</h2>

- 1.-Descripción del proyecto.
- 2.-Mapa.
- 3.-Introducción teórica
- 4.-Herramientas utilizadas.
- 5.-Desarrollo del proyecto con detalle.
- 6.-Conclusiones y dificultades encontradas en el proyecto.
- 7.-Referencias utilizadas.

<h2 align="center"> 📝 DESCRIPCIÓN DEL PROYECTO 📝 </h2>

FULLSIEMBuzzi es una solución integral de gestión de información y eventos de seguridad (SIEM) que combina varias herramientas avanzadas de monitoreo, visualización y análisis de seguridad. El objetivo del proyecto es proporcionar una plataforma robusta que permita a las organizaciones detectar, analizar y responder a incidentes de seguridad de manera eficiente.

Las principales características del proyecto incluyen:

- **Wazuh:** Plataforma de SIEM y monitorización de seguridad que permite la detección de intrusiones, análisis de integridad de archivos, monitorización de logs y gestión de vulnerabilidades.

- **Grafana:** Herramienta de visualización de datos que permite crear dashboards interactivos para la visualización en tiempo real de métricas y datos de seguridad.

- **Suricata:** Motor de detección y prevención de intrusiones que analiza el tráfico de red en busca de patrones maliciosos.

- **Alertas a través de Telegram:** Envío de alertas de seguridad directamente a un canal o grupo de Telegram para una comunicación inmediata.

- **VirusTotal y Maltiverse:** Análisis automatizado de archivos y URLs contra bases de datos de amenazas conocidas para mejorar la detección de malware y sitios maliciosos.

- **ManoliBot:** Bot de Telegram que permite la ejecución de comandos en el servidor desde la plataforma de mensajería, facilitando la administración remota y la respuesta rápida a incidentes.
  
- **The Hive con Cortex:** Sistema de gestión de tickets que facilita la organización y seguimiento de incidentes de seguridad, integrando análisis automatizados y enriquecimiento de datos para mejorar la respuesta a incidentes.



FULLSIEMBuzzi proporciona una solución completa y eficiente para la gestión de la seguridad en redes, integrando tecnologías avanzadas y facilitando una respuesta rápida y efectiva a los incidentes de seguridad.



<h2 align="center"> 🗺️ MAPA 🗺️ </h2>


![mapa](/img/mapa1.png)



<h2 align="center"> 📓📌 INTRODUCCIÓN TEÓRICA 📌📓 </h2> 

**TL;DR**: Este proyecto integra múltiples herramientas de seguridad como Wazuh, Grafana, Suricata, y más, para crear un sistema de monitoreo y respuesta a incidentes de seguridad eficiente y completo. 

 - [Introducción detallada](/Guia/introduccionTeorica.md)



<h2 align="center"> 🔌🛠️ DESARROLLO DEL PROYECTO 🛠️🔌 </h2>

   1.- **Instalación Wazuh**.- [Click Aquí](https://documentation.wazuh.com/current/installation-guide/index.html)

   - 1.1.- Configuración Agente Wazuh - [Click Aquí](https://documentation.wazuh.com/current/installation-guide/wazuh-agent/index.html)
 

   2.- **Instalación Grafana** - [Click Aquí](https://github.com/Scosrom/monitorizacion/blob/master/graf.md)
   
   - 2.1 Dashboard - [Click Aquí](Guia/Dashboard.json)
     
   3.- **Integraciones:**

   - 3.1.- Integración con Alertas Telegram - [Click Aquí](Guia/conf-telegram.md)

   - 3.2.- Integración Virus Total - [Click Aquí](https://documentation.wazuh.com/current/user-manual/capabilities/malware-detection/virus-total-integration.html)
   - 3.3.- Integracion con Maltiverse - [Click Aquí](https://documentation.wazuh.com/current/user-manual/manager/manual-integration.html#maltiverse)
   - 3.4.- Instalación Suricata - [Click Aquí](https://github.com/Scosrom/Suricata-Telegram/blob/main/README.md)  - ¡(No realizar el paso 3 marcado como Opcional)!
      - 3.4.1- Configuración suricata Agente - [Click Aquí](https://documentation.wazuh.com/current/proof-of-concept-guide/integrate-network-ids-suricata.html)
   - 3.5.- Integración con ManoliBot Telegram - [Click Aquí](https://github.com/Scosrom/ManoliBot-Telegram)  - ¡(No instalar DLCs, están integrados en Wazuh)!st

   4.- **Instalación de The Hive y Cortex**: [Click Aquí](https://docs.thehive-project.org/thehive/legacy/thehive3/installation/install-guide/#docker) 
   
   - 4.1- Configuración de Wazuh con The Hive - [Click Aquí](https://wazuh.com/blog/using-wazuh-and-thehive-for-threat-protection-and-incident-response/)

<h2 align="center"> ⚔️💡 CONCLUSIONES Y DESAFÍOS EN EL PROYECTO 💡⚔️ </h2>


<h3 align="center">  CONCLUSIONES </h3>

La creación y despliegue de FULLSIEMBuzzi ha sido un paso significativo hacia una gestión de seguridad más efectiva en entornos digitales. Esta solución integral ofrece una herramienta potente para detectar, analizar y responder a amenazas de seguridad de manera eficiente. Al combinar tecnologías avanzadas como Wazuh, Suricata, Grafana y otras, FULLSIEMBuzzi proporciona una visión completa y un control mejorado sobre la infraestructura de TI, permitiendo una defensa proactiva contra las crecientes amenazas cibernéticas.

Los principales logros del proyecto incluyen:

- **Mejora en la Respuesta a Incidentes:** La integración de diversas herramientas y la capacidad de recibir alertas en tiempo real han mejorado significativamente los tiempos de respuesta a incidentes. Esto permite actuar de manera rápida y efectiva para mitigar posibles daños.

- **Visualización Avanzada de Datos:** La implementación de Grafana ha facilitado la creación de dashboards interactivos para monitorear métricas y datos de seguridad en tiempo real. Esta capacidad de visualización mejora la comprensión de la situación de seguridad y facilita la toma de decisiones informadas.

- **Flexibilidad y Movilidad:** FULLSIEMBuzzi proporciona la capacidad de mantener el control sobre los sistemas desde cualquier ubicación. La integración con Telegram y el desarrollo de ManoliBot permiten recibir alertas y ejecutar comandos desde dispositivos móviles, garantizando una respuesta rápida incluso fuera de la oficina.

---
<h3 align="center">  DESAFÍOS  </h3> 

Durante el desarrollo de FULLSIEMBuzzi, me encontré con varios desafíos técnicos que requerían soluciones creativas:

- **Limitaciones de IPs Estáticas en AWS:** AWS ofrece la opción de tener IPs estáticas, pero implica costos adicionales que quería evitar, especialmente en un proyecto con recursos limitados como mi laboratorio estudiantil. Para resolver esto, implementé ZeroTier, una solución que me permitió mantener la conectividad sin incurrir en costos adicionales.

- **Compatibilidad con OpenSearch y Grafana:** La migración de Wazuh a OpenSearch presentó dificultades de compatibilidad con Grafana. Descubrí que el plugin de OpenSearch en Grafana no funcionaba correctamente, por lo que opté por utilizar el plugin de Elasticsearch, que demostró ser más compatible y confiable.

- **Limitaciones del Sistema de Monitorización:** Aunque el sistema de alertas a través de Telegram era útil, enfrenté limitaciones cuando no tenía acceso a un PC para responder a los incidentes. Para superar esto, desarrollé ManoliBot, una herramienta que me permite ejecutar comandos directamente desde mis dispositivos móviles, proporcionando una respuesta rápida y efectiva en cualquier situación.

En resumen, el proyecto FULLSIEMBuzzi ha demostrado ser una solución efectiva para la gestión de seguridad en redes, superando desafíos técnicos con soluciones prácticas y adaptativas. Las lecciones aprendidas durante el proceso de desarrollo me han permitido crear una plataforma sólida y flexible, capaz de adaptarse a las necesidades cambiantes de seguridad cibernética en entornos dinámicos como el mío.


<h2 align="center"> 🎖️ REFERENCIAS 🎖️  </h2> 


<p align="center">
  <a href="https://prometheus.io/docs/introduction/overview/">
    <img src="/img/virustotal_logo_icon_170249.png" alt="VirusTotal">
  </a>
 
  <a href="https://grafana.com/docs/grafana/latest/">
    <img src="/img/grafana_logo_icon_171049.png" alt="Grafana Documentation">
  </a>
  
  <a href="https://www.debian.org/doc/index.es.html">
    <img src="/img/telegram_logo_icon_168691.png" alt="Telegram Documentation">
  </a>

   <a href="https://www.debian.org/doc/index.es.html">
    <img src="https://asset.brandfetch.io/idGBqJSmMa/idNog5T5UD.svg" alt="wazuh Documentation">
  </a>
</p>



<h2 align="center"> Licencia  </h2>

<p align="center">
  <img src="/img/88x31.png" alt="licencia">
</p>




