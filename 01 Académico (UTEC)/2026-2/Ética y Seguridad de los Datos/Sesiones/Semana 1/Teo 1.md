---
type: sesion-clase
curso: "Ética y Seguridad de los Datos"
codigo: "DS3031"
semana: 1
sesion: "Teoría 1"
fecha: 2026-08-10
tipo: "Teoria"
docente: "Pazos Ortiz, Jose Carlos"
tags:
  - academico/sesion
  - seguridad/fundamentos
  - etica/privacidad
---

# Semana 01 — Teoría 1: Fundamentos de Seguridad, Privacidad y Ética

> [!info] Referencias Rápidas
> - **Docente:** Pazos Ortiz, Jose Carlos
> - **Modalidad:** Virtual (Lunes 17:00 - 19:00)
> - **Estructura del Ciclo:** ~8 semanas de Seguridad Técnica (Criptografía, software) + ~6–7 semanas de Privacidad y Ética (Leyes, sesgo, GenAI).

---

## ✍️ Núcleo Conceptual

### 1. Las Tres Disciplinas Interrelacionadas
- **Seguridad:** ¿El sistema y los datos están técnicamente protegidos?
- **Privacidad:** ¿Qué nivel de control y consentimiento tiene el titular sobre sus datos?
- **Ética:** ¿Es correcto y justo lo que se está haciendo con la tecnología y los datos?

### 2. Tríada CIA (Information Security)
Marco central para analizar cualquier fallo o arquitectura de seguridad:
- **C — Confidentiality (Confidencialidad):** Protección de **lectura**. Solo personas autorizadas acceden a la información.
- **I — Integrity (Integridad):** Protección de **escritura / modificación**. Los datos no deben ser alterados sin autorización.
- **A — Availability (Disponibilidad):** Acceso continuo y oportuno al servicio cuando se requiere (ej. mitigación de DoS/DDoS).

### 3. Ciclo de Vida del Dato
La seguridad y la privacidad deben diseñarse desde la recolección (*Privacy by Design*), no agregarse al final:
```
Recolección ➔ Almacenamiento ➔ Procesamiento ➔ Compartición ➔ Eliminación
```

---

## 🏛️ Marco Regulatorio y Legal

### Ley 29733 (Perú) vs. GDPR (Unión Europea)
- **GDPR (General Data Protection Regulation):** Estándar global más estricto. Incluye multas masivas, designación obligatoria de Oficial de Datos (DPO) y **aplicación extraterritorial** (aplica a cualquier empresa peruana si almacena o procesa datos de ciudadanos de la UE).
- **Ley 29733 (Perú):** Regula el tratamiento de datos personales en territorio nacional. Desde 2025, empresas extranjeras que operen en Perú también deben cumplirla formalmente.

### Derechos ARCO (Control del Titular)
- **A — Acceso:** Derecho a saber qué datos personales tiene la organización.
- **R — Rectificación:** Derecho a corregir datos inexactos o desactualizados.
- **C — Cancelación:** Derecho a solicitar la eliminación de datos cuando no sean necesarios.
- **O — Oposición:** Derecho a negarse al uso de sus datos para fines específicos.

---

## 🔍 Casos de Estudio Reales Vistos en Clase

1. **Filtración RENIEC (2025):** Funcionaria con credenciales legítimas extrajo datos masivos de ciudadanos. *(Fallo de control de acceso interno e incumplimiento del deber de confidencialidad).*
2. **Municipalidad de Miraflores:** Exposición pública de datos de 82,000 vecinos en Internet. *(Negligencia en configuración, no un exploit sofisticado).*
3. **Cambridge Analytica (Facebook):** Extracción indebida de datos para perfilamiento psicológico y manipulación electoral. *(Fallo simultáneo de seguridad, privacidad y ética).*
4. **Sesgo Algorítmico en Amazon (2018):** Sistema de selección de CVs penalizaba postulaciones femeninas debido a datos históricos de entrenamiento desbalanceados.

---

## ❓ Puntos de Debate y Aclaraciones

- **¿Por qué Disponibilidad no se profundiza tanto en este curso?** Los ataques DoS/DDoS completan la tríada CIA, pero el foco principal de la materia estará puesto en confidencialidad, integridad, criptografía y privacidad.
- **Cuantificación del Sesgo Algorítmico:** No existe una métrica matemática universal; el sesgo suele emerger de datos históricos que reflejan desigualdades previas.
- **Deepfakes y Copyright en GenAI:** Frontera legal y ética abierta; los modelos actuales se entrenaron con datos sin consentimiento explícito y la regulación global sigue en desarrollo.

---

## 🎯 Puntos Clave para Examen

> [!tip]+ Checklist de Repaso para Evaluaciones
> - [ ] **Distinguir componentes de la Tríada CIA:** Dar ejemplos claros de vulneración para cada uno (Lectura no autorizada = C, Modificación no autorizada = I, DoS = A).
> - [ ] **Identificar fallos compuestos:** Explicar cómo un incidente real puede violar los 3 pilares simultáneamente.
> - [ ] **Comparar Ley 29733 vs GDPR:** Extraterritorialidad, severidad de sanciones y rol del Oficial de Protección de Datos.
> - [ ] **Dominar Derechos ARCO:** Definición exacta de cada letra y caso de aplicación.
> - [ ] **Sesgo en IA:** Origen en datasets históricos y el caso Amazon 2018.

---

## 🧠 Conceptos Evergreen Conectados
- [[04 Conocimiento/AI & Data Science/Sesgo Algorítmico|Sesgo Algorítmico]]
- [[04 Conocimiento/Arquitectura & Backend/Tríada CIA|Tríada CIA]]
- [[04 Conocimiento/Gestión & Liderazgo/Privacidad y Derechos ARCO|Privacidad y Derechos ARCO]]
- [[04 Conocimiento/Gestión & Liderazgo/GDPR y Ley 29733|GDPR y Ley 29733]]
