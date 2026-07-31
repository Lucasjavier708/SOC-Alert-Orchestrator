
<img width="1500" height="480" alt="imagen" src="https://github.com/user-attachments/assets/e262e766-b143-46f9-a74b-be3824065dee" />


# SOC Automation Playbook |




Este proyecto nace con el objetivo de demostrar como la automatizacion puede optimizar los procesos de un Centro de operaciones de Seguridad (SOC)

Para ello dentro de mi [HomeLab-SOC](https://github.com/Lucasjavier708/HomeLab-SOC.git) desarrollo distintos escenarios de ataques para validar las capacidades de deteccion , analisis y respuesta automatizada. 

A través de un flujo automatizado, el proyecto recibe alertas de seguridad, las enriquece con fuentes de Threat Intelligence y facilita el análisis inicial del incidente reduciendo los tiempos de evaluación. 

La solución integra Wazuh como plataforma SIEM, n8n como motor de automatización  y Jira como plataforma de gestión de incidentes, donde se documentan y notifican automáticamente los eventos relevantes, comunicándose mediante una red privada (VPN) utilizando WireGuard.


El objetivo en este caso es  reproducir el flujo operativo de un analista SOC durante las primeras etapas de gestión de un incidente:

- Recepción de alertas y triage.
- Enriquecimiento mediante fuentes de Threat Intelligence.
- Correlación de la información obtenida.
- Documentación automática de los   incidentes relevantes mediante Jira como plataforma de ticketing.


