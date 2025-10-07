# Proyecto 2.2 - SASE/ZTNA Casero con Túneles por Usuario (WireGuard/IPsec)

## 🧠 Descripción general
Implementación de un concentrador de acceso remoto bajo el modelo **Zero Trust Network Access (ZTNA)**, donde cada usuario obtiene un túnel dedicado mediante **WireGuard** (o IPsec), con políticas L3/L4 específicas según su rol.  
El entorno emula un **SASE casero**, donde ninguna red interna es expuesta por defecto y el acceso se otorga bajo el principio de **mínimo privilegio**.

---

## 👥 Integrantes
- **Camilo Iván Palacio Pérez - 2224643**
- **Daniel**

---

## 🎯 Objetivo general
Diseñar e implementar una arquitectura **SASE/ZTNA** doméstica que otorgue acceso remoto seguro mediante túneles dedicados, políticas por identidad y observabilidad básica.

### Objetivos específicos
- Configurar un concentrador ZTNA (VyOS/pfSense) con zonas WAN/Inside.  
- Establecer túneles dedicados (WireGuard/IPsec) para tres roles: Dev, Soporte e Invitado.  
- Aplicar políticas L3/L4 por rol (firewall con estado).  
- Implementar split-tunnel y registros de conexión.  
- Validar accesos permitidos y denegados por usuario.

---

## 🧱 Topología general
```text
CLIENTE DEV       CLIENTE SOPORTE       CLIENTE INVITADO
     │                  │                     │
     └──── Internet ─────┬─────────────────────┘
                         │
                    [ZTNA-HUB]
                 (VyOS / pfSense)
                WAN ↔ Internet
                INSIDE ↔ 10.20.0.0/24
                     │
                 [APP-SRV]
          (Git / CMDB / SSH)
