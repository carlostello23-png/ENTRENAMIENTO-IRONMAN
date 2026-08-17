---
name: planificar-semana
description: Planifica la próxima semana de entrenamiento día por día, a partir de datos reales y la fase actual del plan. Úsala cuando el atleta pida planear la semana, la próxima semana, qué toca esta semana, armar el calendario, "planifica", "qué hago esta semana", "pásame la semana", o cuando empiece una semana nueva.
---

# Planificar la semana

Genera el archivo de la semana siguiente en `entrenamiento/YYYY-MM-DD-semana.md`
(fecha del **lunes**).

## Antes de escribir nada

1. `perfil-atleta.md` — quién es, qué tiene, qué zonas hay (hoy: ninguna medida)
2. `entrenamiento/restricciones.md` — **manda sobre el plan**
3. `entrenamiento/plan.md` — fase actual y horas objetivo de esa semana
4. El archivo de la semana **anterior** — qué se planificó
5. **Garmin Connect** — qué se hizo **de verdad**
6. La última revisión en `revisiones/`

**No se planifica sobre lo planificado. Se planifica sobre lo ejecutado.**
Si la semana pasada se cumplió al 60 %, la siguiente no sube un 10 % sobre el
plan: sube sobre lo real.

## Restricciones que no se negocian

- **Entre semana: máximo 60 min por sesión**, desplazamiento incluido.
- **Sesiones largas y ladrillos: solo sábado y domingo.** Es donde caben.
- **Rutas de bici en exterior: solo fin de semana.** Entre semana, **rodillo**.
- **Techo semanal ~11 h** (5 h entre semana + fin de semana).
- Sesión larga por encima de **3,5 h**: preguntar antes.

## Progresión — por disciplina, nunca sobre el total

| | Límite |
|---|---|
| **Carrera** | **+10 % de tiempo semanal máx.** Tirada larga: **+10 min/semana máx.**, nunca dos semanas grandes seguidas. Techo ~1 h 45. |
| **Bici** | +15 % semanal máx. |
| **Natación** | Flexible. Punto fuerte: mantener, no maximizar. |
| **Fuerza** | 2 sesiones/semana estables. |

Partiendo de base cero, **cualquier porcentaje contra una historia vacía es
aritmética, no fisiología**. Se razona en minutos absolutos, no en ratios.

## Trabajo de calidad: bloqueado hasta el test

**No se prescriben series por zonas de pulso hasta que el test de campo esté
hecho** (`salud/protocolos/test-campo.md`, semana 3). Sin umbral medido son
adivinanzas con aspecto de ciencia.

Hasta entonces: **RPE y regla de conversación.**

## Cómo se prescribe cada deporte

- **Bici:** en **tiempo + RPE**. **Nunca en vatios** (no hay potenciómetro) y
  **nunca en distancia** (viento, desnivel y tráfico la hacen incomparable; en
  rodillo la distancia es un número inventado).
- **Carrera:** en tiempo o distancia + RPE. Pulso continuo sirve como
  referencia; en series cortas manda el RPE (el óptico va con retraso).
- **Natación:** en metros + ritmo/100 m. **El pulso no se usa.**
- **Fuerza:** ejercicios, series, repeticiones. Sin historia de pulso.

## Prioridades de este bloque

1. **Consistencia sobre todo.** El intento anterior falló por no entrenar. Un
   plan aburrido que se cumple gana a uno brillante que se abandona. Si hay
   duda entre ambicioso y cumplible, **cumplible**.
2. **La carrera a pie decide el resultado** — y es donde se puede lesionar.
   Prioridad alta, progresión lenta. No hay contradicción: frecuencia antes que
   duración.
3. **La bici es ~50 % del tiempo de carrera** — el mayor retorno por hora.
4. **La natación es el punto fuerte y el segmento más corto.** Mantener. No
   invertir horas ahí buscando minutos que no llegan.
5. **Desde la semana 9, la aclimatación al calor entra en el calendario** como
   sesiones reales, no como nota (`salud/protocolos/aclimatacion-calor.md`).

## Formato del archivo

```
# Semana N · fechas
**Fase:** · **Objetivo:** X h · **Días a la carrera al cerrar:** N

## El trabajo de esta semana
(qué se busca y por qué — 2-3 frases)

## La semana
| Día | Sesión | Tiempo | Cómo |

## Reglas de la semana
## Registro real  (tabla vacía: planificado vs real, se rellena al cerrar)
```

**Nunca se edita lo planificado a posteriori.** El registro real se añade
aparte — así se ve la diferencia entre intención y ejecución, que es el dato
más útil de todo el proyecto.

## Al terminar

Decir en una línea qué cambió respecto a la semana anterior y por qué.
Si la semana pasada se incumplió, **decirlo con el número** antes de proponer
la nueva.
