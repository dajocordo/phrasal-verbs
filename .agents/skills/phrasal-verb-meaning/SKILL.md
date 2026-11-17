---
name: phrasal-verb-meaning
description: >-
  Explica el significado de un phrasal verb en inglés con su traducción al español y ejemplos prácticos, en el chat o en un archivo Markdown. Usa esta skill cuando el usuario pregunte qué significa un phrasal verb, pida documentarlo en un archivo `.md` o invoque `/phrasal-verb-meaning`.
---

# Significado de Phrasal Verbs

Obtiene y estructura el significado en inglés y la traducción al español de cualquier phrasal verb, ya sea en el chat o dentro de un archivo Markdown del proyecto.

## Cuándo usar
- El usuario pregunta por el significado o traducción de un phrasal verb (ej. *"what does run out of mean"*, *"significado de look forward to"*).
- El usuario tiene abierto o menciona un archivo `<phrasal_verb>.md` vacío o incompleto y pide rellenarlo.
- El usuario invoca `/phrasal-verb-meaning` seguido de un verbo compuesto en inglés.

## Cuándo NO usar
- Para traducir textos largos, artículos completos o párrafos sin foco en un phrasal verb concreto.
- Para explicar tiempos verbales generales, reglas gramaticales amplias o vocabulario que no sea un phrasal verb.

## Instrucciones
1. Identifica el phrasal verb solicitado por el usuario (por su mensaje o por el nombre del archivo activo, convirtiendo guiones bajos como `run_out_of.md` a `run out of`).
2. Si el phrasal verb tiene más de una acepción de uso frecuente (más de 1 significado común), enumera cada acepción por separado, ordenadas de la más común a la menos común.
3. Para cada acepción, redacta:
   - **Significado en inglés:** definición clara y directa en una frase.
   - **Traducción al español:** equivalentes naturales en español.
   - **Ejemplos:** 2 oraciones cortas en inglés con su traducción al español entre paréntesis.
4. Determina dónde entregar el resultado:
   - Si el usuario pide guardar en archivo o tiene activo un archivo `.md` con el nombre del phrasal verb (ej. `run_out_of.md`) y está vacío, escribe el contenido en dicho archivo usando formato `<verbo_con_guiones_bajos>.md`.
   - Si solo hace una consulta rápida en el chat sin mencionar ni tener abierto un archivo destino, responde directamente en el chat siguiendo la misma estructura.

## Formato de respuesta

```markdown
# <Phrasal Verb>

## 1. <Traducción principal al español>
- **Meaning:** <Definición breve en inglés>
- **Spanish:** <Traducciones equivalentes en español>
- **Examples:**
  - *"<Oración de ejemplo 1 en inglés>"* (<Traducción 1 al español>)
  - *"<Oración de ejemplo 2 en inglés>"* (<Traducción 2 al español>)
```

## Ejemplo
Entrada: `/phrasal-verb-meaning run out of` (con `run_out_of.md` abierto)

Salida (escrita en `run_out_of.md`):
```markdown
# Run out of

## 1. Quedarse sin / Agotarse
- **Meaning:** To use all of something so that there is none left.
- **Spanish:** Quedarse sin, agotarse, acabarse.
- **Examples:**
  - *"We ran out of milk this morning."* (Nos quedamos sin leche esta mañana.)
  - *"I'm running out of patience."* (Se me está agotando la paciencia.)
```
