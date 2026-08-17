---
name: chequeo-recuperacion
description: Chequeo diario de recuperación y disponibilidad para entrenar. Úsala cuando el atleta pregunte cómo amaneció, si está recuperado, si puede entrenar hoy, si debe descansar, cómo va su pulso en reposo o su HRV, si está cansado o sobreentrenado, o diga cosas como "¿entreno hoy?", "¿cómo voy?", "amanecí cansado", "¿estoy recuperado?", "chequeo", "readiness".
---

# Chequeo de recuperación

Decide **qué hacer hoy** y lo justifica con números. No es un espejo de
métricas: es una decisión.

## Antes de nada

Leer `perfil-atleta.md` y `entrenamiento/restricciones.md`.
Las reglas generales de entrenador están en `CLAUDE.md` — no se repiten aquí.

## Qué se mira

Fuente: **Garmin Connect** (única fuente de bienestar del proyecto).

1. **FC en reposo** — contra **su propia** línea base de 7 días
2. **HRV** — contra media móvil de 7 días, banda normal ±0,5 SD (protocolo
   Kiviniemi)
3. **Sueño** — duración y continuidad
4. **Carga de los últimos 7 días** y qué toca hoy según el archivo de la semana
   en `entrenamiento/`
5. **Lo que dijo el atleta** — si hay relato subjetivo, **manda sobre los
   datos**

## ⚠️ Antes del 31 de agosto de 2026 — sin línea base

Hacen falta **~14 días continuos** de datos Garmin para tener línea base de FC
en reposo y HRV. Antes de eso **no hay contra qué comparar**.

Si aún no hay línea base, **decirlo así de claro** y no fabricar un veredicto:
*"Llevas X días de datos. Sin línea base no puedo llamar nada anormal — el
número de hoy no significa nada por sí solo. Sigue el plan."*

**No inventar un veredicto de recuperación sobre datos insuficientes.**

## Cómo se decide

**Nunca alarmar por una métrica suelta.** El sobreentrenamiento se diagnostica
por **convergencia** (Meeusen et al., 2013, consenso ECSS/ACSM). Un marcador
fuera de rango es ruido.

| Situación | Decisión |
|---|---|
| Todo dentro de banda | **Entrena lo planificado.** Una línea y ya. |
| **Un** marcador fuera | Entrena lo planificado. Se menciona, no se cambia nada. |
| **Dos o más** convergen (FC reposo alta + HRV baja + sueño malo + sensación mala) | **Se recorta o se descansa.** Con los números delante. |
| Dolor articular o tendinoso | **Se corta la carrera a pie**, no todo. Se nada y se pedalea igual. |
| Síntomas de enfermedad | No se entrena. Sin discusión. |

**Tendencia, no una mañana.** Especialmente el HRV: tanto subidas como bajadas
se han asociado a adaptación negativa (Plews et al.). Tres días de deriva dicen
algo; un martes no dice nada.

## Formato de salida

**Día normal = una línea.** La longitud sigue a lo que hay que decir.

> Todo en banda (FC reposo 54, base 53–56). Rodillo 40' como estaba.

**Día con bandera = el número, la convergencia, la decisión:**

> FC reposo 61 — cinco por encima de tu base (53–56), tercer día seguido.
> HRV por debajo de la banda. Dormiste 5h20.
> Tres señales convergiendo, no una. Hoy: descanso o 30' muy suave. No la
> tirada larga.

**Nunca:** "te veo cansado", "buen trabajo", "escucha a tu cuerpo".
**Siempre:** el número, su línea base, cuántos días lleva.

## Contexto específico de este atleta

- **Base cero desde el 17 ago 2026.** Las primeras semanas van a mostrar fatiga
  de reactivación, que es **normal y esperada**, no una alarma. No confundirla
  con sobrecarga.
- **El ACWR no significa nada hasta ~la semana 6** — la ventana crónica está
  llena de ceros (Impellizzeri et al., 2020, acoplamiento matemático). Si se
  menciona, se dice que es artefacto.
- **La carrera a pie es la disciplina de riesgo.** Cualquier molestia ahí se
  toma en serio antes que en las otras dos.
- **Pulso óptico de muñeca.** Fiable en reposo y en continuo. Si un dato de
  sesión parece imposible, probablemente lo sea — se dice, no se interpreta.
