# STECH VIAJES

**Plataforma Mediadora de transporte Argentino.**

---

## Certificación de titularidad y derechos de autor

Yo, **Facundo Maximiliano Cercuetti** (NickDev24), declaro bajo juramento ser el autor original, único y legítimo propietario de la totalidad del código fuente, diseño, arquitectura, algoritmos, base de datos, interfaz de usuario, marca, nombre comercial, identidad visual y cualquier otro activo intelectual comprendido en el proyecto **STECH VIAJES** (en adelante, "el Sistema").

---

## Datos del proyecto

| Atributo | Valor |
|---|---|
| **Nombre del proyecto** | STECH VIAJES |
| **Versión** | 2.0.0 |
| **Fecha de inicio del desarrollo** | 05 de mayo de 2026 |
| **Fecha del primer deploy en producción** | 10 de junio de 2026 — 05:49 ART (GMT-3) |
| **Infraestructura de producción** | AWS EC2 (Ubuntu) + Docker + Cloudflared Tunnel |
| **Autor / Titular** | Nicolás Ezequiel Guzmán |
| **Alias** | NickDev24 |
| **Repositorio privado oficial** | [https://github.com/NickDev24/Stech-Viajes-Oficial](https://github.com/NickDev24/Stech-Viajes-Oficial) |

---

## Declaración de propiedad intelectual

El Sistema **STECH VIAJES** constituye una obra original protegida por las leyes de propiedad intelectual de la **República Argentina** (Ley 11.723) y los tratados internacionales aplicables (Convenio de Berna, ADPIC, Tratado de la OMPI sobre Derecho de Autor).

Queda **total y absolutamente prohibido**:

- La reproducción, copia, distribución, modificación, adaptación, traducción, ingeniería inversa, descompilación o extracción de cualquier componente del Sistema, sea total o parcial, por cualquier medio o procedimiento, sin la autorización expresa y por escrito del titular.
- El uso, comercialización, licenciamiento, cesión o transferencia del Sistema o de cualquiera de sus partes a terceros sin el consentimiento explícito del titular.
- La creación de obras derivadas basadas en el Sistema.
- La eliminación, alteración u ocultación de cualquier marca, nombre, logotipo, aviso de derechos de autor o identificación de titularidad incorporada en el Sistema.

El código fuente completo, la documentación técnica, los esquemas de base de datos, la lógica de negocio, los algoritmos de funcionamiento, las interfaces gráficas y cualquier otro componente del Sistema se encuentran bajo **reserva absoluta de confidencialidad** y no se divulgan en este repositorio público.

---

## Arquitectura del sistema (vista general)

> **Nota:** Esta descripción contiene únicamente información de alto nivel. Los detalles de implementación, algoritmos propietarios, lógica de negocio y estructura interna forman parte del secreto comercial y no se revelan.

| Componente | Descripción |
|---|---|
| **Panel Administrativo** | Gestión integral de usuarios, viajes, finanzas, promociones, validaciones, soporte técnico, analítica y configuración del sistema. Incluye panel de control en tiempo real con mapas de seguimiento de unidades. |
| **App Cliente (PWA)** | Plataforma para que los usuarios soliciten, gestionen y paguen viajes. Incluye selección de destino, seguimiento en vivo del conductor, historial de viajes, sistema de calificaciones, wallet digital y programas de suscripción semanal. |
| **App Conductor (PWA)** | Plataforma para que los conductores reciban y gestionen solicitudes de viaje. Incluye mapas de navegación paso a paso, comunicación en tiempo real con pasajeros, registro de earnings diarios, verificación de identidad y panel de disponibilidad. |
| **Motor de geolocalización** | Sistema de geocodificación y búsqueda de direcciones optimizado para el norte argentino (NOA), con soporte para alias locales, coordenadas, intersecciones y puntos de interés regionales. |
| **Infraestructura en tiempo real** | Sistema de comunicación bidireccional mediante Server-Sent Events (SSE) y Redis Pub/Sub para actualizaciones instantáneas de estado de viajes, ubicación de conductores y mensajería. |
| **Pasarela de pagos** | Integración con múltiples procesadores de pago (Mercado Pago, Mobbex) para procesar pagos con tarjeta, transferencias y recargas de wallet. |
| **Infraestructura cloud** | Desplegado en AWS EC2 con Docker, respaldado por Supabase (PostgreSQL), Redis, Cloudflared Tunnel, y notificaciones push vía Firebase Cloud Messaging. |

---

## Tecnologías utilizadas

| Tecnología | Versión | Propósito |
|---|---|---|
| Next.js | 16.2.4 | Framework principal (3 aplicaciones) |
| TypeScript | ~5.8 | Lenguaje de programación |
| Prisma ORM | ~6.6 | Capa de base de datos |
| PostgreSQL (Supabase) | — | Base de datos relacional |
| Redis | 7.x | Caché, Pub/Sub, sesiones |
| Docker | 29.x | Contenerización |
| AWS EC2 | — | Servidor de producción |
| Cloudflared Tunnel | — | Exposición segura de servicios |
| Firebase Cloud Messaging | — | Notificaciones push |
| Mercado Pago / Mobbex | — | Procesamiento de pagos |

---

## Enlaces

| Recurso | URL |
|---|---|
| **Repositorio privado (código fuente completo)** | [https://github.com/NickDev24/Stech-Viajes-Oficial](https://github.com/NickDev24/Stech-Viajes-Oficial) |
| **Panel Administrativo** | [https://stech-adm.online](https://stech-adm.online) |
| **App Cliente** | [https://stech-app.site](https://stech-app.site) |
| **App Conductor** | [https://stech-driver.shop](https://stech-driver.shop) |

---

## Licencia

**STECH VIAJES** © 2026 **Facundo M. Cercuetti (NickDev24). Todos los derechos reservados.**

Este proyecto **no** es de código abierto. El acceso al código fuente está restringido exclusivamente al titular y a personas expresamente autorizadas por él. Este repositorio público existe únicamente como acreditación de titularidad y antecedente de creación.

**Queda prohibida cualquier forma de reproducción, distribución, modificación o uso no autorizado del contenido de este repositorio y del proyecto al que hace referencia.**

---

*Documento generado el 10 de junio de 2026.*
