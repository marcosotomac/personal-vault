---
type: sesion-clase
curso: "Evaluación Financiera de Proyectos"
codigo: "GI4101"
semana: 1
sesion: "Teoría 1"
fecha: 2026-08-11
tipo: "Teoria"
docente: "Diana Ramírez Fonseca"
tags:
  - academico/sesion
  - finanzas/evaluacion-proyectos
  - gi4101
---

# Semana 01 — Teoría 1: Fundamentos de Evaluación de Proyectos y Modelado Financiero

> [!info] Referencias Rápidas
> - **Docente:** Diana Ramírez Fonseca *(Magíster en Administración, doctoranda en Negocios, especialista en ProInnóvate)*
> - **Horario:** Martes 19:00 - 22:00 (Virtual)
> - **Herramienta Principal:** Microsoft Excel
> - **Objetivo Central:** Construcción de modelos financieros estructurados para evaluar la viabilidad económica y financiera de proyectos de inversión.

---

## 🏛️ 1. Fundamentos de Teoría Financiera

La teoría financiera analiza la asignación eficiente de recursos escasos con el objetivo de **optimizar recursos y maximizar valor económico**.

### Las Tres Decisiones Financieras Básicas
Toda estructura de flujo de caja responde a tres decisiones fundamentales:
1. **Decisión de Inversión (Capex):** ¿Qué activos tangibles e intangibles adquirir para operar?
2. **Decisión de Financiamiento:** ¿Cómo fondear la inversión? (Recursos propios / *Equity* vs. Deuda bancaria / Pasivos).
3. **Decisión de Operación (Opex):** Gestión de ingresos, costos de venta y gastos operativos del día a día.

### El Triángulo de las Inversiones
Toda decisión financiera equilibra tres variables interdependientes:
- **Riesgo:** Probabilidad de ocurrencia de eventos inesperados que afecten el retorno.
- **Rendimiento:** Tasa de ganancia generada por el activo ($\text{Mayor Riesgo} \implies \text{Mayor Rendimiento Exigido}$).
- **Liquidez:** Facilidad y velocidad para convertir la inversión en efectivo sin pérdida significativa de valor.
- *Diversificación:* Estrategia de portafolio para mitigar el riesgo no sistemático.

### Valor del Dinero en el Tiempo
$$\text{Un sol hoy vale más que un sol mañana}$$
Debido a la **inflación**, el **costo de oportunidad** y el **riesgo**. Este principio sustenta el descuento de flujos futuros en el cálculo del **VAN (Valor Actual Neto)** y la **TIR (Tasa Interna de Retorno)**.

![[Pasted image 20260811210345.png]]

---

## 🏢 2. Tipos de Proyectos y Viabilidades Requeridas

### Tipos de Proyectos en una Empresa:
- **Inversión / Expansión:** Aumento de capacidad instalada (nueva planta, maquinaria).
- **Innovación:** Lanzamiento de nuevos productos, servicios o automatización.
- **Mejora Continua:** Optimización de procesos, reducción de costos y mermas (*Lean*).
- **Estratégicos:** Internacionalización o penetración en nuevos mercados.
- **Social / Ambiental (ESG):** Eficiencia energética, sostenibilidad y cumplimiento normativo.

### Las 4 Viabilidades Clave:
1. **Viabilidad Económica/Financiera:** Los flujos proyectados cubren costos, gastos, servicio de deuda y rentabilidad exigida.
2. **Viabilidad Técnica:** Disponibilidad de tecnología, capacidad productiva y know-how.
3. **Viabilidad Ambiental:** Cumplimiento de normativas y sostenibilidad (motivo de rechazo de proyectos).
4. **Viabilidad Social:** Impacto en la comunidad, empleo y entorno.

---

## 📊 3. Arquitectura del Modelo Financiero en Excel

```
┌─────────────────────────────────────────────────────────────┐
│                 Supuestos e Inputs Base                     │
│ (Fuentes verificables: BCR, estudios de mercado, cotizaciones)│
└──────────────────────────────┬──────────────────────────────┘
                               │
            ┌──────────────────┴──────────────────┐
            ▼                                     ▼
┌──────────────────────────────┐       ┌──────────────────────────────┐
│    Proyección de Ingresos    │       │     Proyección de Costos     │
│       (Precio × Cantidad)    │       │     (Materia Prima, MOD, CIF)│
└──────────────┬───────────────┘       └──────────────┬───────────────┘
               │                                      │
               └──────────────────┬───────────────────┘
                                  ▼
┌─────────────────────────────────────────────────────────────┐
│                  Flujos de Caja Proyectados                 │
│         (Flujo de Inversión + Flujo Operativo + Deuda)       │
└──────────────────────────────┬──────────────────────────────┘
                               │
                               ▼
┌─────────────────────────────────────────────────────────────┐
│                 Evaluación y Análisis de Riesgo             │
│            (VAN, TIR, Payback, WACC, Sensibilidad)          │
└─────────────────────────────────────────────────────────────┘
```

