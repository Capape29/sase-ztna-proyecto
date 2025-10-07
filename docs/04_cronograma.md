# 04 - Cronograma de trabajo

## Planificación general

| Semana | Actividad | Responsable | Entregable |
|--------|------------|--------------|-------------|
| **30 Sep – 5 Oct** | Preparar documentación base: resumen, objetivos, diseño y diagrama de red (PlantUML). | Ambos | Documento de avance inicial. |
| **6 – 8 Oct** | Instalar laboratorio virtual (VyOS o pfSense + 1 cliente Dev) y probar conectividad básica vía ping. | Integrante 1 | Entorno montado y primera conexión. |
| **9 Oct** | **Entrega del avance:** Documentación + Diagrama + Prueba funcional del túnel Dev (WireGuard/IPsec). | Ambos | Informe en GitHub + evidencia (captura/log). |
| **10 – 15 Oct** | Añadir usuarios Soporte e Invitado con IPs y políticas iniciales. | Integrante 2 | Configs actualizadas. |
| **16 – 22 Oct** | Implementar ACLs L3/L4 (firewall VyOS/pfSense) por usuario. | Integrante 1 | Pruebas de acceso/bloqueo. |
| **23 – 27 Oct** | Configurar split-tunnel y observabilidad (logs, contadores). | Integrante 2 | Logs funcionales y métricas. |
| **28 Oct – 3 Nov** | Validación completa de roles (Dev, Soporte, Invitado). | Ambos | Evidencias y capturas. |
| **4 – 6 Nov** | Grabación de video mostrando accesos y bloqueos. | Ambos | Video final (≤8 min). |
| **7 Nov** | **Entrega final del proyecto.** | - | Documentación, configs, logs y video. |

---

## 💡 Avance del 9 de octubre – Alcance técnico
Para esta entrega, se mostrará:
1. **ZTNA Hub operativo** con dos interfaces (WAN/Inside).  
2. **Túnel activo** para el usuario **Dev (172.16.0.10)**.  
3. Conectividad validada mediante **ping o curl** hacia el servicio interno Git (HTTP o SSH).  
4. Evidencia de conexión (log de WireGuard o captura de pantalla).  

---

## Control de versiones
- Cada avance se documentará en el repositorio GitHub (`/docs`).
- Configuraciones se subirán a `/configs/vyos` y `/configs/wireguard`.
- Evidencias (logs, capturas) se guardarán en `/evidencias/dev/`.

