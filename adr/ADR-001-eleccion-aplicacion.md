ADR-001 — Elección de la aplicación

Contexto:
Se necesitaba seleccionar una aplicación web de código abierto que pudiera instalarse en una máquina virtual y que permitiera realizar pruebas de red, HTTP, seguridad, rendimiento y disponibilidad.

Opciones consideradas:

Healthchecks
Shlink

Decisión:
Se seleccionó Healthchecks.

Justificación:
Healthchecks ofrece una arquitectura web suficientemente completa para los objetivos del trabajo práctico. Permite trabajar con proxy inverso, servidor de aplicación, base de datos, puertos, HTTP y monitoreo mediante pings. Además, su complejidad es adecuada para el tiempo disponible.

Consecuencia:
El despliegue se realizará utilizando Healthchecks como aplicación principal.
