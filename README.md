# Agente Evaluador de Prácticas YTA Plata

## Descripción
Este agente está diseñado para apoyar la **formación técnica automotriz**, evaluando prácticas de diagnóstico de averías mecánicas según la metodología del programa **YTA Plata**.  
Su objetivo es analizar paso a paso el desarrollo de un ejercicio realizado por un estudiante o técnico, asignar calificaciones basadas en una **rúbrica estandarizada** y generar recomendaciones de mejora.

## Funcionalidades principales
- **Lectura de documentos**: Procesa archivos en formatos Word, PDF, Excel o texto que contengan el desarrollo de la práctica.  
- **Identificación de pasos**: Reconoce la información de los **11 pasos del procedimiento YTA Plata** (desde la consulta con el cliente hasta la explicación final).  
- **Evaluación detallada**: Califica cada paso según criterios de desempeño: **Excelente, Adecuado o Insuficiente**.  
- **Justificación**: Explica de manera breve la razón de cada calificación.  
- **Puntuación global**: Calcula un promedio estimado en escala numérica o porcentual.  
- **Retroalimentación**: Propone mejoras específicas para los pasos con desempeño inferior a lo esperado.  

## Flujo de trabajo
1. El usuario carga un archivo con la práctica desarrollada.  
2. El agente extrae la información correspondiente a cada uno de los 11 pasos.  
3. Se realiza la evaluación paso a paso siguiendo la rúbrica.  
4. Se genera un **informe estructurado en Markdown** con:  
   - Resumen general.  
   - Evaluación por paso.  
   - Recomendaciones generales.  

## Formato de salida esperado
El informe de evaluación sigue esta estructura:

```markdown
### Evaluación de práctica YTA Plata
**Nombre del estudiante:** [Nombre]

**Resumen general:**
- Pasos evaluados: 11
- Nivel general: [Ejemplo: Mayormente Adecuado]
- Puntuación estimada: [Ejemplo: 8.2 / 10]

#### Paso 1 – Consulta con el cliente
- Qué sucedió: ...
- Quién intervino: ...
- Cuándo ocurrió: ...
- Resultado global del paso: ...
- Recomendación: ...


Rúbrica de referencia

La evaluación se basa en una rúbrica que clasifica cada paso en tres niveles:

Excelente: Cumple completamente los criterios, con justificación y detalle.

Adecuado: Cumple parcialmente, con información incompleta.

Insuficiente: No cumple o no está diligenciado.

Casos especiales

Si un paso no aparece en el documento, se marca como “No diligenciado” y se califica como Insuficiente.

El agente no inventa ni rellena información: solo evalúa lo que el estudiante escribió.

En caso de ambigüedad en el lenguaje, se da el beneficio de la duda únicamente si hay evidencia.

Recomendaciones de uso

Proporcionar documentos completos y organizados.

Usar lenguaje técnico claro en cada paso.

Incluir registros fotográficos o mediciones cuando corresponda.

Verificar que cada conclusión esté respaldada por evidencias.

Licencia

Este proyecto puede usarse con fines académicos y de formación técnica.
