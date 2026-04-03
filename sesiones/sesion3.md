# Sesión 3 — Deploy: sube tu oráculo al mundo 

Revisión de proyectos.

## Objetivos

Revisar
- Revisaremos los oráculos en desarrollo. 
- Compartiremos avances, dudas y feedback entre el grupo.

Publicar
- A qué nos referimos cuando hablamos de publicar un proyecto en la web.
- Identificar qué plataforma se adapta mejor a cada tipo de oráculo
- Lograr que cada participante tenga al menos una URL pública funcionando
- Dejar documentado el proceso en el repo para futuras referencias

## Agenda

| Tiempo | Bloque |
|--------|--------|
| 0:00 – 0:30 | Revisión de proyectos — ronda rápida |
| 0:30 – 0:50 | Trabajo por pares / equipos |
| 0:50 – 1:40 | Charla: Publiquemos nuestro proyectos |
| 1:40 – 2:15 | Manos a la obra — práctica acompañada |
| 2:15 – 2:30 | Cierre, URLs y tarea |

---

## Ejercicio de mapeo de proyectos 
¿Qué necesita tu oráculo para vivir en la web?

> **Completa la frase:** Mi oráculo responde a __________ y para eso necesita __________.

Compartir en el chat o en voz alta lo siguiente: 
- tipo de proyecto 
- lenguajes usados  
- expectativas de interacción con el usuario


Esto nos ayudará a entender mejor las necesidades técnicas de cada proyecto y a elegir la plataforma de deploy más adecuada.

Si somos pocos asistentes, en 1 min por participante compartir:
- Nombre del oráculo
- Qué pregunta responde
- Cómo funciona (cartas, frases, algoritmo, etc.)

---
## Trabajo por pares 

Anotar en el chat:
- Quiénes ya tienen prototipo
- Quiénes solo tienen concepto

- ¿Cómo funciona tu oráculo?
- Tengo algún bloqueo, si sí,  ¿en dónde o en qué parte del proceso?  
- ¿Qué parte del oráculo es más interesante?
- ¿Qué podría hacerlo más claro o potente?
- ¿Qué interacción podría mejorar?

Qué tipo de oráculos aparecieron. 
- Oráculos tipo carta (visualización, texto, audio)
- Oráculos tipo experiencia (narrativa, multimedia, interactiva)
- Oráculos tipo algoritmo (respuestas generadas a partir de inputs)
- Oráculos tipo comunidad (respuestas basadas en contribuciones de usuarios)

¿Consideras que tu proyecto es poético, aleatoorio, generativo, visual, interactivo, electrónico, narrativo?

## Charla: Publiquemos nuestro proyectos 

Conceptos clave a cubrir antes de las demos:

**¿Qué es publicar en la web?** 
- Servidor
- Dominio 
- URL pública


**Archivos estáticos / apps con backend**
  - Estático: HTML, CSS, JS puro → casi cualquier host lo soporta.
  - Backend: Python, bases de datos, lógica en servidor → necesita entorno de ejecución.
- **Por qué importa la diferencia:** no todas las plataformas soportan todo tipo de proyecto

---

## Las rutas — plataformas de deploy

### GitHub Pages
**Para:** sitios estáticos, JS puro, proyectos narrativos en HTML  
**Gratis:** sí  
**Dominio:** `usuario.github.io/repo`


**Pasos básicos:**
1. Crear cuenta en
https://github.com

2. Crear repositorio
nombre: `oraculo` (o el que quieras)

3. Subir archivos
  - `index.html`
  - `sketch.js` (si optaste por la opción de p5)

4. Ir a **Settings → Pages**

6. Activar **Deploy from branch**

7. URL final: `https://usuario.github.io/oraculo`


**Consideraciones:**
- Solo archivos estáticos (no corre Python ni bases de datos)
- Ideal para oráculos tipo carta/visualización en JS
- Se puede conectar un dominio propio
   
