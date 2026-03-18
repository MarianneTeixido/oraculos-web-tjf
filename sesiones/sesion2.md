# Taller de Oráculos THF
## Sesión 2: ipersticiones, herramientas y tecnologías para la creación de oráculos web. 
### Desarrollo de piezas.  

Pensemos los oráculos como una práctica artística narrativa que nos permita crear **hipersticiones** de futuros otros, nuestros, especulativos, que nos permitan reconfigurar el presente.

---

## Estructura de la sesión

### Ejercicios:
1. Definir el **concepto de nuestro oráculo**
2. Modificar una **plantilla p5.js** para empezar a probar

---

## Preguntas para definir tu oráculo

### Si tu oráculo pudiera responder solo **una pregunta**, ¿cuál sería?

- ¿Qué debo observar hoy?
- ¿Qué energía, sensación, problema, pensamiento me atraviesa este momento?
- ¿Qué debo dejar ir?
- *(Tu propia pregunta)*

### ¿De dónde vendrían las respuestas?

Piensa con qué entidad divina te quieres comunicar y cómo. ¿Qué o quién será la agencia intermediaria?

### ¿Con qué entidad te estás intentando comunicar?

- Textos
- Imágenes
- Sonidos
- Frases generativas
- Cartas
- Combinaciones aleatorias
- Datos externos (API's, sensores, etc.)

---

## ¿Qué tipo de oráculo queremos hacer?

Consideremos que los oráculos pueden ser:
- Fotografías
- Un PDF
- Una instrucción
- Una página web interactiva
- Una instalación
- Una receta de cocina
- Un texto performático
- Una escultura

La idea es que, independientemente del soporte, pueda estar disponible en una página web.

---

## Principios para una internet feminista y transfeminista

Pensemos en descentralizar internet de las RRSS y mejor sembremos jardines con las semillas que cargamos en nuestras bolsas narrativas.

[Principios para una internet feminista](https://feministinternet.org/en/principles)

---

## Herramientas técnicas

En el taller les compartiré una forma de usar **P5.js**, creado por Lauren McCarty, para dar forma a nuestros oráculos. Pero siéntete libre de usar la tecnología que prefieras:

- Fotografía
- API's
- Escritura
- MediaPipe
- Cocina
- ESP32
- Textiles
- Escultura
- Tu cuerpo
- Lo que imagines

---

## Código: estructura base

### Estructura general de los ejemplos en P5.js

```
setup()
  └─ lanzarFrase()

draw() [LOOP PRINCIPAL]
  ├─ drawTitulo()
  ├─ drawFrase()
  │    └─ [lógica de ajuste de texto]
  └─ drawBoton()
       └─ [detección de hover]

mousePressed()
  └─ dispararFrase()
       └─ [actualización de variables]

windowResized()
  └─ [reajuste de posiciones]
```

### Ejemplos de código

- **[Ejemplo básico: frases aleatorias](https://editor.p5js.org/MarianneTeixido/sketches/G7wSsiglZ
)** - Estructura sencilla para empezar
- **[Oráculo con frases según hora del día](https://editor.p5js.org/MarianneTeixido/sketches/nXUQ5-tgo)** - Responde diferente según el momento

### Ejemplo Marianne

> "Yo quiero hacer un oráculo sobre el cuerpo en donde me quiero conectar con el cuerpo, la mediación es la interfaz de la máquina. Para hacer mi oráculo puse frases del texto *Corpus* de Jean Luc Nancy, las cuales cada vez que se genera una consulta te arroja una frase para conectar con lo que tu cuerpo necesita en ese momento. En su realización es un sketch de P5 con un arreglo de frases que al pulsar el botón te devuelve una elegida al azar."

**[Ver ejemplo Marianne](https://editor.p5js.org/MarianneTeixido/sketches/4SPw9bFcl)**
---

## Tipos de oráculos (con ejemplos)

### Oráculo de selección
- Elige un elemento aleatorio de una lista
- **[Ejemplo con texto](https://editor.p5js.org/MarianneTeixido/sketches/JxmpiHzEm)**

### Oráculo combinatorio
- Mezcla dos o más listas de texto
- **[Ejemplo combinatorio](https://editor.p5js.org/MarianneTeixido/sketches/ww4JFCWDi)**

### Oráculo visual
- Usa formas / colores / símbolos
- **[Ejemplo solo imagen](pendiente)**
Pendiente

### Oráculo combinatorio visual y textual
- Usa formas, colores, símbolos y texto combinados
- **[Ejemplo imagen - texto](https://editor.p5js.org/MarianneTeixido/sketches/X1WIpjJVy)**

### Oráculo de selección de sonidos
- pendiente

### Oráculo combinatorio sonido - texto
pendiente


## Consideraciones técnicas para publicar

### Opciones de desarrollo

| Si ya programas | Si usas editor p5.js |
|-----------------|----------------------|
| Python local | Editor web de p5.js |
| npm / npx | Límite: 20 MB para recursos multimedia |
| Servidor local | |

### Almacenamiento de recursos

**Repositorios de GitHub:**
- Espacio generoso para código
- Para multimedia, usar recursos externos

**Usar recursos externos:**
El link debe terminar en la extensión del archivo:
- `.mov`, `.mp4` (video)
- `.mp3`, `.wav` (audio)
- `.jpg`, `.png` (imagen)

**Opciones para almacenar archivos:**

- **[catbox.moe](https://catbox.moe)** - Subida temporal y sencilla, no requiere cuenta
- **[Usar el mismo editor de P5js](https://editor.p5js.org)** - Subir assets directamente en el editor
- **Almacenar archivos localmente**
  

---

### Disclaimer importante ⚠️

> Este es un espacio de experimentación. No necesitas saber programar para crear un oráculo. El código es una herramienta más, como el bordado, la cocina o la escritura. Si es tu primera vez con p5.js, bienvenida: aquí se aprende haciendo, equivocándose y preguntando.    
> Estos ejercicio los trabajé de la siguiente forma. Le pasé un codigo, sencillo pero funcional (de los primero ejemplos puestos acá) hecho por mi a Claude. Me fue devolviendo los ejercicios template de los cuales a no todos los modifiqué el contenido. Lo importante de los proyectos que hagan, más allá del código o las herramientas, es lo que dice su oráculo, con sus imágenes, textos, sonidos, procesos. Ahí esta la magia de verdad. <3 
---

## Dinámica: diseña tu oráculo

### Breakout rooms (3 personas por grupo)

Cada grupo puede:
- Trabajar **juntes** en un mismo oráculo
- O **cada quien en su proyecto**, pero ayudándose

**Esto es clave:** el formato no es lo importante, sino el concepto.

### Regreso al grupo: intercambio rápido (20 minutos)

Cada persona comparte en **1 minuto**:
- **Nombre del oráculo**
- **Qué pregunta responde**
- **Cómo funciona**

---

## Plantilla de diseño del oráculo

### Pregunta fundamental
¿Qué tipo de pregunta responde tu oráculo?
_________________________________

### Mecanismo de decisión
¿Cómo decide el oráculo la respuesta?
- [ ] Random simple (aleatorio)
- [ ] Combinaciones (mezcla de elementos)
- [ ] Tiempo (hora del día, fecha)
- [ ] Clicks (número de interacciones)
- [ ] Movimiento del mouse
- [ ] Datos externos (API)
- [ ] Otro: _________________

### Interfaz de consulta
¿Cómo lo consulta el usuario?
- [ ] Botón
- [ ] Carta (click en imagen)
- [ ] Escribir pregunta
- [ ] Sacudir celular
- [ ] Movimiento
- [ ] Voz
- [ ] Otro: _________________

---

## Tercera Sesión (Preparación)

Para la siguiente sesión trabajaremos con:
- Una **idea clara** de tu oráculo
- Un **prototipo básico** funcionando (aunque sea muy sencillo)
- **Problemas o preguntas** específicas que quieras resolver

---

## Glosario técnico

| Término | Significado |
|---------|-------------|
| **Arreglo** | Lista de elementos (frases, imágenes, números) guardados juntos |
| **Índice del arreglo** | La posición de un elemento en la lista (empieza en 0) |
| **Función** | Caja negra que realiza una acción; tiene un valor de entrada y otro de salida |
| **Loop** | Ciclo que se repite (como `draw()` que corre 60 veces por segundo) |
| **Variable** | Caja donde guardamos información que puede cambiar |
| **Evento** | Acción del usuario (click, mover mouse, teclear) |
| **API** | Interfaz que conecta tu programa con datos externos |

---

## Recursos

- [Editor p5.js](https://editor.p5js.org)
- [Referencia de p5.js](https://p5js.org/reference/)
- [Catbox - Almacenamiento temporal](https://catbox.moe)

---

> **Todavía hay semillas para recolectar, y espacio en la bolsa
de estrellas.** 𖡼.𖤣𖥧𖡼.𖤣𖥧.☘︎ ݁˖༘⋆⋆｡°✩.✩₊˚.⋆☾⋆⁺₊✧
Úsula K. Leguin
