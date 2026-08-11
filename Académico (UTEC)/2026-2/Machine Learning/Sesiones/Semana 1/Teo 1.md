---
type: sesion-clase
curso: "Machine Learning"
codigo: "CS3061"
semana: 1
sesion: "Teoría 1"
fecha: 2026-08-10
tipo: "Teoria"
docente: "Luque Mamani, Edson Francisco"
tags:
  - academico/sesion
  - ai/machine-learning
  - cs3061
---

# Semana 01 — Teoría 1: Introducción a Machine Learning y Paradigmas

> [!info] Referencias Rápidas
> - **Docente:** Luque Mamani, Edson Francisco
> - **Horario:** Lunes 20:00 - 22:00 (Virtual)
> - **Enfoque del Curso:** Rigor matemático-teórico (Álgebra lineal, cálculo multivariable, optimización y estadística) como base para entender e implementar modelos, no solo llamar librerías.

---

## 🎯 Definiciones Fundamentales de Machine Learning

### 1. Definición Formal de Tom Mitchell (1998)
> "Un programa de computadora aprende de la experiencia **$E$** con respecto a una clase de tareas **$T$** y una medida de rendimiento **$P$**, si su rendimiento en las tareas en **$T$**, medido por **$P$**, mejora con la experiencia **$E$**."

$$\text{ML} \iff P(T, E) \text{ incrementa al aumentar } E$$

- **$T$ (Task):** La tarea a resolver (ej. clasificar imágenes, predecir precios).
- **$E$ (Experience):** Los datos o interacciones de entrenamiento.
- **$P$ (Performance):** La métrica cuantitativa de éxito (Accuracy, F1-Score, MSE).

### 2. Definición Intuitiva de Arthur Samuel (1959)
> "Machine Learning es el campo de estudio que da a las computadoras la habilidad de aprender sin ser explícitamente programadas."

---

## 🧩 Los Tres Paradigmas de Aprendizaje

```
                            ┌─ Supervisado (Datos etiquetados: X -> y)
Machine Learning Paradigms ─┼─ No Supervisado (Solo datos X, descubrir patrones)
                            └─ Por Refuerzo (Agente, Entorno, Recompensa/Castigo)
```

1. **Aprendizaje Supervisado (*Supervised Learning*):**
   - El dataset contiene entradas $X$ y etiquetas objetivo $y$.
   - **Objetivo:** Aprender una función $f(X) \approx y$.
   - *Ramas:* Regresión (valores continuos) y Clasificación (categorías discretas).

2. **Aprendizaje No Supervisado (*Unsupervised Learning*):**
   - Solo se cuenta con datos $X$ sin etiquetas de salida.
   - **Objetivo:** Encontrar estructura oculta, agrupaciones (Clustering) o reducir dimensiones (PCA).

3. **Aprendizaje por Refuerzo (*Reinforcement Learning*):**
   - Un agente aprende a tomar decisiones secuenciales mediante interacción con un entorno, recibiendo recompensas (*rewards*) o penalizaciones.

---

## ⚙️ Reglas de Juego y Metodología del Curso

### Dinámica de Clases y Laboratorios
- **Lunes (20:00 - 22:00):** Clase Teórica.
- **Martes (09:00 - 11:00):** Exposición y revisión del laboratorio anterior en grupos de 3.
- **Miércoles (07:00 - 09:00):** Explicación del nuevo laboratorio (~6 días para desarrollo).

### Normas de Participación y Asistencia
- **Asistencia obligatoria** con 30 minutos de tolerancia.
- **Llamadas en clase:** Si el docente formula una pregunta y el alumno no responde, se computa como **inasistencia**.
- **Política de IA:** Asistentes de código (Copilot, Claude, Codex) están permitidos, pero el estudiante debe ser capaz de explicar y fundamentar matemáticamente cada línea de código.
- **Curso Candado:** Se debe aprobar el componente teórico (40%) y el práctico (60%) de forma independiente.

---

## 📋 Tareas y Acciones Inmediatas

- [ ] **Alumnos:** Formar grupo de 3 integrantes para laboratorios y registrarse en el Excel de Canvas antes del miércoles.
- [ ] **Alumnos:** Repasar fundamentos de Álgebra Lineal (vectores, matrices, operaciones), Cálculo (derivadas parciales, gradiente) y Estadística.
- [ ] **Docente:** Publicar Excel de grupos y subir slides (PPT) a Canvas.

---

## 🧠 Conceptos Evergreen Conectados
- [[Conocimiento/AI & Data Science/Framework de Tom Mitchell (T, P, E)|Framework de Tom Mitchell (T, P, E)]]
- [[Conocimiento/AI & Data Science/Paradigmas de Machine Learning|Paradigmas de Machine Learning]]
- [[Conocimiento/AI & Data Science/Supervised vs Unsupervised Learning|Supervised vs Unsupervised Learning]]
- [[Conocimiento/AI & Data Science/Gradient Descent|Gradient Descent]]
