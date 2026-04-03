# Protocolo de Aplicación de Indicadores

## Propósito

Este documento explica **cómo se usa cada indicador sobre un corpus**. No es teoría: es un manual operativo para que la taxonomía sea reproducible, auditable y aplicable a conflictos más allá de Irán 2026.

---

## 1. Unidad de análisis

Cada indicador puede aplicarse a distintas unidades de análisis según el corpus disponible:

| Tipo de unidad | Descripción | Ejemplo | Indicadores más aplicables |
|----------------|-------------|---------|---------------------------|
| **Declaración oficial** | Comunicado, discurso, conferencia de prensa de un actor estatal o institucional | Discurso presidencial, resolución del Consejo de Seguridad, comunicado de la Casa Blanca | 1.1, 1.2, 1.5, 2.1, 2.2, 2.3 |
| **Pieza periodística** | Artículo, crónica, editorial, reportaje de un medio identificable | Artículo de El Mundo, crónica de Times of Israel | 1.2, 1.3, 1.4, 2.5 |
| **Publicación en red social** | Post, hilo, vídeo publicado en X, Telegram, Reddit u otra plataforma | Hilo de "análisis OSINT" en X, vídeo viral de la Casa Blanca | 1.3, 1.4, 3.1, 3.2 |
| **Interfaz/panel** | Dashboard, visualización interactiva, panel de datos | Panel de Liveuamap, interfaz de FlightRadar24 | 3.1, 3.3, 3.4, 3.5 |
| **Mercado de predicción** | Apuesta activa en plataformas como Polymarket o Kalshi | Apuesta sobre alto el fuego en Irán | 2.4 |
| **Evento mediático** | Acontecimiento que genera cobertura masiva y discusión pública | Caso Fabian, publicación de "Justice the American Way" | Todos (como caso de estudio) |

**Regla**: especificar siempre la unidad de análisis antes de aplicar un indicador. Un indicador activado en un hilo de X no tiene el mismo peso que un indicador activado en una resolución del Consejo de Seguridad.

---

## 2. Escala temporal

| Escala | Ventana de observación | Uso principal | Riesgo |
|--------|----------------------|---------------|--------|
| **Micro** | Horas a días | Detección de anomalías puntuales | Alta tasa de falso positivo; eventos aislados no son tendencias |
| **Meso** | Semanas a meses | Detección de patrones emergentes | Balance razonable entre señal y ruido |
| **Macro** | Meses a años | Confirmación de desplazamientos estructurales | Baja tasa de falso positivo, pero detección tardía |

**Regla**: un indicador solo se considera **activado** cuando se detecta de forma sostenida en escala **meso** o se confirma en escala **macro**. Las detecciones en escala micro se registran como **señales débiles**.

---

## 3. Criterios de presencia/ausencia

Para cada indicador aplicado a un corpus:

| Valoración | Criterio |
|------------|---------|
| **Sí** | El indicador se detecta de forma clara, sostenida y documentable con ejemplos múltiples. |
| **Parcial** | El indicador se detecta en algunos registros pero no de forma generalizada, o se detecta una versión atenuada del fenómeno descrito. |
| **No** | El indicador no se detecta en el corpus, o solo se detecta en registros aislados sin patrón reconocible. |

**Regla**: la ausencia de un indicador es tan informativa como su presencia. Documentar siempre los "No" con la misma rigurosidad que los "Sí".

---

## 4. Umbral de intensidad

| Intensidad | Criterio |
|------------|---------|
| **Alta** | El fenómeno es dominante en el corpus: aparece en múltiples tipos de fuente, es reconocible sin búsqueda especializada, afecta a actores principales. |
| **Media** | El fenómeno es detectable pero no dominante: requiere búsqueda activa, aparece en fuentes especializadas o secundarias, afecta a actores intermedios. |
| **Baja** | El fenómeno es marginal: solo detectable con análisis fino, aparece en fuentes minoritarias, no tiene efecto observable en actores principales. |
| **Ausente** | No se detecta ni con análisis fino. |

**Regla**: la intensidad debe calibrarse con el corpus completo, no con ejemplos aislados. Un solo ejemplo espectacular (el vídeo de la Casa Blanca) no determina por sí solo una intensidad "Alta" — necesita estar acompañado de un patrón más amplio.

---

## 5. Evaluación de reversibilidad

Columna añadida a la matriz comparativa. Tres niveles:

