# 🚀 Checklist de Despliegue en GitHub Pages

## Baby Shower — Alice Madelyn de la Cruz Romo

---

### 1. Preparación del Repositorio

- [ ] Crear cuenta en [github.com](https://github.com) (si no tienes)
- [ ] Crear un **nuevo repositorio** con nombre: `baby-shower-alice`
- [ ] Inicializar con README (opcional)
- [ ] Clonar el repositorio en tu computadora:
  ```bash
  git clone https://github.com/TU_USUARIO/baby-shower-alice.git
  ```

### 2. Subir los archivos

- [ ] Copiar **todos** los archivos de la carpeta `invitacion-alice` al repositorio clonado:
  - `index.html`
  - `gracias.html`
  - `mensaje-whatsapp.txt`
  - `hero-sm.jpg`, `hero-md.jpg`, `hero-lg.jpg`
  - `ilustracion1-sm.jpg`, `ilustracion1-md.jpg`, `ilustracion1-lg.jpg`
  - `ilustracion2-sm.jpg`, `ilustracion2-md.jpg`, `ilustracion2-lg.jpg`
  - `padres1-sm.jpg`, `padres1-md.jpg`, `padres1-lg.jpg`
  - `padres2-sm.jpg`, `padres2-md.jpg`, `padres2-lg.jpg`
  - `video_latidos-mobile.mp4`
  - `video_latidos-desktop.mp4`
  - `deploy.sh`

- [ ] Verificar estructura final:
  ```
  baby-shower-alice/
  ├── index.html
  ├── gracias.html
  ├── hero-sm.jpg
  ├── hero-md.jpg
  ├── hero-lg.jpg
  ├── ilustracion1-sm.jpg
  ├── ilustracion1-md.jpg
  ├── ilustracion1-lg.jpg
  ├── ilustracion2-sm.jpg
  ├── ilustracion2-md.jpg
  ├── ilustracion2-lg.jpg
  ├── padres1-sm.jpg
  ├── padres1-md.jpg
  ├── padres1-lg.jpg
  ├── padres2-sm.jpg
  ├── padres2-md.jpg
  ├── padres2-lg.jpg
  ├── video_latidos-mobile.mp4
  └── video_latidos-desktop.mp4
  ```

### 3. Hacer commit y push

- [ ] Desde la carpeta del repositorio:
  ```bash
  git add .
  git commit -m "🍼 Baby Shower Alice Madelyn - Invitación digital"
  git push origin main
  ```
  > Si la rama se llama `master`, cambiar `main` por `master`.

### 4. Activar GitHub Pages

- [ ] Ir al repositorio en GitHub → pestaña **Settings**
- [ ] En el menú lateral, click en **Pages**
- [ ] En **Source**, seleccionar:
  - Branch: `main` (o `master`)
  - Folder: `/ (root)`
- [ ] Click en **Save**
- [ ] Esperar 1-3 minutos hasta que aparezca el mensaje:
  > ✅ **Your site is published at** `https://TU_USUARIO.github.io/baby-shower-alice/`

### 5. Verificación Post-Despliegue 🔍

- [ ] Abrir el enlace en **Chrome móvil** y verificar:
  - [ ] La página carga completa
  - [ ] Las **imágenes se ven** correctamente
  - [ ] El **video se reproduce** al hacer click
  - [ ] El **countdown** funciona
  - [ ] El botón de **WhatsApp** abre la app con el mensaje
  - [ ] La sección **Dedicatoria** funciona
  - [ ] Los corazones flotantes se ven
  - [ ] El scroll reveal anima las secciones
- [ ] Abrir en **escritorio** y verificar lo mismo
- [ ] Probar el enlace de **Google Maps**
- [ ] Probar el enlace de la **tarjeta de agradecimiento** (`/gracias.html`)

### 6. Compartir 📲

- [ ] Copiar el enlace de GitHub Pages
- [ ] Pegar el enlace en el **mensaje de WhatsApp** (archivo `mensaje-whatsapp.txt`)
- [ ] Enviar el mensaje a los invitados
- [ ] Verificar que el enlace se previsualiza bien en WhatsApp

---

## ⚡ Método Alternativo: deploy.sh

Si prefieres automatizar, el archivo `deploy.sh` hace todo por ti:

```bash
chmod +x deploy.sh
./deploy.sh
```

> Asegúrate de tener `git` instalado y haber iniciado sesión.

---

## 🔧 Solución de Problemas

| Problema | Solución |
|----------|----------|
| No se ven las imágenes | Verificar que los archivos JPG están en la raíz del repo, no en subcarpetas |
| El video no carga | Verificar que los MP4 se subieron correctamente (peso < 1MB) |
| GitHub Pages muestra 404 | Esperar 3 min, verificar que la rama es `main` y folder es `/root` |
| WhatsApp no abre | Probar desde el celular; desde PC puede no detectar la app |
| Imágenes pesadas | Ya están optimizadas (sm < 50KB), si se ven lentas, usar solo `-sm` |

---

**¡Listo! Tu invitación estará en línea para todo el mundo 💕**