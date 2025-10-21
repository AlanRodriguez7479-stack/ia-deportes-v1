Descripción de Componentes y Planes del Proyecto (Clasificador de Deportes)
Front-end
Descripción: Es la interfaz web simple donde el usuario interactúa. Actualmente, consiste en un botón o un área para "arrastrar y soltar" (drag-and-drop) donde el usuario sube una imagen desde su computadora. Una vez procesada, el front-end muestra el resultado (el nombre del deporte) de forma clara, por ejemplo: "El deporte detectado es: Fútbol".

Planes a Futuro: Mejorar la interfaz para permitir cargar múltiples imágenes y procesarlas en lote. Además, planeamos mostrar la "puntuación de confianza" de la IA ("Fútbol: 95%, Rugby: 3%..."), para que el usuario sepa qué tan segura está la IA de su predicción.

Back-end
Descripción: El servidor es montado utilizando FastAPI que recibe la imagen que el front-end le envía. Tiene un endpoint que toma esa imagen, la pre-procesa  y la pasa al modelo de IA. Luego, recibe la predicción del modelo y la devuelve al front-end en un formato simple.

Planes a Futuro: Optimizar el pre-procesamiento de imágenes para que sea más preciso. El plan principal es refactorizar el endpoint para que pueda manejar una mayor carga de peticiones simultáneas (escalabilidad) y añadir un sistema de caché para imágenes que se consulten frecuentemente.

Utilizar una IA
Descripción: Es el componente central. Se trata de un modelo de clasificación de imágenes, que se busca entrenar y optimizar un dataset con miles de imágenes etiquetadas (Fútbol, Baloncesto, Tenis, Béisbol, etc.). Su único trabajo es recibir una imagen y devolver el nombre del deporte.

Planes a Futuro: La prioridad es mejorar la precisión del modelo. Esto se logrará re-entrenándolo con un dataset mucho más grande y variado (diferentes ángulos, calidades de imagen, a mediano plazo, planeamos añadir más categorías de deportes para hacerlo más robusto.

Presentación del Proyecto
Descripción: El repositorio incluirá los recursos de la presentación (como diapositivas o un resumen ejecutivo). Esta presentación explicará el objetivo del proyecto: cómo la aplicación web, construida en React, permite a los usuarios subir una imagen, la cual es enviada a un servidor de FastAPI para ser analizada. Mostrará visualmente el flujo de trabajo, desde la interfaz de usuario hasta la respuesta del modelo de IA.

Tutorial de Despliegue
De momento estará disponible en un Github Pages.

Capturas:

<img width="876" height="616" alt="1_" src="https://github.com/user-attachments/assets/e3e40d74-e6b6-44be-b435-b1104342bce6" />
<img width="848" height="871" alt="2_" src="https://github.com/user-attachments/assets/47919a8f-5afa-4937-9685-7b5646e84d0d" />
<img width="815" height="890" alt="3_" src="https://github.com/user-attachments/assets/550c8f7b-04b5-4de3-b435-82de73cb2d62" />
