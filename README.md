# Red Neuronal para Conversión de Temperatura (Celsius a Fahrenheit)

Este proyecto implementa una red neuronal simple utilizando TensorFlow y Keras para convertir temperaturas de Celsius a Fahrenheit. Aunque inicialmente se planteó como una red de una sola neurona, evolucionó a una arquitectura más compleja con capas ocultas para mejorar su precisión.

## Características

- Red neuronal con arquitectura: 1 neurona de entrada, 2 capas ocultas (3 neuronas cada una) y 1 neurona de salida
- Función de pérdida: Error cuadrático medio (MSE)
- Optimizador: Adam con tasa de aprendizaje de 0.1
- Entrenamiento con 1000 épocas

## Requisitos

- Python 3.x
- TensorFlow 2.x
- NumPy
- Matplotlib (para visualización)

## Instalación

1. Clona el repositorio o descarga los archivos
2. Instala las dependencias:
   ```bash
   pip install tensorflow numpy matplotlib

## USO

El código principal realiza las siguientes acciones:

Define los datos de entrenamiento (pares Celsius-Fahrenheit)

Construye la arquitectura de la red neuronal

Entrena el modelo

Muestra la gráfica de pérdida durante el entrenamiento

Realiza una predicción de ejemplo (200°C a Fahrenheit)

Muestra los pesos aprendidos por el modelo
Para ejecutar: 
python temperatura_red_neuronal.py
Resultados
El modelo logra aprender la relación no lineal entre Celsius y Fahrenheit. En la predicción de ejemplo:

Input: 200°C

Output: ~391.54°F (el valor real es 392°F)

La gráfica de pérdida muestra cómo disminuye el error durante el entrenamiento.

Estructura del Modelo
Capa oculta 1: 3 neuronas con pesos [[ 0.0687967, 0.22337745, -0.5392805 ]] y biases [1.8656694, 3.0944872, -3.2129369]

Capa oculta 2: 3 neuronas con pesos complejos y biases [-2.8409283, -3.117581, 3.121324]

Capa de salida: 1 neurona con pesos [[-0.9222508], [-1.3829153], [1.4113914]] y bias [3.1110375]

Posibles Mejoras
Aumentar el conjunto de datos de entrenamiento

Experimentar con diferentes arquitecturas de red

Ajustar hiperparámetros (tasa de aprendizaje, épocas)

Implementar validación cruzada

Notas
Este proyecto fue desarrollado originalmente en Google Colab como ejercicio de aprendizaje sobre redes neuronales básicas. La evolución de una neurona simple a una red con capas ocultas demuestra cómo aumentar la complejidad puede mejorar los resultados.

Este README incluye:
1. Título descriptivo
2. Secciones organizadas
3. Explicación del código
4. Resultados obtenidos
5. Estructura técnica
6. Posibles mejoras
7. Notas contextuales
