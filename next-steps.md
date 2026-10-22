# Pasos a Seguir: Configuración Local del Proyecto LaTeX con GitHub

Este documento describe los pasos para traer tu proyecto de Overleaf (**QUALITY MANAGEMENT - PROJECT PART 3**) a este entorno local y conectarlo con GitHub.

---

## Estado Actual
- [x] **Git instalado en el sistema:** Versión `2.56.0` configurada en la variable de entorno `PATH`.
- [ ] **Archivos de Overleaf descargados.**
- [ ] **Repositorio de GitHub creado y vinculado.**

---

## Paso 1: Descargar el proyecto desde Overleaf

1. Ve a la pestaña de tu navegador donde tienes abierto **Overleaf**.
2. En la barra superior izquierda, haz clic en el botón **Menu** (icono con la letra O / menú lateral).
3. En la sección **Download**, haz clic en el botón **Source**:
   - Esto descargará un archivo comprimido `.zip` con todos los archivos fuente de tu proyecto (`main.tex`, figuras, tablas, etc.).
4. Guarda o mueve ese archivo descargado a esta carpeta:
   `C:\Users\joan_\Desktop\Test1`
   *(Si se queda en tu carpeta de Descargas, no hay problema, indícalo en el chat y lo moveré por ti).*

---

## Paso 2: Crear el repositorio en GitHub

1. Ingresa a tu cuenta de GitHub y dirígete a:
   [https://github.com/new](https://github.com/new)
2. Asigna un nombre al repositorio, por ejemplo:
   `quality-management-project`
3. **Importante:** Déjalo **completamente vacío**:
   - NO marques la casilla *"Add a README file"*.
   - NO añadas *.gitignore* ni licencia por ahora (lo configuraremos aquí).
4. Haz clic en **Create repository**.
5. Copia la URL del repositorio (terminada en `.git`), por ejemplo:
   `https://github.com/tu-usuario/quality-management-project.git`

---

## Paso 3: Sincronización y Checkout Local

Una vez completados los pasos anteriores:
1. Regresa al chat y envía la **URL de tu repositorio de GitHub**.
2. El asistente ejecutará automáticamente:
   - La descompresión de todos tus archivos en esta carpeta.
   - La inicialización del repositorio local (`git init -b main`).
   - El commit inicial con todo tu código LaTeX y recursos.
   - La vinculación remota (`git remote add origin <tu-url>`) y el `git push`.

A partir de ese momento, podremos modificar [`main.tex`](file:///c:/Users/joan_/Desktop/Test1/main.tex) y cualquier otro archivo directamente aquí.
