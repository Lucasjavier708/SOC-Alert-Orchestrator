
<img width="1580" height="490" alt="Orch-SOc" src="https://github.com/user-attachments/assets/4db3a239-d73a-4469-a29f-ff0387a5b185" />




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


# Arquitectura

Arquitectura del Laboratorio 

- En la red de laboratorio se ejecutan los escenarios de ataques. Los agantes de wazuh monitorean la actividad y mandan las alertas al SIEM
- EN la red de estudio esta el Wazuh manager particularmente en en la PC de estudio , este recibe las alertas por los agentes y las envia al nodo de automatizacion para su procesamiento
- En la Pc 5 se encuentra el woorkflow de automatizacion , donde las alertas son procesadas , enriquecidas , con threat intelligence , correlacionadas y documentadas automaticamente en jira , quedando lista para su analisis

<p align="center">
  <img width="1500 height="300" alt="infra de proyecto SOC-Autom-Play (2)" src="https://github.com/user-attachments/assets/2b4a8415-b066-4927-bada-dd44761823ed" />

</p>


