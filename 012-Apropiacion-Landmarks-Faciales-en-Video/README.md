# Detección de Rostro y Puntos Faciales desde Webcam

Este cuaderno de Google Colab tiene como objetivo principal servir como una herramienta educativa y demostrativa para explorar el uso de la librería MediaPipe en la implementación de tareas de visión artificial en tiempo real, específicamente la detección de rostros, la identificación de puntos faciales clave y la segmentación de figura humana, utilizando la cámara web como fuente de entrada de video.

## Autor

**Andres Alievi**

## Funcionalidades

Este cuaderno implementa las siguientes funcionalidades:

*   **Detección de Rostros:** Identifica la presencia de rostros en el stream de video de la webcam utilizando el modelo BlazeFace de MediaPipe.
*   **Detección de Puntos Faciales (Face Mesh):** Localiza y mapea 468 puntos clave (landmarks) en el rostro detectado para análisis detallado.
*   **Segmentación de Figura Humana:** Detecta y segmenta la figura humana en el stream de video, permitiendo aplicar efectos como cambio de fondo.
*   **Procesamiento en Tiempo Real:** Procesa los frames de video en tiempo real para visualizar las detecciones y segmentaciones.
*   **Interfaz Interactiva:** Permite iniciar y detener el procesamiento de video haciendo clic en la ventana de visualización.

## Requisitos

Para ejecutar este cuaderno, necesitas:

*   Una cuenta de Google con acceso a Google Colab.
*   Una webcam funcional conectada a tu dispositivo.
*   Conexión a internet para descargar las librerías y modelos necesarios.

Las librerías de Python y los modelos de MediaPipe se instalan automáticamente al ejecutar las celdas correspondientes en el cuaderno.

## Uso

1.  Abre el cuaderno en Google Colab.
2.  Ejecuta todas las celdas en orden.
3.  Cuando se te solicite, permite el acceso a tu webcam.
4.  Observa la ventana de video que mostrará la detección de rostros, puntos faciales y/o la segmentación según la sección que estés ejecutando.
5.  Haz clic en la ventana de video para detener el procesamiento.

**Nota:** Puede ser necesario ejecutar algunas celdas varias veces o reiniciar la sesión de Colab para que todas las librerías se instalen correctamente, especialmente si experimentas errores de importación.

## Estructura del Cuaderno

El cuaderno está organizado en las siguientes secciones:

1.  **Instalación de Librerías:** Instala las dependencias necesarias como `numpy`, `mediapipe`, y `opencv-python`.
2.  **Importación de Librerías:** Importa los módulos de Python requeridos.
3.  **Importación y Seteo de Modelos:** Descarga y configura los modelos de detección de rostros y puntos faciales de MediaPipe.
4.  **Código para Interacción con el Navegador:** Funciones JavaScript y Python para capturar frames de la webcam y mostrar resultados en el navegador.
5.  **Función Principal de Video Streaming:** Define la función que activa el stream de video de la webcam.
6.  **Función para Dibujar Landmarks:** Helper para visualizar los puntos faciales detectados.
7.  **Streaming con Detección de Rostro y Puntos:** Implementación del procesamiento en tiempo real para detección de rostros y puntos faciales.
8.  **Segmentación de Figura Humana:** Implementación del procesamiento en tiempo real para segmentación de figura humana, incluyendo la posibilidad de cambiar el fondo.

## Créditos

Este cuaderno adapta y utiliza código de los siguientes recursos:

*   [Artículo sobre MediaPipe](https://www-assemblyai-com.translate.goog/blog/mediapipe-for-dummies?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=tc) (Traducido al español)
*   [Cuaderno de Google Colab para Captura de Video](https://colab.research.google.com/drive/1QnC7lV7oVFk5OZCm75fqbLAfD9qBy9bw?usp=sharing)

## Autor

Andres Alievi
