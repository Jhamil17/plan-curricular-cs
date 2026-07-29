### SIS-502 — Redes de Computadoras: Protocolos y Arquitectura

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-201, MAT-104 |
| **ADN institucional** | Stanford CS144 · MIT 6.829 |

**Competencia terminal.** Implementa una pila de protocolos desde la especificación y razona sobre control de congestión con modelos analíticos.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Capas física y enlace | Codificación Manchester, 4B5B · Modulación · Ethernet: CSMA/CD, exponential backoff con análisis de carga · Switching · STP · VLAN |
| 2 | 4–6 | Capa de red | IPv4 e IPv6 · CIDR y agregación · Fragmentación · TTL · NAT · ICMP · Forwarding vs routing |
| 3 | 7–9 | Enrutamiento | RIP como Bellman-Ford distribuido · OSPF como Dijkstra distribuido · BGP como path vector · Políticas y estabilidad · Convergencia y bucles transitorios |
| 4 | 10–12 | Transporte | Máquina de estados completa de TCP · Three-way handshake · Control de flujo por ventana deslizante · Control de congestión: AIMD, slow start, congestion avoidance, CUBIC, BBR · Modelo analítico de throughput de TCP · UDP |
| 5 | 13–15 | Aplicación y seguridad de transporte | DNS: jerarquía, resolución iterativa vs recursiva, caché · HTTP/1.1, HTTP/2 con HPACK, HTTP/3 sobre QUIC · TLS 1.3: handshake, ECDHE · SDN y OpenFlow · DHT (Kademlia), BitTorrent |

**Prueba de Dominio.** Router IP con tabla de enrutamiento y plano de forwarding + implementación de TCP sobre UDP en espacio de usuario, con control de congestión AIMD, retransmisión con estimación adaptativa de RTT y detección de pérdidas. Evaluado bajo pérdida, reordenamiento y latencia variable inyectadas.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria, con el escalamiento declarado respecto al número de flujos concurrentes y al tamaño de la tabla de enrutamiento. El número que decide algo es la **memoria por conexión**: multiplicada por los flujos concurrentes fija el techo de conexiones simultáneas, y es la cantidad que dimensiona la ventana de recepción y el buffer de reensamblado. Un techo que se descubre por agotamiento en producción es el techo que este criterio existe para calcular antes.

**Bibliografía.**
- **Base:** *Computer Networks: A Top-Down Approach* (8ª ed.) — Kurose & Ross
- **Complementaria:** *Computer Networks: A Systems Approach* — Peterson & Davie (gratuito) · *TCP/IP Illustrated, Vol. 1* — Fall & Stevens
- **Papers:** *"Congestion Avoidance and Control"* — Jacobson & Karels (SIGCOMM 1988) · *"BBR: Congestion-Based Congestion Control"* — Cardwell et al. (ACM Queue 2016)

**Recursos.** cs144.github.io (labs completos de construcción de TCP) · systemsapproach.org (libro gratuito) · Wireshark · mininet · RFCs 793, 9293, 9000 (QUIC), 8446 (TLS 1.3).

**Protocolo de estudio.** Toda máquina de estados se dibuja de memoria antes de implementarla. La captura con Wireshark se contrasta siempre contra la predicción hecha leyendo el RFC — nunca al revés.

---

