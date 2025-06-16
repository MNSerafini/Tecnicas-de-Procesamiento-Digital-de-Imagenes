# Interfaz Multimodelo para Generación de Imágenes con Stable Diffusion
## Autor: Martin Nicolas Serafini
## Junio 2025
---
## Descripción

Este proyecto implementa una interfaz gráfica de usuario (GUI) interactiva utilizando la librería Gradio, diseñada para facilitar la interacción con múltiples modelos pre-entrenados de generación de imágenes basados en la arquitectura Stable Diffusion. La aplicación permite a los usuarios seleccionar entre diferentes pipelines (actualmente configurados para "Openjourney" y "Dreamlike Diffusion 1.0") y ajustar parámetros clave para generar imágenes a partir de prompts textuales.

El enfoque se centra en proporcionar una herramienta accesible para experimentar con distintos estilos de generación de imágenes ofrecidos por modelos de difusión, optimizando el proceso de inferencia mediante el uso de hardware GPU y técnicas como `torch_dtype=torch.float16` y la asignación explícita al dispositivo CUDA.

## Funcionalidad

La interfaz permite:

*   **Seleccionar el Modelo de Generación:** Elegir entre los pipelines de Stable Diffusion disponibles (ej. Openjourney, Dreamlike Diffusion 1.0).
*   **Definir Prompts:** Especificar un prompt textual principal para guiar la generación de la imagen.
*   **Definir Prompt Negativo:** Opcionalmente, especificar un prompt negativo para indicar conceptos o características a evitar en la imagen generada.
*   **Controlar el Guidance Scale:** Ajustar la influencia del prompt en el proceso de difusión. Un valor más alto generalmente resulta en una imagen más cercana al prompt.
*   **Configurar el Número de Pasos de Inferencia:** Definir la cantidad de iteraciones del proceso de difusión. Un mayor número de pasos puede mejorar la calidad pero aumenta el tiempo de generación.
*   **Establecer una Semilla Aleatoria (Seed):** Asegurar la reproducibilidad de las imágenes generadas al fijar la semilla del generador aleatorio.
*   **Visualizar la Imagen Generada:** Mostrar la imagen resultante directamente en la interfaz.

## Requisitos

*   Python 3.7 o superior.
*   Entorno con acceso a una GPU compatible con CUDA (recomendado para un rendimiento óptimo). Google Colab con aceleración por hardware (GPU) es un entorno ideal.

## Instalación y Uso

### 1. Clonar el Repositorio

Clona este repositorio en tu entorno local o en Google Colab:
