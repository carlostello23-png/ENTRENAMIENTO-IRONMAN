# El sistema — mapa de una página

**IRONMAN 70.3 Cartagena · domingo 29 de noviembre de 2026**
*(mapa actualizado el 17 ago 2026 — mantener verdadero)*

---

## Qué es esto

Un sistema de entrenamiento persistente: archivos que sobreviven entre
sesiones, skills que se lanzan con un comando y un dashboard que dice qué hacer
hoy. No es un plan de entrenamiento en PDF; es una memoria de trabajo que se
va corrigiendo.

## Dónde está cada cosa

| Archivo | Para qué | Cuándo se lee |
|---|---|---|
| **`CLAUDE.md`** | Manual de operación: cómo se trabaja, reglas duras, ruteo de datos, cosas que nos han mordido | Cada sesión, automático |
| **`perfil-atleta.md`** | Quién es el atleta, qué equipo tiene, qué zonas hay | Cada sesión |
| **`sistema.md`** | Este mapa | Cuando uno se pierde |
| **`entrenamiento/plan.md`** | A dónde vamos: 15 semanas, 4 fases, la aritmética del 6:30 | Al planificar |
| **`entrenamiento/restricciones.md`** | Lo que la realidad permite. **Gana sobre `plan.md`** | Al planificar |
| **`entrenamiento/YYYY-MM-DD-semana.md`** | Una semana concreta, día a día | Cada semana |
| **`revisiones/`** | Revisiones semanales. **Solo se añade, nunca se sobrescribe** | Al cerrar semana |
| **`salud/protocolos/`** | Documentos permanentes: test de campo, aclimatación al calor, **molestias sin AINEs** | Cuando toque |
| **`salud/`** | Banderas fechadas, solo en días que merecen bandera | Cuando pase algo |
| **`carreras/`** | Investigación de la carrera y plan de parciales | Fase 3 y logística |
| **`dashboard/`** | La superficie de decisión | A diario |
| **`.claude/skills/`** | Las skills | Automático |
| **`archivo/`** | Trabajo retirado — se guarda, no se borra | Rara vez |

**`plan.md` y `restricciones.md` están separados a propósito.** Uno es a dónde
vamos, el otro es lo que se puede. **Cuando chocan, gana `restricciones.md`.**

## Las skills

| Comando | Qué hace |
|---|---|
| `/chequeo-recuperacion` | ¿Entreno hoy? Con los números delante. Calla si todo es normal |
| `/planificar-semana` | La semana que viene, día a día, desde datos reales |
| `/revision-semanal` | Planificado vs real. Añade a `revisiones/` |
| `/analisis-carrera` | Sesión de correr — ritmo, deriva cardíaca, señales de lesión |
| `/analisis-bici` | Sesión de bici — tiempo y RPE. Sin vatios, no hay potenciómetro |
| `/analisis-natacion` | Sesión de nado — ritmo/100 m, eficiencia. Sin pulso |
| `/analisis-fuerza` | Gimnasio — carga y frecuencia. Sin historia de pulso |

**Están escritas por separado a propósito.** Las métricas de cada deporte son
genuinamente distintas: correr va de ritmo y desacople; la bici sin
potenciómetro va de resistencia a cadencia y pulso igualados, medida en tiempo;
nadar va de ritmo por 100 m con el pulso descartado; la fuerza no tiene historia
de pulso en absoluto. Una skill clonada con buscar-y-reemplazar produce
tonterías dichas con mucha seguridad.

**Lo que aplica a todo el coaching vive en `CLAUDE.md`, no copiado en cada
skill** — si no, se actualiza en seis sitios y se olvidan dos.

## Las restricciones que atraviesan todo

0. **⚠️ ALERGIA A LOS AINEs** → nunca se sugiere un antiinflamatorio ni ningún
   fármaco. Las molestias se gestionan con carga. **Va antes que todo lo demás**
   y está en `CLAUDE.md` por encima de las reglas duras.
