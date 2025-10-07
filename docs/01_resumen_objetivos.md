
---

## 📘 **2️⃣ `docs/01_resumen_objetivos.md`**

```markdown
# 01 - Resumen y Objetivos

## Introducción
El proyecto 2.2 busca implementar una arquitectura **SASE/ZTNA casera** que permita un acceso remoto seguro basado en identidad.  
Cada usuario obtiene un túnel dedicado (WireGuard/IPsec) con políticas L3/L4 que controlan estrictamente qué servicios internos puede acceder, eliminando la exposición de la red interna.

## Justificación
El modelo tradicional de VPN otorga acceso amplio a toda la red.  
El enfoque **Zero Trust Network Access (ZTNA)** elimina la confianza implícita, otorgando acceso únicamente a los recursos necesarios.  
Este laboratorio permite comprender los fundamentos de **SASE (Secure Access Service Edge)** y su aplicación práctica usando herramientas libres.

## Objetivo general
Diseñar e implementar un entorno ZTNA con control de acceso granular y observabilidad básica, aplicando los principios de Zero Trust.

## Objetivos específicos
- Desplegar un concentrador ZTNA con zonas WAN/Inside.  
- Configurar túneles WireGuard/IPsec con asignación individual de IP.  
- Aplicar ACLs por rol (Dev, Soporte, Invitado).  
- Implementar split-tunnel y telemetría.  
- Validar accesos y bloqueos mediante pruebas por rol.

