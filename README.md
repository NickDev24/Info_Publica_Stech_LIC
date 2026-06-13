# STECH VIAJES

**Plataforma Mediadora de Transporte Argentino**

[![Version](https://img.shields.io/badge/version-2.1.0-brightgreen)]()
[![License](https://img.shields.io/badge/license-Propietaria-blue)]()
[![Stack](https://img.shields.io/badge/stack-Next.js%2016%20%7C%20TypeScript%20%7C%20PostgreSQL%20%7C%20Redis-purple)]()

---

## Certificacion de titularidad y derechos de autor

Yo, **Facundo Maximiliano Cercuetti** (NickDev24), declaro bajo juramento ser el autor original, unico y legitimo propietario de la totalidad del codigo fuente, diseno, arquitectura, algoritmos, base de datos, interfaz de usuario, marca, nombre comercial, identidad visual y cualquier otro activo intelectual comprendido en el proyecto **STECH VIAJES** (en adelante, "el Sistema").

---

## Datos del proyecto

| Atributo | Valor |
|---|---|
| **Nombre del proyecto** | STECH VIAJES |
| **Version** | 2.1.0 |
| **Fecha de inicio del desarrollo** | 05 de mayo de 2026 |
| **Fecha del primer deploy en produccion** | 10 de junio de 2026 — 05:49 ART (GMT-3) |
| **Infraestructura de produccion** | AWS EC2 (Ubuntu) + Docker + Cloudflared Tunnel |
| **Autor / Titular** | Facundo Maximiliano Cercuetti |
| **Alias** | NickDev24 |
| **Repositorio privado oficial** | [https://github.com/NickDev24/Stech-Viajes-Oficial](https://github.com/NickDev24/Stech-Viajes-Oficial) |

---

## Funcionalidades principales

### Para clientes
- Solicitud de viajes con precio fijo (sin tarifa dinamica)
- Seguimiento en vivo del conductor en el mapa
- Viajes compartidos (car pooling) — hasta 4 pasajeros
- Wallet digital con recarga via Mercado Pago / Mobbex
- Suscripcion semanal con descuento
- Puntos de fidelidad y codigos promocionales

### Para conductores
- Recepcion y gestion de solicitudes de viaje
- Navegacion integrada paso a paso
- Ganancias en tiempo real con comision justa
- Verificacion de identidad con selfie + DNI
- Notas internas privadas para el admin
- Cancelacion segura en zona peligrosa con registro GPS
- Recargos por demora y pago insuficiente
- Carrusel de comercios afiliados con cupones de descuento
- Notificaciones push en tiempo real (SSE + FCM)

### Para comercios afiliados
- Creacion y gestion de cupones de descuento
- Canje mediante codigo QR o codigo numerico
- Control de stock, fechas de validez y limites de uso
- Notificaciones en tiempo real a conductores

### Para administradores
- Panel de control con mapa en tiempo real
- Gestion integral de usuarios, viajes y finanzas
- Dashboard de analitica con metricas clave
- Sistema de soporte con chat integrado

---

## Arquitectura del sistema (vista general)

> Esta descripcion contiene informacion de alto nivel. Los detalles de implementacion, algoritmos propietarios y logica de negocio forman parte del secreto comercial.

| Componente | Descripcion |
|---|---|
| **Panel Administrativo** | Gestion integral de usuarios, viajes, finanzas, promociones, validaciones, soporte tecnico, analitica y configuracion del sistema. Incluye panel de control en tiempo real con mapas de seguimiento de unidades. |
| **App Cliente (PWA)** | Plataforma para que los usuarios soliciten, gestionen y paguen viajes. Incluye seleccion de destino, seguimiento en vivo del conductor, historial de viajes, sistema de calificaciones, wallet digital y programas de suscripcion semanal. |
| **App Conductor (PWA)** | Plataforma para que los conductores reciban y gestionen solicitudes de viaje. Incluye mapas de navegacion paso a paso, comunicacion en tiempo real con pasajeros, registro de earnings diarios, verificacion de identidad y panel de disponibilidad. |
| **Motor de geolocalizacion** | Sistema de geocodificacion y busqueda de direcciones optimizado para el norte argentino (NOA), con soporte para alias locales, coordenadas, intersecciones y puntos de interes regionales. |
| **Infraestructura en tiempo real** | Sistema de comunicacion bidireccional mediante Server-Sent Events (SSE) y Redis Pub/Sub para actualizaciones instantaneas de estado de viajes, ubicacion de conductores y mensajeria. |
| **Pasarela de pagos** | Integracion con multiples procesadores de pago (Mercado Pago, Mobbex) para procesar pagos con tarjeta, transferencias y recargas de wallet. |
| **Infraestructura cloud** | Desplegado en AWS EC2 con Docker, respaldado por Supabase (PostgreSQL), Redis, Cloudflared Tunnel, y notificaciones push via Firebase Cloud Messaging. |

---

## Tecnologias utilizadas

| Tecnologia | Version | Proposito |
|---|---|---|
| Next.js | 16 | Framework principal (3 aplicaciones) |
| TypeScript | ~5.8 | Lenguaje de programacion |
| Prisma ORM | ~6.6 | Capa de base de datos |
| PostgreSQL (Supabase) | — | Base de datos relacional |
| Redis | 7.x | Cache, Pub/Sub, sesiones |
| Docker | 29.x | Contenerizacion |
| AWS EC2 | — | Servidor de produccion |
| Cloudflared Tunnel | — | Exposicion segura de servicios |
| Firebase Cloud Messaging | — | Notificaciones push |
| Cloudinary | — | Gestion de imagenes |
| Mercado Pago / Mobbex | — | Procesamiento de pagos |

---

## Documentacion

| Documento | Descripcion |
|---|---|
| [CHANGELOG.md](CHANGELOG.md) | Historial de versiones |
| [FEATURES.md](FEATURES.md) | Guia completa de funcionalidades |
| [ROADMAP.md](ROADMAP.md) | Proximos pasos y vision del proyecto |
| [SECURITY.md](SECURITY.md) | Politica de seguridad y reporte de vulnerabilidades |
| [BRAND.md](BRAND.md) | Identidad de marca y guia de uso |
| [TERMINOS_Y_CONDICIONES.md](TERMINOS_Y_CONDICIONES.md) | Terminos y condiciones de uso |
| [POLITICA_DE_PRIVACIDAD.md](POLITICA_DE_PRIVACIDAD.md) | Politica de privacidad y proteccion de datos |
| [COPYRIGHT.md](COPYRIGHT.md) | Certificacion de titularidad y derechos de autor |
| [PREGUNTAS.md](PREGUNTAS.md) | Preguntas frecuentes |
| [LICENSE](LICENSE) | Licencia |

---

## Enlaces

| Recurso | URL |
|---|---|
| **Repositorio privado (codigo fuente completo)** | [https://github.com/NickDev24/Stech-Viajes-Oficial](https://github.com/NickDev24/Stech-Viajes-Oficial) |
| **Repositorio publico (acreditacion)** | [https://github.com/NickDev24/Info_Publica_Stech_LIC](https://github.com/NickDev24/Info_Publica_Stech_LIC) |
| **Panel Administrativo** | [https://stech-adm.online](https://stech-adm.online) |
| **App Cliente** | [https://stech-app.site](https://stech-app.site) |
| **App Conductor** | [https://stech-driver.shop](https://stech-driver.shop) |

---

## Licencia

**STECH VIAJES** (c) 2026 **Facundo M. Cercuetti (NickDev24). Todos los derechos reservados.**

Este proyecto **no** es de codigo abierto. El acceso al codigo fuente esta restringido exclusivamente al titular y a personas expresamente autorizadas por el. Este repositorio publico existe unicamente como acreditacion de titularidad y antecedente de creacion.

**Queda prohibida cualquier forma de reproduccion, distribucion, modificacion o uso no autorizado del contenido de este repositorio y del proyecto al que hace referencia.**

---

*Documento actualizado el 13 de junio de 2026. Version 2.1.0.*
