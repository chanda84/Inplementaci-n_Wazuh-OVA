# Implementación de Wazuh en laboratorio de ciberseguridad

## 🧭 Introducción

Este entorno de laboratorio de ciberseguridad está diseñado para fortalecer capacidades defensivas y ofensivas mediante la integración de herramientas clave en el monitoreo, análisis e inteligencia de amenazas. 

La presente guía documenta el proceso de instalación, configuración y puesta en marcha de **Wazuh** utilizando su imagen en formato OVA, desplegada sobre una máquina virtual local.

## 🧰 Entorno del laboratorio

El laboratorio se encuentra compuesto por las siguientes máquinas y componentes:

- 🐱 Kali Linux (básico y Purple Team)
- 🔍 OpenCTI (Cyber Threat Intelligence)
- 📊 ElasticSearch, Kibana y Filebeat (stack de visualización y análisis)
- 🛡️ Wazuh (detección y respuesta ante amenazas)
- 💥 Máquinas de pentesting específicas por escenarios
- 🔧 Redmux (administración remota del entorno)

## 🎯 Rol de Wazuh en el entorno

Wazuh actúa como núcleo de **detección, análisis y correlación de eventos** de seguridad dentro del laboratorio. Permite:

- Registro y gestión centralizada de agentes
- Análisis de integridad de archivos
- Recolección de logs y alertas en tiempo real
- Integración directa con el stack Elastic para visibilidad avanzada
- Soporte para cumplimiento normativo (PCI DSS, HIPAA, etc.)
- Monitoreo continuo de endpoints y servidores

## ⚙️ Instalación rápida de la OVA

1. Descargar el archivo `wazuh-4.12.0.ova` desde el sitio oficial
2. Importar en VirtualBox y configurar:
   - Controlador gráfico: `VMSVGA`
   - Adaptador de red: `Puente`
   - Reloj del sistema: `UTC`
3. Iniciar la VM y acceder:
   - Usuario: `wazuh-user`
   - Contraseña: `wazuh`
   - Dashboard: `https://<IP_VM>`
     - Usuario: `admin`
     - Contraseña: `admin`
4. Configurar agentes desde `manage_agents` y validar conectividad

## 📎 Conclusiones

Con esta implementación, se fortalece la capacidad del laboratorio para:
- Simular y detectar amenazas en entornos controlados
- Realizar ejercicios de Red/Blue Team de manera estructurada
- Probar integraciones con fuentes de inteligencia como OpenCTI
- Evaluar tiempos de respuesta y efectividad de alertas

Wazuh se convierte así en una pieza clave para **experimentación, monitoreo y evaluación proactiva de seguridad** en entornos de prueba avanzados.

