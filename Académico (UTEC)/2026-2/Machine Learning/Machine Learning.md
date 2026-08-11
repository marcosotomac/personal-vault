---
type: curso-hub
codigo: "CS3061"
curso: "Machine Learning"
nivel: 6
ciclo: "2026-2"
creditos: 4
seccion: "2"
tipo: "Obligatorio"
docente: "Luque Mamani, Edson Francisco"
modalidad: "Virtual"
tags:
  - academico/curso
  - ciclo/2026-2
  - area/ia
---

# Machine Learning

> [!info] Ficha Técnica
> - **Docente:** Luque Mamani, Edson Francisco
> - **Código:** CS3061 | **Créditos:** 4 | **Sección:** 2 | **Nivel:** 6
> - **Horario:**
>   - **Lunes:** 20:00 - 22:00 (Teoría Virtual)
>   - **Martes:** 09:00 - 11:00 (Laboratorio Virtual — Revisión/Exposición)
>   - **Miércoles:** 07:00 - 09:00 (Laboratorio Virtual — Explicación de nuevo Lab)
> - **Plataformas:** [Canvas UTEC](https://utec.instructure.com) • [Google Calendar Event](https://calendar.google.com)

---

## 📊 Sistema de Evaluación Oficial (Sílabo)

$$\text{NF} = 0.10 \cdot \text{EP} + 0.30 \cdot \text{EF} + 0.10 \cdot \text{P1} + 0.30 \cdot \text{P2} + 0.10 \cdot \text{EC1} + 0.10 \cdot \text{EC2}$$

| Componente | Código | Peso (%) | Semana Oficial | Descripción / Dinámica |
| :--- | :---: | :---: | :---: | :--- |
| **Proyecto 1** | P1 | 10% | Semana 07 | Proyecto de primera etapa |
| **Evaluación Continua 1** | EC1 | 10% | Semana 08 | Exposición de laboratorios (Martes) + Quizzes en clase |
| **Examen Parcial** | EP | 10% | Semana 08 | Evaluación teórica individual |
| **Evaluación Continua 2** | EC2 | 10% | Semana 15 | Exposición de laboratorios (Martes) + Quizzes en clase |
| **Proyecto 2 (Final)** | P2 | 30% | Semana 16 | Proyecto aplicado en equipos de hasta 5 |
| **Examen Final** | EF | 30% | Semana 16 | Evaluación teórica acumulativa |

> [!warning] Reglas Críticas del Curso
> - **Curso Candado:** Se debe aprobar la teoría (40%) y la práctica/laboratorio (60%) por separado.
> - **Asistencia:** Obligatoria con 30 minutos de tolerancia. Si el alumno no responde al ser llamado en clase, se registra como inasistente.
> - **Política de IA:** Permitido el uso de asistentes de código (Copilot, Claude, Codex), pero se exige dominio total y defensa del fundamento matemático.

---

## 🔄 Dinámica Semanal de Laboratorios

```
Lunes (20:00 - 22:00) ➔ Clase Teórica del tema semanal
Martes (09:00 - 11:00) ➔ Revisión y exposición del laboratorio anterior (Grupos de 3)
Miércoles (07:00 - 09:00) ➔ Explicación del nuevo laboratorio (~6 días de desarrollo)
```

- **Grupos de Laboratorio:** Máximo 3 integrantes formados por afinidad (registro en Excel de Canvas).
- **Grupos de Proyecto Final:** Máximo 5 integrantes por sorteo a partir de la Semana 7.

---

## 🗺️ Mapa Temático del Sílabo

### Etapa 1: Fundamentos y Modelos Clásicos (Semanas 1–7)
- **1. Introducción y Paradigmas:** Framework de Tom Mitchell ($T, P, E$), Pipeline End-to-End.
- **2. Aprendizaje Supervisado (Regresión):** Regresión lineal/no lineal, Funciones de pérdida (Loss), Optimización con Gradient Descent (GD, SGD, Mini-batch).
- **3. Evaluación y Generalización:** Regularización ($L_0, L_1, L_2$), Bias-Variance Tradeoff, Cross Validation, Hyperparameter Tuning, Desbalance de clases.
- **4. Feature Engineering:** Feature Scaling, Polynomial Features, Transformaciones y Feature Maps.
- **5. Métodos Probabilísticos:** PAC Learning, Maximum Likelihood Estimate (MLE), Maximum a Posteriori (MAP), Naive Bayes.
- **6. Aprendizaje Supervisado (Clasificación):** Regresión Logística, SVM con Kernels, Árboles de Decisión (ID3), Métricas (F1, Accuracy, Matriz de Confusión), Ensamblajes (Bagging, Boosting, Random Forest).

### Etapa 2: Redes Neuronales y No Supervisado (Semanas 7–16)
- **7. Redes Neuronales:** Arquitecturas Fully Connected, Feed-forward, Backpropagation, Regularización (Dropout, BatchNorm).
- **8. Reducción de Dimensionalidad:** PCA, LDA, Factor Analysis, Visualización con t-SNE y UMAP.
- **9. Aprendizaje No Supervisado (Clustering):** K-Means, Mean-Shift, Clustering Jerárquico, DBSCAN, Gaussian Mixture Models (GMM), Métricas de clustering.
- **10. Learning Theory e Interpretabilidad:** Sesgo algorítmico, interpretabilidad y explicabilidad de modelos.

---

## 📂 Sesiones del Ciclo
- [x] [[Sesiones/Semana 1/Teo 1|Semana 01 - Teoría 1: Introducción a Machine Learning y Paradigmas]]
- [ ] [[Sesiones/Semana 1/Lab 1|Semana 01 - Lab 1: Explicación de Laboratorio 1]]
- [ ] [[Sesiones/Semana 2/Teo 2|Semana 02 - Teoría 2: Regresión Lineal y Gradient Descent]]

---

## 🎯 Entregables y Proyectos
- [ ] **Lab 01:** Pipeline de Preprocesamiento y Regresión Lineal
- [ ] **Proyecto 1 (10% - Sem 07):** [[Entregables/Proyecto 1|P1 - Propuesta y Baseline del Modelo]]
- [ ] **Proyecto 2 (30% - Sem 16):** [[Entregables/Proyecto 2|P2 - Modelo Final, Optimización e Informe Técnico]]

---

## 📚 Bibliografía Oficial
- **Christopher M. Bishop (2007):** *Pattern Recognition and Machine Learning* (Springer) — Texto base del curso.
- **Ian Goodfellow, Yoshua Bengio, Aaron Courville (2016):** *Deep Learning* (MIT Press).
- **Andreas C. Müller & Sarah Guido (2016):** *Introduction to Machine Learning with Python* (O'Reilly).
- **Stephen Marsland (2011):** *Machine Learning: An Algorithmic Perspective*.

---

## 🧠 Conceptos Evergreen Vinculados
- [[Conocimiento/AI & Data Science/Framework de Tom Mitchell (T, P, E)|Framework de Tom Mitchell (T, P, E)]]
- [[Conocimiento/AI & Data Science/Paradigmas de Machine Learning|Paradigmas de Machine Learning]]
- [[Conocimiento/AI & Data Science/Gradient Descent|Gradient Descent]]
- [[Conocimiento/AI & Data Science/Overfitting y Regularización|Overfitting y Regularización]]
- [[Conocimiento/AI & Data Science/Bias-Variance Tradeoff|Bias-Variance Tradeoff]]
