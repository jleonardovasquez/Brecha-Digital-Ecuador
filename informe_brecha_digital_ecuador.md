# Brecha digital en Ecuador: análisis exploratorio con datos del INEC (2022-2025)

**Autor:** [Tu nombre]
**Fuente de datos:** Encuesta ENEMDU-TIC, Instituto Nacional de Estadística y Censos (INEC), Ecuador
**Periodo analizado:** julio 2022 - julio 2025
**Herramientas:** Python, pandas (Google Colab)

## Introducción

Este análisis exploratorio busca responder una pregunta central: **¿cómo se relaciona el acceso y uso de herramientas digitales con distintos grupos de la población ecuatoriana?** Se examinaron tres dimensiones principales: zona geográfica (urbana/rural), grupo étnico, y tipo de uso (comunicación, trabajo, educación, entretenimiento).

## Metodología

Se trabajó con los archivos tabulados públicos del INEC correspondientes a la encuesta TIC de julio 2022 a julio 2025, procesados con Python y la librería pandas. Se limpiaron los datos (corrección de separadores, codificación de texto, formato numérico) antes del análisis.

## Hallazgos principales

### 1. Brecha digital urbano-rural: se reduce, pero persiste

El porcentaje de personas que usan internet, dentro de cada zona:

| Año | Zona urbana | Zona rural | Brecha (puntos) |
|-----|------------|------------|------------------|
| 2022 | 78.5% | 50.5% | 28.0 |
| 2023 | 81.1% | 54.5% | 26.6 |
| 2024 | 85.1% | 59.8% | 25.3 |
| 2025 | 85.3% | 68.5% | 16.8 |

La zona rural creció mucho más rápido (+18 puntos) que la urbana (+6.8 puntos), que ya se acerca a un techo natural. La brecha se está achicando, pero en 2025 seguía siendo de casi 17 puntos porcentuales.

### 2. Brecha étnica: más amplia y más persistente que la geográfica

Porcentaje de personas que usan internet, por grupo étnico:

| Año | Indígena | Afroecuatoriano | Montubio | Mestizo |
|-----|----------|------------------|----------|---------|
| 2022 | 40.2% | 71.5% | 53.2% | 74.8% |
| 2023 | 40.0% | 74.7% | 60.5% | 78.3% |
| 2024 | 49.7% | 82.5% | 68.0% | 81.8% |
| 2025 | 57.3% | 82.4% | 73.8% | 83.6% |

La población indígena parte del nivel más bajo (40.2% en 2022) y, aunque crece con fuerza, sigue teniendo la brecha más amplia frente a la población mestiza (26.3 puntos en 2025). El analfabetismo digital en la población indígena bajó de 31.0% (2022) a 10.0% (2025), una mejora notable pero que arrancó desde un nivel muy alto.

### 3. Para qué se usa internet (nivel nacional)

Entre las personas que ya usan internet, distribución por actividad principal:

| Actividad | 2022 | 2023 | 2024 | 2025 |
|-----------|------|------|------|------|
| Comunicación y redes sociales | 73.3% | 79.2% | 79.9% | 76.8% |
| Educación y aprendizaje | 12.3% | 7.7% | 5.3% | 6.9% |
| Entretenimiento | 9.2% | 9.6% | 11.8% | 13.0% |
| Trabajo | 2.9% | 1.8% | 1.7% | 1.9% |

Llama la atención la caída sostenida del uso educativo (12.3% → 6.9%) frente al aumento del entretenimiento (9.2% → 13.0%) — un patrón que valdría la pena investigar con más profundidad.

## Limitaciones

Los datos tabulados públicos del INEC no permiten cruzar más de una variable a la vez (por ejemplo, no es posible saber qué actividad de uso predomina *dentro* de la población indígena, o por rango de edad). Para responder ese tipo de preguntas se requeriría trabajar con los microdatos (base de datos individual) de la encuesta ENEMDU-TIC.

## Preguntas abiertas para profundizar

- ¿Cómo varía el uso por rango de edad?
- ¿La actividad de uso (trabajo, educación) varía según etnia o nivel educativo?
- ¿Qué factores explican la caída del equipamiento tecnológico del hogar desde 2022?

## Conclusión

Ecuador muestra una reducción sostenida de la brecha digital urbano-rural entre 2022 y 2025, pero la brecha étnica —particularmente para la población indígena— sigue siendo más amplia y requiere atención específica en política pública. El uso de internet sigue concentrado en comunicación y entretenimiento, con una participación baja y decreciente en fines educativos y laborales.
