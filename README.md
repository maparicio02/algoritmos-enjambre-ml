# 🧠 Algoritmos de Enjambre en Machine Learning

Este repositorio contiene el desarrollo de la **Actividad 3 del curso de Aprendizaje Máquina** de la Universidad Nacional del Altiplano, donde se aplican algoritmos de enjambre en diferentes problemas de Machine Learning.

---

## 📚 Contenido del Proyecto

El proyecto está dividido en 4 aplicaciones principales del algoritmo PSO:

### 🔹 1. Feature Selection con ABC
Se utilizó ABC para equilibrar la explotación y la exploración

### 🔹 2. Optimización de Hiperparámetros en CNN
Se utilizó PSO para optimizar parámetros como:
- Learning Rate
- Momentum

Esto permitió mejorar el rendimiento de una red neuronal convolucional aplicada a clasificación de imágenes.

📊 **Resultados:**
- Accuracy: **90.68%**
- F1-Score promedio: **0.906**
- Convergencia estable de la pérdida de validación :contentReference[oaicite:0]{index=0}  

---

### 🔹 3. Entrenamiento de Red Neuronal con PSO (sin Backpropagation)
Se resolvió el problema clásico **XOR** utilizando PSO para optimizar los pesos y bias de una red neuronal.

📊 **Resultados:**
- Precisión: **100%**
- Error MSE < 0.001
- Arquitectura: 2 → 8 → 1 :contentReference[oaicite:1]{index=1}  

---

### 🔹 4. Clustering con PSO (PSO Clustering)
Se aplicó PSO para realizar agrupamiento de datos sobre el dataset **Churn_Modelling.csv**, identificando patrones en clientes bancarios sin usar etiquetas.

Se incorporaron mejoras como:
- Función de aptitud basada en **WCSS**
- Inicialización inteligente
- Ajuste de centroides tipo K-Means

📊 **Resultados:**
- Clusters: 3
- Iteraciones: 50
- WCSS PSO: **88662.50**
- WCSS K-Means: **88348.89** :contentReference[oaicite:2]{index=2}  

👉 El PSO logró resultados altamente competitivos frente a K-Means.

---

## ⚙️ Fundamentos del PSO

El algoritmo PSO simula el comportamiento de un enjambre, donde cada partícula representa una posible solución.

Cada partícula se actualiza en función de:
- 🧠 Experiencia propia (pBest)
- 🌍 Mejor solución global (gBest)

### 🔄 Etapas del algoritmo:
1. Representación de la partícula  
2. Inicialización del enjambre  
3. Evaluación (Fitness)  
4. Movimiento de partículas  
5. Evolución (exploración/explotación)  
6. Criterio de parada  

---

## 📈 Resultados Clave

- Convergencia rápida del PSO en todos los problemas
- Alta capacidad de exploración del espacio de soluciones
- Resultados comparables con métodos clásicos como K-Means
- Optimización efectiva sin uso de gradientes (en el caso de redes neuronales)

---

## 🛠️ Tecnologías Utilizadas

- Python 🐍
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Google Colab