| Nivel | Descripción | Criterio | Ejemplo |
|-------|-------------|----------|---------|
| **Reversible** | El desplazamiento puede deshacerse mediante decisión política, regulatoria o de diseño sin cambio estructural. | Basta con que un actor con capacidad de decisión lo revierta. | Incluir metadatos epistémicos en dashboards (3.4). Ralentizar el ciclo declarativo institucional (2.1). |
| **Parcialmente reversible** | El desplazamiento puede atenuarse pero no eliminarse. Requiere esfuerzo sostenido y cambio cultural o institucional. | Necesita intervención de múltiples actores durante tiempo prolongado. | Restaurar la distancia irónica (1.3). Regular mercados de predicción bélicos (2.4). Rehabilitar el subjuntivo geopolítico (1.5). |
| **Estructural** | El desplazamiento refleja un cambio en infraestructura (tecnológica, informativa, cognitiva) que no puede revertirse sin desmantelar la infraestructura misma. | Incluso si el conflicto termina, el desplazamiento persiste. | Democratización de herramientas OSINT (3.1). Inversión de cadena de custodia informativa (2.5). Compresión del ciclo atención-interpretación (3.2). |

**Regla**: la reversibilidad no indica gravedad. Un indicador reversible pero activo puede ser más peligroso a corto plazo que uno estructural que opera lentamente.

---

## 6. Cómo evitar sobrelectura

La sobrelectura es el riesgo principal de cualquier taxonomía de indicadores: ver señales donde no las hay, o atribuir significado sistémico a anomalías puntuales. Protocolos contra la sobrelectura:

### 6.1 Regla de triangulación
Un indicador solo se considera activado si se detecta en **al menos dos tipos de unidad de análisis distintos** (por ejemplo: declaración oficial + cobertura periodística, o publicación en red social + interfaz de panel).

### 6.2 Regla de persistencia
Un indicador solo se confirma si se detecta en **al menos dos momentos distintos dentro de la escala meso** (semanas a meses). Una detección puntual es una señal débil, no un indicador activado.

### 6.3 Regla de falsabilidad
Para cada indicador activado, el analista debe formular explícitamente: **"¿Qué evidencia me haría desactivar este indicador?"** Si no puede formularse esa pregunta, el indicador no está bien aplicado.

### 6.4 Regla de contexto
Un indicador no se evalúa en aislamiento. La activación de un indicador debe contextualizarse con:
- El estado de los demás indicadores del mismo nivel.
- El estado de los indicadores de otros niveles.
- El contexto geopolítico, institucional y tecnológico del momento.

### 6.5 Regla de humildad
Los indicadores no predicen colapso. Detectan desplazamientos en la gramática de lo pensable. Un indicador activado no significa que el orden vaya a cambiar — significa que las condiciones cognitivas para que cambie están presentes. La diferencia es fundamental.

---

## 7. Plantilla de registro

Para cada aplicación de la taxonomía a un corpus, usar esta plantilla:

```
REGISTRO DE APLICACIÓN DE INDICADORES

Corpus: [identificar]
Período: [fecha inicio - fecha fin]
Analista: [nombre]
Fecha de análisis: [fecha]

INDICADOR: [número y nombre]
Unidad de análisis: [tipo]
Escala temporal: [micro/meso/macro]
Presencia: [Sí/Parcial/No]
Intensidad: [Alta/Media/Baja/Ausente]
Reversibilidad: [Reversible/Parcialmente reversible/Estructural]
Evidencia: [descripción concreta, con fuente y fecha]
Riesgo de falso positivo evaluado: [Sí/No — explicar]
Triangulación: [¿Se detecta en otra unidad de análisis?]
Persistencia: [¿Se detecta en otro momento temporal?]
Pregunta de falsabilidad: [¿Qué evidencia lo desactivaría?]
Nivel de confianza: [Hecho confirmado / Señal débil / Narrativa plausible]
Notas: [observaciones adicionales]
```

---

## 8. Aplicabilidad a otros conflictos

Esta taxonomía está diseñada para ser portátil. Los indicadores no son específicos de Irán 2026: detectan patrones de transición de orden que pueden manifestarse en cualquier conflicto. Para aplicarla a un nuevo corpus:

1. **Seleccionar el corpus** con criterios explícitos (período, fuentes, idiomas).
2. **Aplicar los 15 indicadores** usando la plantilla de registro.
3. **Comparar con la matriz existente** (entreguerras + Irán 2026) para identificar patrones recurrentes.
4. **Documentar los indicadores ausentes** tan rigurosamente como los presentes.
5. **Evaluar la reversibilidad** en el nuevo contexto (puede variar).
6. **Publicar los resultados** con la plantilla para que sean reproducibles.

**Conflictos candidatos para aplicación futura:**
- Ucrania 2022-presente (especialmente indicadores de Nivel 3)
- Crisis del Estrecho de Taiwán (si se materializa)
- Pre-WWI (julio 1914) como caso de validación retrospectiva
- Colapso soviético (1989-1991) como caso de transición no bélica

---

*El protocolo no reemplaza el juicio del analista. Lo disciplina.*