> [!caution] Responsabilidad Ética: "El Excel Aguanta Todo"
> Cualquier modelo puede forzarse para mostrar rentabilidad positiva. La ética del evaluador radica en utilizar **supuestos realistas, transparentes y documentados** (ej. proyecciones de inflación del BCR, datos sectoriales), evitando fraudes o decisiones de inversión erróneas.

### Incorporación de Riesgos Externos y Macro:
Los modelos deben incorporar shocks exógenos cuantificables (ej. proyecciones macroeconómicas del BCR, impactos climáticos como el Fenómeno del Niño o penalidades contractuales por retrasos).

---

## 🎯 4. Especificaciones del Proyecto Grupal (Horizonte: 6 Años)

Formulación y evaluación financiera de un **nuevo emprendimiento** en equipos de **4 integrantes**:

| Etapa | Semana | Contenido Exigido | Dinámica de Evaluación |
| :--- | :---: | :--- | :--- |
| **PC1** | **Semana 06** | Identificación de problema/oportunidad, demanda proyectada, costos (MOD, MP, CIF), Flujo de Inversión (Capex) y Flujo Operativo (Opex). | Exposición grupal (10 min) + Preguntas individuales de la docente (10 min). |
| **PC2** | **Semana 14** | Correcciones de PC1 + Flujo Económico, Flujo de Deuda, Flujo Financiero, Costo de Capital (**WACC**), Indicadores (VAN, TIR, B/C, Payback) y Análisis de Sensibilidad/Escenarios. | Exposición grupal (10 min) + Preguntas individuales de la docente (10 min). |

> [!tip] Criterio para Selección de Idea
> Elegir un negocio del cual **exista información secundaria y estudios de mercado disponibles** para sustentar los supuestos de ingresos y costos. Evitar proyectos sin datos accesibles.

---

## ⚙️ 5. Sistema de Evaluación de la Materia

- **Evaluación Continua (Quizzes individuales en Canvas con Proctorio):**
  - Duración: 5 a 10 minutos al inicio de clase.
  - **C1 (Semana 07):** Promedio de quizzes clases 1 a 7 (se elimina la nota más baja).
  - **C2 (Semana 15):** Promedio de quizzes clases 8 a 15 (se elimina la nota más baja).
  - *(La participación activa en clase puede compensar notas bajas en quices).*
- **Prácticas Calificadas (Grupales):** PC1 (Semana 6) y PC2 (Semana 14).
- **Examen Parcial:** Semana 8 (Individual, virtual).
- **Examen Final:** Semana 16 (Individual, virtual con casos prácticos en Excel).

---

## 📋 6. Acciones Inmediatas para la Próxima Sesión

- [ ] **Lectura Obligatoria:** Leer el **Capítulo 1 del libro de Nassir Sapag Chain** (*Formulación y Evaluación de Proyectos*); se debatirá al inicio de la sesión 2.
- [ ] **Configuración Técnica:** Instalar y verificar **Proctorio** en Canvas para el primer quiz de la clase 2.
- [ ] **Conformación de Grupos:** Cerrar grupo de **4 integrantes** y registrarse en Canvas antes del próximo martes.
- [ ] **Definición de Idea:** Explorar ideas de negocio con datos secundarios y validarlas con la docente.

---

## 🧠 Conceptos Evergreen Conectados
- [[Conocimiento/Finanzas/Valor del Dinero en el Tiempo|Valor del Dinero en el Tiempo]]
- [[Conocimiento/Finanzas/Valor Actual Neto (VAN) y TIR|Valor Actual Neto (VAN) y TIR]]
- [[Conocimiento/Finanzas/Costo de Capital (WACC)|Costo de Capital (WACC)]]
- [[Conocimiento/Finanzas/Estructura del Flujo de Caja Libre|Estructura del Flujo de Caja Libre]]
- [[Conocimiento/Finanzas/Análisis de Sensibilidad y Escenarios|Análisis de Sensibilidad y Escenarios]]
