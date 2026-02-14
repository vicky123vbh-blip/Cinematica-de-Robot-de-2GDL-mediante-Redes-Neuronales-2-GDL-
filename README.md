# Cinemática de un Robot mediante Redes Neuronales (2 GDL)
### Pruebas Preliminares de Tesis | Ingeniería Mecatrónica

Este repositorio contiene el desarrollo y validación de modelos de Inteligencia Artificial aplicados a la cinemática de un manipulador planar de 2 Grados de Libertad (GDL). Estos experimentos sirvieron como base para la implementación final en el robot **UR3e**.

---

## Descripción del Proyecto
El objetivo fue entrenar una red neuronal capaz de aprender la relación entre los ángulos de las articulaciones (\theta_1, \theta_2) y las coordenadas cartesianas (x, y), eliminando la necesidad de resolver ecuaciones trigonométricas complejas de forma manual.

### Especificaciones Técnicas
* **Arquitectura:** Red Neuronal Prealimentada (MLP).
* **Entradas:** 2 nodos (Valores de theta en grados).
* **Capas Ocultas:** 2 capas densas de 64 neuronas (ReLU y Sigmoid).
* **Salida:** 2 nodos (Coordenadas x, y).



---

##  Contenido del Repositorio
A continuación, se describen los cuadernos de Jupyter (`.ipynb`) incluidos:

### 1. [Predicción de Coordenadas](https://github.com/TU_USUARIO/NOMBRE_REPO/blob/main/PrediccionROBOT.ipynb)
Este archivo contiene el entrenamiento del modelo. Se enfoca en la **Cinemática Directa**, donde la red aprende a predecir la posición del efector final basándose en la configuración articular.

### 2. [Controlador Definitivo](https://github.com/TU_USUARIO/NOMBRE_REPO/blob/main/CONTROLADOR_definitivo.ipynb)
Implementación de la red entrenada para el control del movimiento. Incluye la lógica de predicción que posteriormente fue escalada para el robot industrial **UR3e** en el laboratorio.

---

##  Resultados Preliminares
* **Convergencia:** El modelo alcanzó un error cuadrático medio (MSE) mínimo, validando la arquitectura de 64 neuronas.
* **Generalización:** La red logró predecir puntos no incluidos en el dataset original con alta precisión.

---

##  Requisitos
Para ejecutar estos modelos, es necesario contar con:
* Python 3.x
* TensorFlow / Keras
* NumPy & Matplotlib
* Jupyter Notebook / Google Colab

---
**Contacto:** Victoria Bello - Estudiante de Ingeniería Mecatónica.