1. **Sin potenciómetro** → no existen vatios ni FTP. La bici va en tiempo + RPE.
2. **Sin banda pectoral** → pulso óptico. No fiable en series ni nadando.
3. **Sin zonas medidas** → el trabajo de calidad está **bloqueado** hasta el
   test de campo de la semana 3.
4. **Base cero + 15 semanas** → progresión **por disciplina**, no sobre el
   total. Ninguna semana sobra.
5. **Bogotá 2.640 m → Cartagena nivel del mar, 30 °C, 80 % humedad** → la
   aclimatación al calor es un bloque del plan, no una nota al pie.
6. **1 h al día entre semana; fin de semana libre** → todo lo largo va en fin de
   semana. Techo real ~11 h/semana.
7. **El fallo anterior fue de consistencia** → la métrica que manda es
   sesiones cumplidas / planificadas.

## Calendario de puntos de control

| Semana | Fechas | Qué pasa |
|---|---|---|
| 1–3 | 17 ago – 6 sep | Reactivación. Se acumulan 14 días de datos para tener línea base |
| **3** | 31 ago – 6 sep | **TEST DE CAMPO.** Desbloquea la calidad y **decide si el 6:30 sigue en pie** |
| 4–8 | 7 sep – 11 oct | Base. Descarga en la 7. Retest en la 8 |
| **9** | 12 oct | **Arranca la aclimatación al calor** |
| 9–13 | 12 oct – 15 nov | Específico. Descarga en la 11. Retest en la 12. **Pico en la 13** |
| 14–15 | 16 – 29 nov | Taper. Se mantiene el calor hasta el final |
| **15** | **29 nov** | **CARRERA** |

## Estado actual

*(17 ago 2026)*

- **Semana 1 de 15.** Fase: reactivación. 104 días a la carrera.
- **Base cero.** No entrenaba al arrancar.
- **Sin línea base** de FC en reposo ni HRV — hacen falta ~14 días de Garmin.
- **Sin zonas medidas.** Calidad bloqueada.
- **Sin conexión automática a Garmin.** Los datos entran a mano y el dashboard
  se escribe a mano.

## Huecos abiertos

Se dicen desconocidos, no se rellenan con números plausibles.

- 🔴 **La inscripción de Cartagena NO está hecha.** Lo más urgente del proyecto:
  entrenando para una carrera sin plaza reservada.
- **Tiempo y parciales del 70.3 que ya completó** — el dato más valioso que
  falta. Un tiempo real de 70.3, aunque saliera mal, calibra el 6:30 mejor que
  cualquier test.
- **Talla** — sin ella los 87 kg no se pueden interpretar.
- Historial de lesiones, otras condiciones crónicas, otras alergias, medicación
- **Qué tipo de reacción provocan los AINEs** *(pregunta para su médico)*
- Año del modelo de la Émonda; **si lleva acoples** *(minutos sobre la mesa en
  90 km llanos)*; tipo de rodillo
- Horarios de la piscina, franja de entrenamiento entre semana
- Techo real de horas en fin de semana

**Resueltos el 17 ago 2026:** edad (35), peso (87 kg), bici (Trek Émonda SL ·
105), rodillo (sí), aguas abiertas (sí, varias veces), chequeo diario (sí),
alergia a AINEs (registrada como regla de seguridad).

## Lo siguiente

1. 🔴 **Hacer la inscripción de Cartagena.** Esta semana.
2. ✅ *Hecho — las siete skills cargan correctamente (verificado el 17 ago 2026).*
3. Llevar el Garmin también para dormir — el reloj de los 14 días de línea base
   corre desde ya
4. Recuperar el tiempo y los parciales del 70.3 anterior
5. Cerrar los huecos de salud que quedan antes de escribir reglas automáticas
6. **Automatización** (chequeo diario + revisión semanal en `cron`) — **aún no
   construida.** El atleta pidió chequeo diario, así que esto sube de prioridad.
7. **Conexión con Garmin Connect** — **aún no construida.** Hoy los datos entran
   a mano y el dashboard se escribe a mano.
