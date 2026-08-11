---
type: sesion-clase
curso: "Machine Learning"
codigo: "CS3061"
semana: 1
sesion: "Teoría 2"
fecha: 2026-08-11
tipo: "Teoria"
docente: "Luque Mamani, Edson Francisco"
tags:
  - academico/sesion
  - ai/supervised-learning
  - cs3061
---

# Semana 01 — Teoría 2: Aprendizaje Supervisado, Generalización y Dimensionalidad

> [!info] Referencias Rápidas
> - **Docente:** Luque Mamani, Edson Francisco
> - **Horario:** Martes 09:00 - 11:00 (Virtual)
> - **Eje Central:** Formalización matemática del aprendizaje supervisado, división de datasets, detección de sobreajuste (*overfitting*), dimensionalidad y aplicaciones reales (Visión / NLP).

---

## 📐 1. Representación Formal del Dataset y Notación Matemática

Un dataset supervisado $\mathcal{D}$ se compone de $N$ muestras con $D$ características (*features*) y una variable objetivo (*Target*):

$$\mathcal{D} = \left\{ (\mathbf{x}^{(i)}, y^{(i)}) \right\}_{i=1}^N \quad \text{donde} \quad \mathbf{x}^{(i)} = [x_1^{(i)}, x_2^{(i)}, \dots, x_D^{(i)}]^T \in \mathbb{R}^D, \quad y^{(i)} \in \mathcal{Y}$$

- **Matriz de Diseño ($X \in \mathbb{R}^{N \times D}$):** Cada fila representa una observación y cada columna una variable independiente.
- **Vector de Target ($\mathbf{y} \in \mathbb{R}^N$):** Las etiquetas reales que el modelo intenta predecir.
- **Función de Hipótesis ($\hat{y} = f(\mathbf{x}; \mathbf{w})$):** Donde $\mathbf{w}$ son los pesos asignados a cada variable que determinan su impacto en la predicción.
- **Manejo de Outliers:** A mayor volumen de datos, mayor presencia de valores atípicos que pueden distorsionar el ajuste de la función si no se limpian o tratan.

---

## ⚖️ 2. Regresión vs. Clasificación en Aprendizaje Supervisado

| Criterio | Regresión | Clasificación |
| :--- | :--- | :--- |
| **Naturaleza del Target ($\mathcal{Y}$)** | **Continua** ($\mathcal{Y} \subseteq \mathbb{R}$) | **Discreta / Categórica** ($\mathcal{Y} \in \{0, 1\}$ o $\{C_1, \dots, C_K\}$) |
| **Ejemplo Típico** | Predicción del precio de un inmueble ($) según m² | Clasificar tipo de inmueble (*Casa* vs. *Departamento*) |
| **Objetivo del Modelo** | Ajustar una curva/superficie continua | Encontrar una frontera de decisión (*decision boundary*) |
| **Complejidad del Ajuste** | Lineal ($y = \mathbf{w}^T\mathbf{x} + b$) vs. Polinomial | Clasificador lineal (Logística) vs. No lineal (SVM Kernels, Árboles) |

> [!note] Clasificación vs. Clustering (Diferencia Clave)
> - **Clasificación (Supervisado):** Separa los datos basándose en **etiquetas conocidas previas**.
> - **Clustering (No Supervisado):** Agrupa datos basándose en **similitud o métricas de distancia** sin conocer clases de antemano (ej. K-Means, KNN no supervisado).

---

## ⚠️ 3. Partición del Dataset y el Peligro del Overfitting

```
┌─────────────────────────────────────────────────────────┐
│                    Dataset Completo                     │
└────────────────────────────┬────────────────────────────┘
                             │
            ┌────────────────┴────────────────┐
            ▼                                 ▼
┌───────────────────────┐         ┌───────────────────────┐
│  Train Set (70% - 90%)│         │   Test Set (10% - 30%)│
│  (Ajuste de pesos w)  │         │(Evaluación Incorrupta)│
└───────────────────────┘         └───────────────────────┘
```

