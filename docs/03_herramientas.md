# 03 - Herramientas y tecnologías

## Software principal

| **Componente** | **Herramienta / Sistema** | **Función dentro del proyecto** |
|-----------------|---------------------------|----------------------------------|
| **ZTNA Hub (Concentrador central)** | **VyOS** | Actúa como firewall y VPN hub. Aplica políticas L3/L4 por usuario y gestiona los túneles WireGuard. |
| **VPN Túneles** | **WireGuard** | Proporciona conexión segura punto a punto entre el hub y cada cliente (Dev, Soporte, Invitado). |
| **Servidor interno** | **Ubuntu Server** + **Apache / SSH / Git** | Simula los servicios internos accesibles por los distintos roles: repos Git, CMDB y acceso SSH. |
| **Clientes remotos** | **Linux (Xubuntu VM)** y **Windows 10/11** | Equipos desde los cuales se conectan los usuarios mediante WireGuard según su rol. |
| **Simulación de red** | **GNS3** | Emula la topología completa, permite probar conectividad, túneles y políticas sin usar múltiples equipos físicos. |
| **Telemetría y observabilidad** | **Logs del VyOS (firewall/VPN)** + **Syslog local** | Registra eventos, conexiones y contadores por política para validar las reglas. |
| **Control de versiones y documentación** | **GitHub** | Repositorio central con configuraciones, diagramas, scripts y evidencias del proyecto. |

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

