# Protocolo — Test de campo

**Documento permanente.** Se ejecuta en la semana 3 (31 ago – 6 sep 2026) y se
repite en la semana 8 y en la 12.

---

## Por qué existe

Hoy **no hay ninguna zona medida**. Sin umbral real, prescribir series por zonas
de pulso son adivinanzas con aspecto de ciencia. Por eso **todo el trabajo de
calidad está bloqueado hasta que este test se haga de verdad**.

Además este test es el **punto de control del objetivo de 6:30**. La aritmética
está en `entrenamiento/plan.md` §1: el 6:30 exige correr ~7:24/km al final de la
carrera, con calor y humedad. Este test nos dice si eso está a distancia
razonable o no.

## Antes de hacerlo

- **Dos días fáciles antes.** Un test sobre piernas cansadas mide tu fatiga, no
  tu umbral.
- No lo hagas si has dormido mal dos noches seguidas o si el chequeo de
  recuperación marcó bandera. Se aplaza, no se fuerza.
- **Mismo sitio y mismas condiciones cada vez que se repita.** En Bogotá, a
  2.640 m, un test en una ruta distinta no es comparable.
- Anota temperatura y hora del día. Van al registro.

---

## Test 1 — Carrera (el que más importa)

**Formato: 30 minutos contrarreloj, en solitario, terreno llano.**

1. Calentamiento 15 min muy suave + 4 aceleraciones de 20 s.
2. **30 minutos al máximo esfuerzo que puedas sostener de forma constante.**
   No es un sprint. Si el último tramo es un desastre, saliste muy fuerte.
3. Vuelta a la calma 10 min.

**Qué sacamos:**

| Dato | Cómo se obtiene |
|---|---|
| **LTHR de carrera** | **Pulso medio de los últimos 20 minutos** (no de los 30) |
| **Ritmo umbral** | Ritmo medio de los 30 minutos |

*(Protocolo de Friel. Es una estimación de campo decente del umbral de lactato,
no una medida de laboratorio. Se usa como referencia de trabajo, no como
verdad absoluta.)*

**Cómo se lee el resultado, sin adornos:**

- **~6:00 /km o mejor** → el 6:30 sigue vivo. El plan apunta ahí.
- **6:00–6:40 /km** → 6:30 es improbable. Banda realista 6:45–7:10. Lo digo en
  la revisión de esa semana y recalibramos el objetivo con el número delante.
- **Peor de 6:40 /km** → el objetivo pasa a ser terminar bien y correr el medio
  maratón entero sin caminar. Sigue siendo un objetivo perfectamente digno, y
  es el que sostienen los datos.

**Nota sobre la altitud:** esto se mide a 2.640 m. En Cartagena, a nivel del
mar, el mismo esfuerzo dará un ritmo algo mejor. Es una ventaja real pero
modesta, y **no compensa** la pérdida por calor y humedad. No se usa para
inflar la previsión.

---

## Test 2 — Bici

**Formato: 20 minutos contrarreloj, en rodillo** (el rodillo elimina viento,
tráfico y semáforos: es el único sitio donde dos tests son comparables).

1. Calentamiento 15 min + 3× 1 min fuerte / 1 min suave.
2. **20 minutos al máximo esfuerzo sostenible constante.**
3. Vuelta a la calma 10 min.

**Qué sacamos:**

| Dato | Cómo se obtiene |
|---|---|
| **LTHR de bici** | Pulso medio de los 20 minutos, **×0,95** |
| Referencia de esfuerzo | RPE y sensación a esa intensidad |

**Qué NO sacamos: FTP.** No hay potenciómetro. Si el rodillo o Garmin muestran
una potencia estimada, **es una estimación y no se registra como dato**. La
bici de este proyecto se prescribe en **tiempo + RPE + pulso**.

**Importante:** el LTHR de bici es normalmente **5–10 pulsaciones más bajo** que
el de carrera. Son dos números distintos y no se mezclan.

---

## Test 3 — Natación

**Formato: 1.000 m contrarreloj en piscina**, salida desde el borde, sin
material.

1. Calentamiento 400 m suave + 4×50 progresivos.
2. **1.000 m al máximo esfuerzo sostenible constante.**
3. Vuelta a la calma 200 m.

**Qué sacamos:**

| Dato | Cómo se obtiene |
|---|---|
| **T-pace (ritmo umbral)** | Tiempo total ÷ 10 = ritmo por 100 m |

**El pulso en natación no se registra para nada.** El óptico de muñeca no es
fiable bajo el agua. Aquí manda el reloj de pared y la sensación.

**Nota de altitud:** nadar a 2.640 m es más duro que a nivel del mar. Si el
ritmo parece lento comparado con lo que recuerdas, probablemente sea la altura.
En Cartagena irá mejor. No cundir el pánico.

---

## Después del test

1. Escribir los números en `perfil-atleta.md` §Zonas, **con fecha**, cambiando
   el estado de `SIN MEDIR` a medido.
2. Si hay un valor previo, **conservarlo marcado `SUPERSEDED`** — no se borra.
3. Anotar condiciones: temperatura, hora, sitio, cómo se sintió.
4. **Recalibrar el objetivo** en la revisión de la semana según la tabla de
   lectura de arriba. Con el número delante, sin disimular.

## Cuándo se repite

| Cuándo | Para qué |
|---|---|
| **Semana 3** (31 ago–6 sep) | Línea base. Desbloquea el trabajo de calidad. |
| **Semana 8** (5–11 oct) | ¿Está funcionando la fase base? |
| **Semana 12** (2–8 nov) | Ajuste final de ritmos de carrera. Último punto donde el objetivo se puede recalibrar con tiempo. |
