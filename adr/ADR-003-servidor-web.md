ADR-003 — Servidor web / proxy inverso

Contexto:
La aplicación debe publicarse mediante un servidor web o proxy inverso, de acuerdo con los requisitos del trabajo práctico.

Opciones consideradas:

Nginx
Apache HTTP Server
Caddy

Decisión:
Se utilizará Nginx como proxy inverso.

Justificación:
Nginx es una opción liviana, ampliamente utilizada y adecuada para recibir las solicitudes HTTP/HTTPS y redirigirlas hacia el servidor de aplicación. Además, permitirá configurar posteriormente TLS, cabeceras de seguridad, redirecciones y registros de acceso.

Consecuencia:
Nginx será el punto de entrada de la aplicación en los puertos 80 y 443, mientras que Healthchecks se ejecutará detrás del proxy mediante el servidor de aplicación.