### La Ilusión del Error Cero (*Overfitting*):
- Un modelo con **Error de Entrenamiento $\approx 0$** o **Accuracy $= 0.99$** no es un buen modelo: es motivo de sospecha porque suele indicar **memorización** en lugar de aprendizaje.
- El objetivo real es la **Capacidad de Generalización:** rendir bien frente a datos nunca antes vistos en el *Test Set*.

---

## 🌌 4. La Maldición de la Dimensionalidad

- **Problema:** A medida que agregamos más *features* ($D \gg 1$), el espacio geométrico crece exponencialmente y los datos se vuelven dispersos (*sparse*), haciendo imposible la inspección visual directa.
- **Solución:** Métodos de **Reducción de Dimensionalidad** (como **PCA** para proyección lineal o **t-SNE/UMAP** para visualización no lineal en 2D/3D).
- **Regla Práctica de Elección:**
  - *Pocos datos (~20 muestras):* Modelos simples (Regresión lineal, regularización fuerte).
  - *Miles/Millones de datos:* Métodos de alta capacidad (SVM con kernels, Redes Neuronales Profundas).

---

## 🚀 5. Aplicaciones en Visión y NLP + El Reto de Producción

1. **Visión Computacional:**
   - La entrada es un tensor de píxeles (matrices RGB). 
   - Aplanar la imagen pierde la correlación de vecindad; las **CNN (Redes Convolucionales)** resuelven esto preservando la información espacial jerárquica (bordes $\to$ texturas $\to$ partes $\to$ objetos).
2. **Procesamiento de Lenguaje Natural (NLP):**
   - Traducción automática (Entrada = secuencia de caracteres/tokens $\to$ Salida = traducción).
3. **Data Drift / Cambio de Distribución en Producción:**
   - Un modelo entrenado con una distribución $P_{\text{train}}(X)$ fallará en producción si la distribución del mundo real $P_{\text{prod}}(X)$ cambia con el tiempo (*Concept/Data Drift*). Razón por la cual la disciplina de **MLOps** es fundamental en la industria.

---

## ❓ Preguntas de Debate y Enfoque de Examen

> [!tip]+ Checklist de Preguntas Teóricas
> - [ ] **Definir la diferencia matemática entre Regresión y Clasificación.**
> - [ ] **¿Por qué un accuracy de 99.9% en entrenamiento suele ser una señal de alerta?** (Explicar overfitting vs. generalización).
> - [ ] **Explicar el papel de la matriz de pesos $\mathbf{w}$ en modelos lineales y redes neuronales.**
> - [ ] **Diferenciar formalmente Clasificación de Clustering.**
> - [ ] **¿Qué es la maldición de la dimensionalidad y cómo ayuda PCA a mitigarla?**

---

## 📋 Próximos Pasos (Laboratorio de Mañana)

- [ ] **Alumnos:** Registrar los grupos de 3 en el Excel de Canvas antes del miércoles.
- [ ] **Mañana (Miércoles 07:00):** Sesión práctica de laboratorio — explicación de herramientas (Jupyter, NumPy, Pandas, Scikit-learn), formato de entrega y asignación del Lab 1 (~6 días para entrega).
- [ ] **Revisión recomendada:** Conceptos de MLOps y monitoreo de distribución de datos.

---

## 🧠 Conceptos Evergreen Conectados
- [[Conocimiento/AI & Data Science/Supervised vs Unsupervised Learning|Supervised vs Unsupervised Learning]]
- [[Conocimiento/AI & Data Science/Regresión vs Clasificación|Regresión vs Clasificación]]
- [[Conocimiento/AI & Data Science/Overfitting y Generalización|Overfitting y Generalización]]
- [[Conocimiento/AI & Data Science/Maldición de la Dimensionalidad|Maldición de la Dimensionalidad]]
- [[Conocimiento/AI & Data Science/Reducción de Dimensionalidad (PCA y t-SNE)|Reducción de Dimensionalidad (PCA y t-SNE)]]
