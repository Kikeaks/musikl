<div align="center">
  <!-- Logo de la aplicación: coloca tu archivo en public/logo.png o src/assets/logo.png -->
  <img src="./src/assets/musikl.png" alt="musikl logo" width="256" />

  <p>Tu música, tu mundo, tu ritmo.</p>

  <!-- Badges de tecnologías -->
  <p>
    <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React" />
    <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
    <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="TailwindCSS" />
    <img src="https://img.shields.io/badge/Supabase-3DDC84?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
    <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/Deezer-FF5F00?style=for-the-badge" alt="Deezer" />
    <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  </p>
</div>

---

## 🎧 Descripción

musi**k**l es una aplicación web moderna para descubrir música, explorar artistas, crear listas de reproducción personalizadas y conectar con otros usuarios a través de funciones sociales básicas.

Combina una interfaz intuitiva con funcionalidades rápidas, fluidas y construidas totalmente con **React + Supabase**.
La aplicación usa la API pública de **Deezer** para obtener música, álbumes y artistas, y un **reproductor integrado** permite escuchar canciones directamente desde la app.

---

## 🚀 Características principales

### 🔊 Reproductor integrado

- Reproduce canciones dentro de la aplicación
- Controles de: play / pausa / siguiente / volumen
- Compatibilidad con la API de Deezer

### 📝 Gestión de listas de reproducción
- Creación
- Edición (nombre y portada)
- Borrado
- Añadir y quitar canciones
- Añadir portada personalizada
- Guardar las listas de reproducción en tu perfil

### 👥 Funciones sociales

- Dar "me gusta" a listas de reproducción
- Comentar en listas de reproducción
- Seguir a otros usuarios

*(Sistema social ligero, pensado para futuras ampliaciones)*

### 🔐 Autenticación y base de datos

El *backend* funciona completamente con **Supabase**, ofreciendo:

- Registro e inicio de sesión
- Recuperación de contraseña
- Almacenamiento de perfiles
- Avatares subidos por los usuarios
- Tablas para:
  - usuarios
  - listas de reproducción
  - canciones añadidas
  - me gustas *(likes)*
  - comentarios
  - seguimientos

### 🔎 Explorar

Búsqueda y navegación por:
- artistas
- álbumes
- canciones
- usuarios

---

## 🛠️ Tecnologías utilizadas

| Área          | Tecnología                        |
| ------------- | --------------------------------- |
| Frontend      | React, JavaScript, JSX, CSS       |
| Backend       | Supabase (Auth, REST, Storage)    |
| Base de datos | PostgreSQL                        |
| Música        | API de Deezer                     |
| Despliegue    | Vercel                            |
| Estilos extra | TailwindCSS                       |

---

## 📁 Estructura del proyecto

```src/
 ├── assets/
 ├── componentes/
 │    ├── albumes/
 │    ├── artistas/
 │    ├── canciones/
 │    ├── estructura/
 │    ├── interfaz/
 │    ├── modales/
 │    ├── perfiles/
 │    ├── playlists/
 ├── config/
 ├── contextos/
 ├── hooks/
 ├── paginas/
 │    ├── auth/
 │    ├── perfiles/
 │    ├── playlists/
 ├── App.jsx
 ├── main.jsx
 ├── index.css
```
Perfectamente organizada en módulos reutilizables para mantener el código ordenado y escalable.

---

## 💻 Instalación

Antes de nada, el sistema deberá tener instalada una versión **igual o superior** a *NodeJS 18*.

```bash
git clone https://github.com/Kikeaks/musikl.git
cd musikl-master
npm install
npm start        # o npm run dev si usas Vite
```

> **IMPORTANTE:** para conectar con tu proyecto de Supabase, tendrás que crear el fichero **.env.local** en la raíz del repositorio. El contenido del fichero deberá de ser el siguiente:
> ```bash
> VITE_SUPABASE_URL= # la URL de tu proyecto
> VITE_SUPABASE_ANON_KEY= # clave de tu proyecto
>```
---

## ☁️ Despliegue

La aplicación está desplegada en Vercel, con actualizaciones automáticas cada vez que se hace un push al repositorio.

🔗 [Enlace a la aplicación](https://musikl.vercel.app)

---

## 🤝 Contribuciones

Toda contribución es bienvenida: mejoras, correcciones o nuevas funcionalidades.

---

## 📝 Licencia

Este proyecto está bajo la licencia MIT

---