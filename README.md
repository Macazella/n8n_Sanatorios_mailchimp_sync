# 📧 n8n Mailchimp Campaign Automation

Este proyecto contiene un flujo completo desarrollado en [n8n](https://n8n.io/) que automatiza la gestión de campañas de marketing por correo electrónico a través de la API de Mailchimp.

## 🚀 Funcionalidades principales

- Verificación y validación de contactos desde Google Sheets.
- Creación o selección automática de listas de distribución.
- Alta de contactos con filtros y condiciones de seguridad.
- Creación de campañas desde plantillas predefinidas.
- Programación o envío inmediato de campañas.
- Registro histórico de campañas enviadas.
- Envío de notificaciones a correo institucional.
- Prevención de duplicaciones o errores en los envíos.

## 📂 Estructura del proyecto

- `My workflow 2 (definitivo).json`: flujo exportado desde n8n.
- `/docs`: documentación funcional y técnica del flujo.
- `README.md`: descripción del proyecto y guía de uso.
- `LICENSE`: licencia del proyecto.

## ⚙️ Requisitos

- Servidor o instancia de n8n (local o en la nube).
- Cuenta de Mailchimp con clave API activa.
- Acceso a Google Sheets con permisos de lectura.
- Configuración de credenciales para los servicios conectados.

## 🔐 Seguridad implementada

- Verificación condicional del origen del contacto.
- Filtro anti-envíos vacíos o mal segmentados.
- Validaciones antes de registrar campañas.
- Detención inmediata ante errores críticos.

## 🔁 Futuras mejoras

- Flujo de reenvío automático tras 48 hs sin respuesta.
- Automatización de programación basada en engagement.
- Integración con bases segmentadas por especialidades.

## 📄 Licencia

Este proyecto está licenciado bajo la licencia **MIT**. Ver el archivo [LICENSE](LICENSE) para más detalles.

## 🤝 Contribuciones

Se aceptan issues y sugerencias para mejorar este flujo. Pull requests con nuevas ramas de automatización también son bienvenidas.

---

**Desarrollado por Magalí Cazella Méndez| Macazella - Proyecto personal para automatización de campañas.**

📄 Licencia
Apache 2.0 © Magalí Julieta Cazella Méndez
