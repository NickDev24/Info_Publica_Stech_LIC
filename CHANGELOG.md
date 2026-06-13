# CHANGELOG

## STECH VIAJES — Historial de versiones

**Repositorio público:** https://github.com/NickDev24/Info_Publica_Stech_LIC
**Repositorio privado (código fuente):** https://github.com/NickDev24/Stech-Viajes-Oficial

## [2.1.0] — 2026-06-13

### Añadido
- **Cupones de descuento para comercios afiliados:** Los comercios pueden crear, editar, pausar y eliminar cupones de descuento desde el panel de administracion. Cada cupon tiene codigo unico, tipo de descuento (porcentaje o monto fijo), fechas de validez, limite de usos, y condiciones personalizadas.
- **Sistema de canje con codigo QR:** Cada conductor recibe un codigo QR unico por cupon solicitado. El comercio puede escanear el QR con la camara o ingresar el codigo numerico para validar y canjear el cupon en el momento.
- **Notificaciones en tiempo real (SSE):** Los conductores reciben actualizaciones instantaneas cuando un comercio afiliado crea, modifica o elimina un cupon, sin necesidad de recargar la aplicacion.
- **Carrusel de comercios afiliados:** Los conductores ven un carrusel interactivo en la pantalla principal con los comercios afiliados activos, sus cupones disponibles, y acceso directo a Google Maps para navegacion.
- **Validacion de identidad con fotografia diaria:** Los conductores deben tomarse una selfie diaria para verificar su identidad antes de comenzar a operar.
- **Notificaciones push (FCM):** Los conductores reciben notificaciones en su dispositivo cuando hay nuevos cupones disponibles o actualizaciones importantes.

### Mejorado
- Interfaz del modal de cupones redisenada: centrado vertical, textos mas grandes, padding inferior para respetar la barra de navegacion fija.
- Optimizacion de imagenes de comercios con carga diferida y fallback a icono por defecto.
- Estabilidad del carrusel autoplay con pausa al interactuar.

### Corregido
- El carrusel de comercios ahora consulta la API correcta usando la base URL del servidor admin en lugar de rutas relativas.
- Validacion de cupones: se verifica correctamente el stock, las fechas de vigencia, los limites por conductor y el limite mensual del comercio.
- Prevencion de doble solicitud del mismo cupon por el mismo conductor.

## [2.0.0] — 2026-06-11

### Añadido
- **Panel Administrativo:** Gestion integral de usuarios (clientes y conductores), viajes, finanzas, comercios afiliados, promociones, validaciones, soporte tecnico y analitica en tiempo real.
- **App Cliente (PWA):** Solicitud de viajes con seleccion de destino, seguimiento en vivo del conductor, historial de viajes, sistema de calificaciones, wallet digital, y suscripcion semanal con descuento.
- **App Conductor (PWA):** Recepcion y gestion de solicitudes de viaje, mapas de navegacion paso a paso, comunicacion en tiempo real con pasajeros, registro de ganancias diarias, verificacion de identidad, y panel de disponibilidad.
- **Motor de geolocalizacion:** Sistema de geocodificacion optimizado para el norte argentino (NOA), con soporte para alias locales, coordenadas e intersecciones.
- **Infraestructura en tiempo real:** Comunicacion bidireccional mediante SSE y Redis Pub/Sub para actualizaciones instantaneas de viajes, ubicacion y mensajeria.
- **Pasarela de pagos:** Integracion con Mercado Pago y Mobbex para pagos con tarjeta, transferencias y recarga de wallet.
- **Sistema de viajes compartidos (car pooling):** Hasta 4 pasajeros por vehiculo, cada uno abona solo su distancia recorrida.
- **Chat en tiempo real:** Comunicacion directa entre conductor y pasajero, con soporte tecnico integrado.
- **Notificaciones push (FCM):** Alertas en dispositivo para eventos clave.

### Mejorado
- Interfaz de usuario redisenada con paleta de colores oscura y acentos en verde lima (#BFFF00).
- Validacion de documentos con selfie + DNI para conductores.
- Sidebar colapsable en escritorio para el panel admin.

## [1.0.0] — 2026-05-05

### Añadido
- Inicio del desarrollo del proyecto STECH VIAJES.
- Configuracion inicial del repositorio, infraestructura cloud y base de datos.

*Este documento se actualiza con cada version publicada.*
