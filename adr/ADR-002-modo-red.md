ADR-002 — Modo de red

Contexto:
La máquina virtual necesita acceso a Internet y también debe poder ser accedida desde el equipo anfitrión.

Opciones consideradas:

Adaptador puente
NAT
NAT + Host-only

Decisión:
Se utilizará una combinación de NAT + Host-only.

Justificación:
El adaptador NAT se utilizará para brindar acceso a Internet a la máquina virtual, mientras que Host-only permitirá la comunicación directa entre el equipo anfitrión y la VM. Esta configuración resultó más estable que el uso de adaptador puente.

Consecuencia:
La máquina virtual tendrá dos interfaces de red: una para salida a Internet y otra para las pruebas de conectividad con el equipo anfitrión.
