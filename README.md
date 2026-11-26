# Cuerpo, manos y sonido · MediaPipe

**Unidad 3 · Interfaces Gráficas · Módulo de interacción natural (MediaPipe)** · Taller de Diseño de Interfaces, Ingeniería en Diseño UAI · 2026 · Prof. Jorge Forero
Autor: Luis-Felipe Benitez · Ficha: https://portafolio.insta3d.cl/mediapipe-sonoro/ · Experiencias: https://portafolio.insta3d.cl/mediapipe-sonoro/app/

Tres instrumentos que se tocan sin tocar nada: la cámara reconoce el cuerpo, las manos y los dedos, y cada gesto se convierte en música en tiempo real.

| Experiencia | Archivo | Cómo se toca |
|---|---|---|
| 🚶 **Cuerpo Sonoro** | `cuerpo.html` | Caminar a izquierda o derecha elige el acorde; manos sobre los hombros = arpa; rodillas = bombo y caja; aplausos = palmas; agacharse = filtro submarino; saltar = platillo; brazos arriba = lluvia |
| 🎧 **DJ Re-descubre** | `dj.html` | Pellizcar un disco prende o apaga su pista; mano izquierda arriba/abajo = filtro; mano derecha = eco; puño = stutter; dibujar en el aire = loop |
| ✍️ **Dibujo Sonoro** | `dibujo.html` | Dibujar con el índice; cada gesto es un instrumento (☝️ sintetizador, ✌️ theremin, 🤟 campanitas, 🤘 viento); más arriba = más agudo; la línea queda sonando en loop |

## Objetivos
- Usar el cuerpo completo, las manos y los dedos como interfaz de entrada, sin controles físicos.
- Traducir cada gesto a un parámetro sonoro claro y predecible.
- Explorar tres escalas de movimiento: cuerpo entero, manos y dedos.

## Público y contexto
Público general en exhibiciones y salas, de pie frente a una pantalla con cámara y parlantes. Pensado para que se entienda jugando, sin explicación previa.

## Tecnologías
- **MediaPipe Tasks Vision 0.10.14:** Pose Landmarker (Cuerpo Sonoro) y Hand Landmarker (DJ y Dibujo Sonoro).
- **Web Audio API:** todos los sonidos se sintetizan en el navegador.
- HTML, CSS y JavaScript, sin instalación. Nada se graba ni se envía: todo se procesa en el navegador.

## Cómo ejecutarlo
```bash
python3 -m http.server 8000
```
Abre `http://localhost:8000` en Chrome o Safari y permite la cámara. Fuera de `localhost`, la cámara exige HTTPS.

## Proceso
> 📌 **Por aportar:** bocetos del mapa gesto → sonido, capturas de cada versión y notas de pruebas con usuarios (carpeta `proceso/`).

## Video demostrativo
> 📌 **Por aportar:** video tocando las tres experiencias, subido a YouTube y enlazado aquí.
