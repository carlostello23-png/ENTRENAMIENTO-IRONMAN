---
name: revision-semanal
description: Revisión de la semana cerrada — planificado contra real, sensación contra datos. Úsala cuando el atleta pida revisar la semana, cerrar la semana, cómo fue la semana, el resumen semanal, "revisión", "cómo voy", "balance de la semana", o al terminar un domingo.
---

# Revisión semanal

Compara **lo planificado contra lo ejecutado** y saca una conclusión utilizable.

## Regla dura

**Se AÑADE a `revisiones/`. Nunca se sobrescribe una semana pasada.**
Archivo: `revisiones/YYYY-MM-DD-semana-N.md` (fecha del lunes).
Las correcciones son aditivas: se marca `SUPERSEDED`, no se borra.

## Antes de escribir

1. El archivo de la semana en `entrenamiento/`
2. **Garmin Connect** — sesiones reales de los 7 días
3. `entrenamiento/plan.md` — fase y objetivo de horas
4. La revisión anterior
5. Lo que cuente el atleta sobre cómo se sintió

## Verificación de datos — hazla antes de contar nada

**El fallo silencioso es el enemigo.** Comprobar que los datos **están**, no que
la consulta corrió:

- ¿Cada sesión trae duración, distancia y pulso poblados, o hay registros vacíos?
- ¿Alguna sesión duplicada (misma hora, dos registros)? Se queda la que tenga
  carga real, se excluye la otra y **se anota cuál y por qué**.
- ¿Alguna actividad que no sea nadar/pedalear/correr/fuerza? **El
  entrenamiento cruzado se cae de los filtros y se convierte en carga cero.**
  Cazarla a mano.
- Si faltan datos, **se dice "faltan datos"**. No se estima el hueco.

## La métrica que manda

> **Consistencia = sesiones completadas / sesiones planificadas.**

El intento anterior falló por falta de entrenamiento. Esta es la cifra que
predice el resultado de noviembre, por encima de cualquier otra. **Va primero
en la revisión, siempre.**

## Estructura

```markdown
# Revisión — Semana N · fechas

## Consistencia
X / Y sesiones · Z h de las W planificadas

## Planificado vs real
| Día | Planificado | Real | ✓/✗ |

## Por disciplina
| | Planificado | Real | Δ |
(natación / bici / carrera / fuerza, en minutos)

## La brecha
| | Más larga hasta hoy | Carrera | Falta |
(natación 1,9 km · bici 90 km · carrera 21,1 km)

## Qué progresó
## Qué no progresó
## Sensación vs datos
## La semana que viene
```

## Cómo se escribe

- **Nunca adular.** Si no progresó nada, se dice. Un archivo que solo dice
  "buen trabajo" no vale nada.
- **El número, no la sensación.** "3 de 6 sesiones, 2h10 de 4h" es una
  revisión. "Semana floja" no lo es.
- **Si el relato del atleta choca con lo que infieren los datos, gana él.** Él
  estuvo ahí. Se dice explícitamente que se descarta la inferencia — no se
  reconcilian las dos versiones en silencio.
- **Si se perdieron semanas, se recalibra el objetivo con honestidad.** 15
  semanas desde cero no tienen margen. Perder dos cambia lo que es alcanzable,
  y disimularlo es peor que decirlo.

## Puntos de control del calendario

| Semana | Qué toca |
|---|---|
| **3** (31 ago–6 sep) | **Test de campo.** Se registran zonas en `perfil-atleta.md` y **se decide si el 6:30 sigue en pie** |
| **7, 11** | Semanas de descarga — verificar que se descargó de verdad |
| **8, 12** | Repetición del test |
| **9** | Arranca la aclimatación al calor |
| **13** | Pico de volumen. A partir de aquí solo se baja |

## Al cerrar

- Actualizar **La brecha** con datos reales.
- Si algo falló de forma sistémica (una skill que no cargó, datos que no
  llegaron, un filtro que se comió sesiones), **añadirlo a "Cosas que nos han
  mordido" en `CLAUDE.md`**. Esa sección es lo más valioso del proyecto a los
  seis meses.
- Regenerar el dashboard.
