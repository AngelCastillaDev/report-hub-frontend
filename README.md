# 🎨 Frontend - Report System

Este repositorio contiene el **frontend web** del sistema de reportes.  
La aplicación se conecta a los servicios backend desplegados en Render, utiliza **Firebase** para autenticación y se integra con **Supabase** para datos y almacenamiento de archivos.

---

## ✨ Funcionalidades principales

- 🔐 **Autenticación con Firebase**: inicio de sesión, registro y recuperación de contraseña.  
- 👥 **Gestión de usuarios**: acceso según roles y permisos definidos en Firebase.  
- 📊 **Visualización de reportes**: lista de reportes generados (PDF / PPTX) con opción de descarga.  
- 📤 **Subida de archivos**: manejo de imágenes y plantillas que se almacenan en Supabase Storage.  
- 🕒 **Reportes automáticos**: vista de reportes trimestrales generados por los jobs del backend.  
- 📱 **Responsive**: interfaz adaptable para escritorio y dispositivos móviles.  

---

## 🛠️ Tecnologías clave

- **Framework**: Angular / React / Vue (dependiendo del stack elegido).  
- **UI**: TailwindCSS / Material / Bootstrap (según preferencia).  
- **Auth**: Firebase Authentication (tokens validados en backend).  
- **Data**: Supabase SDK para consumir Postgres y Storage.  
- **API**: conexión con los microservicios del backend (según rama).  

---

## 🔗 Integraciones

- **Firebase**:  
  - Login, registro, logout, recuperación de contraseña.  
  - Manejo de claims para roles y permisos.  

- **Supabase**:  
  - Lectura de reportes disponibles.  
  - Subida y visualización de archivos en Storage.  
  - Consumo de tablas (ej. actividad de usuarios).  

- **Backend en Render**:  
  - Comunicación con los servicios de `security-firebase`, `activity-tracking`, `reports` y `quarterly-reports`.  

---

## ⚙️ Variables de entorno (resumen)

El frontend requiere un archivo `.env` (o configuración equivalente según framework).  
Incluye valores como:

- 🔐 **Firebase**: apiKey, authDomain, projectId, etc.  
- 🗄 **Supabase**: URL del proyecto y public anon key.  
- 🌐 **APIs del backend**: URLs de los servicios en Render.  

---

## 🚀 Ejecución local

```bash
# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm start

# Compilar para producción
npm run build
