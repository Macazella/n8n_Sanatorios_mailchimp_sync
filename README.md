📌 Sanatorios – Google Sheets ➜ Mailchimp (n8n)
Este flujo automatiza la carga de contactos del Sanatorio San José desde una planilla de Google Sheets hacia Mailchimp mediante n8n autoalojado.

🚀 Tecnologías utilizadas
n8n (instancia autoalojada con Docker)

Google Sheets API

Mailchimp API

🧱 Estructura del repositorio
Archivo/Carpeta	Descripción
workflow_san_jose_mailchimp.json	Export del flujo de n8n listo para importar
docs/	Contiene visualizaciones del flujo
.env.example	Variables de entorno necesarias para ejecutar el flujo
README.md	Documentación del proyecto

⚙️ Requisitos
Antes de ejecutar el flujo, se necesita:

✅ Clave API de Mailchimp

✅ Acceso a una hoja de Google Sheets con estructura compatible

✅ Proyecto creado en Google Cloud con Google Sheets API habilitada

✅ Entorno de n8n funcionando en local o en servidor (Docker o instalación manual)

🧪 Instalación local (modo autoalojado)
Instalar Docker Desktop:
👉 https://www.docker.com/products/docker-desktop

Ejecutar n8n en modo local (Docker):

bash
Copiar
Editar
docker run -it --rm \
  -p 5678:5678 \
  -e N8N_BASIC_AUTH_ACTIVE=true \
  -e N8N_BASIC_AUTH_USER=admin \
  -e N8N_BASIC_AUTH_PASSWORD=tu_clave_segura \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
Acceder a n8n desde el navegador:
👉 http://localhost:5678

📥 Importar el flujo
Abrí tu instancia de n8n (localhost o servidor).

Hacé clic en "Import" (ícono de subir).

Seleccioná el archivo workflow_san_jose_mailchimp.json.

Reemplazá los campos con las credenciales de tu entorno.

🔐 Variables de entorno necesarias
Creá un archivo .env (basado en .env.example) con estas claves:

env
Copiar
Editar
MAILCHIMP_API_KEY=tu_api_key
MAILCHIMP_LIST_ID=tu_lista_id
GOOGLE_SHEETS_URL=https://docs.google.com/spreadsheets/d/...
N8N_BASIC_AUTH_USER=admin
N8N_BASIC_AUTH_PASSWORD=clave_segura
📌 Consideraciones
📅 El flujo puede ser programado (ej. cada 24hs) o ejecutado manualmente.

✅ Maneja errores con nodos condicionales y alertas por correo.

🛠️ Adaptable a otros sanatorios cambiando únicamente el Google Sheet y el List ID.

📄 Licencia
Apache 2.0 © Magalí Julieta Cazella Méndez
