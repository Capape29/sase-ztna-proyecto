# 03 - Herramientas y tecnologías

## Software principal

| Componente | Herramienta | Descripción |
|-------------|--------------|--------------|
| **ZTNA Hub** | VyOS / pfSense / OPNsense | Firewall/VPN con ACLs y políticas L3/L4 |
| **VPN Túneles** | WireGuard (principal) / IPsec IKEv2 | Conexión segura y ligera por usuario |
| **Simulación de red** | VirtualBox / EVE-NG / GNS3 | Entorno virtual para desplegar los nodos |
| **Servidor interno** | Linux (Debian/Ubuntu) + Apache / SSH | Emula servicios Git, CMDB y SSH |
| **Clientes remotos** | Linux o Windows | Conectan al hub mediante WireGuard |
| **Telemetría y observabilidad** | Logs del firewall + Syslog | Registra conexiones y contadores por política |

---

## Hardware mínimo
| Elemento | Recurso estimado |
|-----------|------------------|
| CPU | 2 núcleos |
| RAM | 4 GB |
| Almacenamiento | 20 GB |
| NICs | 2 (WAN e Inside) |

---

## Herramientas de apoyo
- **draw.io / PlantUML** → para diagramas.  
- **GitHub** → control de versiones y documentación.  
- **Wireshark / tcpdump** → verificación de túneles.  
- **Ping / curl / ssh** → validación de conectividad y políticas.

