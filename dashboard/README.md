# Dashboard

## ⚠️ EL CONTENIDO ESTÁ HORNEADO EN LA PÁGINA

**`index.html` no lee datos de ningún sitio.** Todos los números —el veredicto,
la brecha, la tabla de la semana, la evidencia— están escritos literalmente
dentro del HTML.

**Editar `perfil-atleta.md`, `plan.md` o el archivo de la semana NO cambia el
dashboard.** Hay que reescribir el HTML.

Esto está escrito así de fuerte a propósito: buscar durante una hora por qué un
cambio no aparece es exactamente el rato perdido que este aviso existe para
evitar.

## Cuándo regenerarlo

- **Después de cada revisión semanal** (obligatorio)
- Después del test de campo (cambian las zonas y posiblemente el objetivo)
- Cuando cambie la fase del plan
- Cuando cambie el veredicto del día

**Un dashboard que muestra el veredicto de ayer es peor que no tener ninguno,
porque parece actual.** Por eso la página lleva un aviso de caducidad visible
arriba con la fecha de generación: si no es la de hoy, lo que se ve está viejo.

## La regla de diseño

> **Es una superficie de decisión, no un espejo de métricas.**

La app de salud del móvil ya pinta HRV, pulso en reposo y sueño mejor de lo que
se puede hacer aquí — en vivo y en el bolsillo. Si el dashboard abre con esos
gráficos, pierde, y se deja de abrir.

Por eso el orden es:

1. **El veredicto** — qué hacer hoy y por qué
2. **La brecha** — sesión más larga por disciplina contra la distancia de
   carrera. Es el panel más valioso de la página y ninguna app de consumo lo
   puede saber
3. **Esta semana** — planificado contra real, reconciliado con datos de Garmin
4. **La evidencia** — todas las métricas, **debajo** del veredicto
5. **El razonamiento** — por qué la llamada actual es la que es

Las métricas nunca van arriba. Son evidencia de una decisión, no el producto.

## Detalles técnicos

- **HTML autocontenido**, sin CDN, sin dependencias externas. Se abre con doble
  clic desde cualquier sitio, también sin internet.
- **Adaptable a móvil y escritorio.** Un solo archivo en vez de dos versiones:
  dos archivos que hay que mantener sincronizados acaban divergiendo, y una
  versión de móvil desactualizada es justo el fallo silencioso que el sistema
  intenta evitar. El punto de corte está en 560 px.
- **Se adapta al tema claro/oscuro** del dispositivo, y respeta un
  `data-theme` explícito si se estampa en la raíz.
- **Paleta validada** para daltonismo (deutan/tritan) y contraste, en los dos
  temas. Natación = azul, bici = naranja, carrera = aguamarina, en ese orden
  fijo. **El color no cambia según el orden ni el ranking** — sigue a la
  disciplina.
- Las barras de la brecha llevan **siempre etiqueta numérica visible**: el
  color nunca es el único canal que transmite el dato.

## Cómo se abre

```
open dashboard/index.html          # macOS
xdg-open dashboard/index.html      # Linux
start dashboard\index.html         # Windows
```

## Pendiente

- [ ] Conectar con datos reales de Garmin Connect para que "Real" se rellene solo
- [ ] Generar el HTML desde un script en vez de escribirlo a mano
- [ ] Que la revisión semanal dispare la regeneración automáticamente
