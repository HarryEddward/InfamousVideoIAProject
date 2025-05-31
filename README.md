# Detección y Seguimiento de Personas por Video con IA

Este proyecto busca simular una inteligencia artificial que observa a las personas en tiempo real a través un video en pantalla, generando la ilusión de que la "persona dentro del video" te está mirando directamente, como si fuera real.

## Especificaciones del proyecto
Al usar IA, Python tiene una comunidad basta para completarse muchas de las funciones sin tanto boilerplate y de forma senzilla al enfocarse como lenguaje de programación a la IA.

En el caso usaríamos librerías ya creadas para facilitarnos el desarollo del proyecto sin tanta inversión de tiempo con librerías ya hechas.

## Librerías de Python:

| Librería                | Descripción                                                                          |
| ----------------------- | ------------------------------------------------------------------------------------ |
| `opencv-python`         | Procesamiento de imágenes y detección de objetos/personas.                           |
| `numpy`                 | Manipulación de arrays y procesamiento numérico (útil para imágenes).                |
| `imutils`               | Funciones útiles para trabajar con OpenCV (redimensionar, dibujar, etc.).            |
| `mediapipe`             | Detección precisa de poses humanas, manos y rostros. Útil para seguimiento avanzado. |
| `dlib`                  | Detección y seguimiento facial más precisa (requiere CMake).                         |
| `torch` o `tensorflow`  | Para aplicar modelos de IA si decides entrenar algo más complejo.                    |
| `pygame` o `tkinter`    | Si quieres mostrar el video procesado en una interfaz personalizada.                 |
| `threading` / `asyncio` | Para mejorar el rendimiento en tiempo real al procesar video.                        |


### Idea General
La idea es realizar una conexión en tiempo real con una cámara, usando OpenCV para detectar rostros y movimiento, y MediaPipe para inferir emociones o posturas. Basado en esa información, se mostrarán en pantalla clips de video que representen comportamientos realistas, como si la figura en pantalla estuviera reaccionando al usuario.

Algunos puntos clave:

- Seguimiento facial para simular contacto visual.

- Análisis emocional para cambiar expresiones o comportamientos de la IA.

- Videos en bucle pre-renderizados que simulan respuestas humanas.

- Simulación de infrarrojos para agregar un toque más técnico sin sensores físicos.

- Bajo consumo de recursos, ideal para ejecutarse sin GPU dedicada, usando IA pre-entrenada y lógica condicional simple.

- Posible integración de PyTorch para comportamientos más avanzados con modelos ligeros si se requiere.
