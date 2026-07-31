# SOC-Alert-Orchestrator

<img width="400" height="200" alt="n8n-cover CeY7WiF5" src="https://github.com/user-attachments/assets/d91f406e-f1eb-4c5c-a660-01fc40e539df" /> <img width="350" height="220" alt="wazuh" src="https://github.com/user-attachments/assets/e21130e2-225c-41c4-a3b6-4257cb57fe34" />




Este proyecto nace con el objetivo de demostrar como la automatizacion puede optimizar los procesos de un Centro de operaciones de Seguridad (SOC)

Para ello dentro de mi [HomeLab-SOC](https://github.com/Lucasjavier708/HomeLab-SOC.git) desarrollo distintos escenarios de ataques para validar las capacidades de deteccion , analisis y respuesta automatizada. 

A través de un flujo automatizado, el proyecto recibe alertas de seguridad, las enriquece con fuentes de Threat Intelligence y facilita el análisis inicial del incidente reduciendo los tiempos de evaluación. 

La solución integra Wazuh como plataforma SIEM, n8n como motor de automatización SOAR y Jira como plataforma de gestión de incidentes, donde se documentan y notifican automáticamente los eventos relevantes, comunicándose mediante una red privada (VPN) utilizando WireGuard.


El objetivo es reproducir el flujo operativo de un analista SOC durante las primeras etapas de gestión de un incidente:

- Recepción de alertas y triage.
- Enriquecimiento mediante fuentes de Threat Intelligence.
- Correlación de la información obtenida.
- Documentación automática de los   incidentes relevantes mediante Jira como plataforma de ticketing.