**Recursos:**
- [Documentación oficial de GitHub Pages](https://docs.github.com/en/pages)


---
### Vercel — Guía rápida de deploy

**Para:** proyectos JS, React, Next.js, Vue, Svelte    
**Gratis:** plan hoobby
**Dominio:** `proyecto.vercel.app`

**Pasos básicos:**

1. Ir a https://vercel.com
2. Conectar tu cuenta de GitHub
3. Importar tu repositorio `oraculo`
4. Deploy automático (Vercel detecta el framework)
5. URL final: `https://usuario.vercel.app/oraculo`

**Ventajas:**
- Deploy automático desde GitHub con cada push
- Excelente para oráculos con componentes interactivos modernos
- Soporta funciones serverless (pequeña lógica de backend sin servidor propio)
- Sin configuración: detecta el framework y hace el build solo

**Recursos:**
- [vercel.com](https://vercel.com)

---

### WordPress
**Para:** proyectos narrativos, arte digital, oráculos tipo revista o experiencia editorial  
**Gratis:** plan básico disponible · **Dominio:** `proyecto.wordpress.com`

**WordPress.com vs WordPress.org:**
| | WordPress.com | WordPress.org |
|--|--|--|
| Hosting | incluido | debes contratarlo |
| Control | limitado | total |
| Plugins | restringidos en plan gratis | todos disponibles |
| Código propio (JS/CSS) | no en plan gratis | sí |

**Cuándo usarlo:**
- El oráculo es principalmente visual/narrativo
- No necesitas lógica de servidor propia
- Quieres un CMS para actualizar contenido fácilmente

**Plugins útiles para oráculos:**
- Formularios: WPForms, Contact Form 7
- Galerías y multimedia: Envira Gallery, Smash Balloon
- Audio/video: AudioIgniter, YouTube Embed

---

### 🟠 Netlify
**Para:** sitios estáticos, JAMstack, proyectos con formularios o funciones ligeras  
**Gratis:** plan starter incluido · **Dominio:** `proyecto.netlify.app`

- Similar a Vercel pero con buen soporte para sitios estáticos puros
- Drag & drop deploy: puedes arrastrar una carpeta directamente
- Netlify Forms: recolecta respuestas sin backend (útil para oráculos interactivos)
- Fácil de usar para quienes vienen de WordPress y quieren más control

**Recursos:**
- [netlify.com](https://netlify.com)

---

### 🟣 Render
**Para:** apps con backend — Python (Flask, FastAPI), Node.js, bases de datos  
**Gratis:** plan free disponible (con limitaciones de inactividad) · **Dominio:** `proyecto.onrender.com`

- La opción cuando el oráculo tiene lógica en Python o necesita servidor
- Soporta servicios web, cron jobs y bases de datos PostgreSQL
- Más configuración que Vercel/Netlify pero mucho más flexible

**Recursos:**
- [render.com](https://render.com)

---

### 📓 Observable / Notion + super.so *(opciones alternativas)*

**Observable** → para oráculos basados en datos y visualizaciones (D3, Plot)  
- Notebooks interactivos publicables con una URL  
- [observablehq.com](https://observablehq.com)

**Notion + super.so** → para oráculos narrativos sin código  
- Convierte páginas de Notion en sitios web con dominio propio  
- Muy accesible para participantes sin experiencia técnica

---

## Tabla resumen — ¿qué plataforma usar?

| Mi oráculo es... | Plataforma recomendada |
|---|---|
| HTML/CSS/JS estático | GitHub Pages · Netlify |
| React / Vue / Svelte | Vercel · Netlify |
| Python / Flask / FastAPI | Render |
| Narrativo / visual / sin código | WordPress · Notion + super.so |
| Visualización de datos | Observable · GitHub Pages |
| Quiero deploy automático con git | Vercel · Netlify · GitHub Pages |

---

## Tarea para la próxima sesión

Documentar el oráculo en un `README.md` dentro de su repo. Debe incluir:

- [ ] Nombre del proyecto y descripción breve
- [ ] URL pública del oráculo
- [ ] Tecnologías usadas
- [ ] Instrucciones para correrlo localmente
- [ ] Capturas de pantalla o GIF (opcional pero recomendado)

---

## Recursos generales

- [Documentación GitHub Pages](https://docs.github.com/en/pages)
- [Guía de Netlify para principiantes](https://docs.netlify.com/get-started/)
- [Vercel — primeros pasos](https://vercel.com/docs/getting-started-with-vercel)
- [Render — deploy de Python](https://render.com/docs/deploy-flask)
- [Observable — publicar notebooks](https://observablehq.com/@observablehq/publishing)



*Sesión anterior: [sesion2.md](sesion2.md)*