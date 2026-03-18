# De p5js a GitHub Pages — sin terminal ni llaves API


**Nivel:** Sin experiencia previa con Git ni GitHub  
**Formato:** Demostración en vivo + práctica guiada  

---

## Objetivos de la sesión

Al terminar, las participantes podrán:

- Entender qué es GitHub y qué problema resuelve (versionar y publicar código)
- Crear una cuenta en GitHub desde cero
- Crear un repositorio y subir su proyecto de p5js usando solo el navegador
- Activar GitHub Pages para tener una URL pública de su proyecto
- Hacer cambios al código y ver esos cambios reflejados en la web

---

## Nota conceptual: ¿necesito una web personal antes?

GitHub Pages tiene dos modalidades:

| Tipo | URL | Cuándo se usa |
|---|---|---|
| Sitio de usuario | `tunombre.github.io` | Página personal o portafolio |
| Sitio de proyecto | `tunombre.github.io/nombre-del-repo` | Cualquier proyecto, como los oráculos |

**No necesitas crear un sitio de usuario primero.** Puedes publicar directamente desde cualquier repositorio de proyecto. La URL de tu oráculo quedará así:  
`tunombre.github.io/nombre-de-tu-oraculo`

---

## Materiales necesarios

- Computadora con navegador (Chrome, Firefox o Safari)
- Conexión a internet
- Tu proyecto funcionando en el editor de p5js: [editor.p5js.org](https://editor.p5js.org)
- Una dirección de correo electrónico para crear la cuenta de GitHub

---

## Estructura de la sesión

| Tiempo | Bloque |
|---|---|
| 0–10 min | Contexto: ¿qué es Git, GitHub y GitHub Pages? |
| 10–20 min | Crear cuenta en GitHub |
| 20–35 min | Crear repositorio y subir el proyecto |
| 35–50 min | Activar GitHub Pages |
| 50–60 min | Hacer un cambio y ver el resultado en vivo |

---

## Bloque 1 — Contexto (0–10 min)

### ¿Qué es Git?

Git es una herramienta para guardar versiones de tu código. Piénsalo como el historial de cambios de Google Docs, pero para archivos de código.

### ¿Qué es GitHub?

GitHub es un sitio web donde puedes guardar tus proyectos con Git en la nube. Es como Google Drive, pero hecho específicamente para código. Millones de proyectos de código abierto viven ahí.

### ¿Qué es GitHub Pages?

Es una funcionalidad gratuita de GitHub que convierte los archivos de tu repositorio en un sitio web con URL pública. Si tu repositorio tiene un `index.html`, GitHub Pages lo sirve como página web.

### ¿Qué es un repositorio?

Un repositorio (o "repo") es una carpeta en GitHub que contiene tu proyecto. Tiene historial de versiones, puede ser público o privado, y puede convertirse en sitio web con GitHub Pages.

---

## Bloque 2 — Crear cuenta en GitHub (10–20 min)

### Paso 1: Ir a github.com

Abre [github.com](https://github.com) en tu navegador.

### Paso 2: Crear cuenta

1. Haz clic en **Sign up** (esquina superior derecha)
2. Ingresa tu correo electrónico → clic en **Continue**
3. Crea una contraseña → clic en **Continue**
4. Elige un nombre de usuario (este será parte de tu URL, ej: `lunaoraculo`) → clic en **Continue**
5. Resuelve el captcha de verificación
6. Verifica tu correo: GitHub te mandará un código de 6 dígitos

> 💡 **Tip para elegir usuario:** elige algo que no te dé vergüenza compartir, porque aparecerá en la URL de tus proyectos. Puede ser tu nombre, un apodo, o algo relacionado con tu práctica artística.

### Paso 3: Configurar la cuenta

GitHub preguntará algunas cosas sobre tu uso. Para esta sesión puedes hacer clic en **Skip personalization** al final. Llegarás al dashboard principal.

---

## Bloque 3 — Crear repositorio y subir el proyecto (20–35 min)

### Preparación: descargar tu proyecto de p5js

Antes de crear el repositorio, necesitas los archivos de tu proyecto.

1. Ve a [editor.p5js.org](https://editor.p5js.org) y abre tu proyecto
2. En el menú superior, haz clic en **File → Download**
3. Esto descargará un archivo `.zip` con tus archivos
4. Descomprime el archivo. Dentro encontrarás al menos:
   - `index.html`
   - `sketch.js`
   - `style.css` (en algunos proyectos)

> ⚠️ **Importante:** GitHub Pages busca un archivo llamado exactamente `index.html` para mostrar tu sitio. El editor de p5js ya lo genera con ese nombre, así que no necesitas cambiarlo.

### Paso 4: Crear un nuevo repositorio

1. En tu dashboard de GitHub, haz clic en el botón verde **New** (o en el ícono `+` → **New repository**)
2. Llena el formulario:
   - **Repository name:** escribe el nombre de tu proyecto, sin espacios (usa guiones), por ejemplo: `oraculo-de-las-estrellas`
   - **Description:** opcional, una línea describiendo el proyecto
   - **Visibility:** selecciona **Public** (GitHub Pages gratuito requiere repositorios públicos)
   - Marca la casilla **Add a README file**
3. Haz clic en **Create repository**

### Paso 5: Subir los archivos de tu proyecto

Ahora estás dentro de tu repositorio. Ves un solo archivo: `README.md`.

1. Haz clic en el botón **Add file → Upload files**
2. Arrastra todos los archivos de tu proyecto descomprimido al área de carga (o haz clic en **choose your files** para seleccionarlos)
   - `index.html`
   - `sketch.js`
   - `style.css` (si existe)
   - Cualquier imagen, fuente u otro asset que use tu proyecto
3. En la sección **Commit changes** (al final de la página):
   - Puedes dejar el mensaje por defecto o escribir algo como `Subir proyecto inicial`
   - Deja seleccionada la opción **Commit directly to the main branch**
4. Haz clic en **Commit changes**

> 💡 Un "commit" es como tomar una foto del estado actual de tu proyecto. Cada vez que guardes cambios en GitHub, estarás creando un commit con un mensaje que describe qué cambiaste.

Ahora tu repositorio debería mostrar todos tus archivos. ¡El código ya está en la nube!

---

## Bloque 4 — Activar GitHub Pages (35–50 min)

### Paso 6: Ir a la configuración del repositorio

1. En tu repositorio, haz clic en la pestaña **Settings** (es la última pestaña, con ícono de engranaje)
2. En el menú de la izquierda, busca y haz clic en **Pages**

### Paso 7: Configurar la fuente de publicación

En la sección **Build and deployment**:

1. En **Source**, asegúrate de que diga **Deploy from a branch**
2. En **Branch**, haz clic en el menú desplegable que dice `None` y selecciona **main**
3. En el segundo menú (carpeta), deja seleccionado `/ (root)`
4. Haz clic en **Save**

### Paso 8: Esperar el despliegue

GitHub tardará entre 1 y 3 minutos en procesar y publicar tu sitio.

1. Recarga la página de Settings → Pages después de un par de minutos
2. Aparecerá un recuadro verde con el mensaje: **Your site is live at...**
3. La URL tendrá el formato: `https://tunombre.github.io/nombre-del-repo`

> ⏱️ Si después de 5 minutos no aparece, ve a la pestaña **Actions** de tu repositorio y revisa si hay algún proceso corriendo o algún error marcado en rojo.

### Paso 9: Visitar tu sitio

Haz clic en la URL que aparece en la sección Pages. ¡Tu oráculo ya tiene dirección en internet!

> 💡 Puedes compartir esa URL con cualquier persona. No necesitan cuenta de GitHub para verlo.

---

## Bloque 5 — Hacer un cambio y publicarlo (50–60 min)

Este bloque muestra el ciclo completo: editar → guardar → ver cambios en vivo.

### Paso 10: Editar un archivo directamente en GitHub

1. Regresa a la pestaña **Code** de tu repositorio (la primera pestaña)
2. Haz clic en el archivo `sketch.js`
3. Haz clic en el ícono del lápiz ✏️ (esquina superior derecha del archivo) para editarlo
4. Haz un cambio visible: por ejemplo, cambia un color, un texto, un número
5. Haz clic en **Commit changes...**
6. Escribe un mensaje descriptivo, por ejemplo: `Cambiar color de fondo`
7. Haz clic en **Commit changes**

### Paso 11: Ver el cambio en tu sitio

1. Espera 1–3 minutos
2. Recarga tu URL pública en el navegador
3. El cambio debería reflejarse

> 💡 Si no ves el cambio de inmediato, prueba recargando con `Ctrl+Shift+R` (o `Cmd+Shift+R` en Mac) para evitar el caché del navegador.

---

## Resumen del flujo

```
Editor p5js → Descargar .zip → Descomprimir
     ↓
Crear repositorio en GitHub → Subir archivos → Hacer commit
     ↓
Settings → Pages → Branch: main → Save
     ↓
URL pública: tunombre.github.io/nombre-del-repo 🎉
```

---

## Vocabulario clave

| Término | Significado |
|---|---|
| **Repositorio (repo)** | Carpeta de proyecto en GitHub con historial de versiones |
| **Commit** | Una versión guardada del proyecto, con mensaje descriptivo |
| **Branch (rama)** | Versión paralela del código; la principal se llama `main` |
| **Deploy** | Publicar o lanzar el proyecto a internet |
| **GitHub Pages** | Servicio de GitHub para publicar sitios web estáticos gratis |
| **index.html** | Archivo de entrada que los navegadores buscan por defecto |

---

## Preguntas frecuentes

**¿Puedo tener varios proyectos publicados?**  
Sí. Cada repositorio tiene su propia URL de Pages. Puedes publicar tantos como quieras.

**¿Puedo hacer el repositorio privado?**  
GitHub Pages gratuito requiere repositorios públicos. Si necesitas privacidad, puedes borrar el archivo `sketch.js` y dejar solo el `index.html`, aunque eso es poco común en proyectos artísticos.

**¿Qué pasa si edito el código en p5js y quiero actualizar el sitio?**  
Descarga el proyecto de nuevo desde p5js, y sube los archivos actualizados a GitHub. En el paso de carga, GitHub detectará que los archivos ya existen y los reemplazará.

**¿Puedo editar el código directamente en GitHub?**  
Sí, como vimos en el Bloque 5. Para cambios pequeños es suficiente. Para cambios grandes, es más cómodo editar en p5js y volver a subir.

**¿Cuánto cuesta?**  
GitHub y GitHub Pages son completamente gratuitos para repositorios públicos.

---

## Recursos para seguir explorando

- [editor.p5js.org](https://editor.p5js.org) — Editor oficial de p5js
- [pages.github.com](https://pages.github.com) — Documentación oficial de GitHub Pages
- [docs.github.com/es](https://docs.github.com/es) — Documentación de GitHub en español
- [p5js.org/es/reference](https://p5js.org/es/reference/) — Referencia de p5js en español

---

*Sesión preparada para el taller de publicación web con p5js y GitHub Pages.*
