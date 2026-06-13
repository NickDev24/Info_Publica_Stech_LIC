# SECURITY POLICY

## STECH VIAJES — Politica de Seguridad

---

## Reporte de vulnerabilidades

STECH VIAJES toma la seguridad de su plataforma seriamente. Si descubres una vulnerabilidad de seguridad, agradecemos que nos la reportes de manera responsable.

### Como reportar

**NO** reportes vulnerabilidades de seguridad en el rastreador de issues publico de GitHub ni en foros publicos. En su lugar, envianos los detalles a traves del repositorio privado oficial:

- **Repositorio oficial:** https://github.com/NickDev24/Stech-Viajes-Oficial
- **Alias:** NickDev24

### Que incluir en tu reporte

- Descripcion clara del tipo de vulnerabilidad.
- Pasos para reproducir el problema (incluyendo capturas de pantalla si es posible).
- Version afectada de la plataforma.
- Posible impacto de la vulnerabilidad.
- Sugerencia de mitigacion (si la tienes).

### Proceso

1. Recibiremos tu reporte y lo evaluaremos en un plazo de 48 horas.
2. Trabajaremos en una solucion y te mantendremos informado del progreso.
3. Una vez solucionado, coordinaremos la divulgacion responsable.

### Recompensas

Actualmente no contamos con un programa formal de bug bounty, pero reconocemos publicamente a quienes reporten vulnerabilidades de manera responsable (previa autorizacion).

---

## Buenas practicas de seguridad para usuarios

### Para conductores

- No compartas tus credenciales de acceso con nadie.
- Realiza la verificacion diaria con fotografia cada vez que inicies sesion.
- Manten tu dispositivo actualizado con las ultimas actualizaciones de seguridad.
- Cierra sesion si alguien mas va a usar tu dispositivo.
- Reporta inmediatamente cualquier actividad sospechosa en tu cuenta.

### Para clientes

- Usa contrasenas fuertes y unicas para tu cuenta.
- No compartas tu codigo de verificacion con nadie.
- Verifica la identidad del conductor antes de subir al vehiculo (nombre, foto, patente).
- Reporta cualquier incidente de seguridad a traves de los canales de soporte.

---

## Cifrado y proteccion de datos

- **En transito:** Todos los datos se transmiten cifrados mediante TLS/SSL.
- **En reposo:** Datos sensibles cifrados en la base de datos.
- **Autenticacion:** JWT tokens con expiracion y Firebase Authentication.
- **Contrasenas:** Almacenadas con hash seguro (bcrypt).

---

*Documento actualizado el 13 de junio de 2026.*
