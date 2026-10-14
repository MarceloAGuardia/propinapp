# Propinapp

Propinapp es una app web para repartir las propinas de un salón entre el equipo, de forma clara y justa. Cada día se carga la propina y quién trabajó en cada turno. La app va sumando todo en un pozo y, al cierre del período, calcula cuánto le toca a cada persona.

**[Ver la demo →](https://marceloaguardia.github.io/propinapp/)**

> En la demo, tocá **«Cargar datos de ejemplo»** para verla funcionando con un equipo y un mes de propinas inventados.

---

## El problema que resuelve

En muchos salones las propinas se juntan en un pozo común y se reparten cada tanto. Hacerlo a mano en un cuaderno o en una planilla trae siempre las mismas dudas:

- ¿Cuánto se juntó hasta hoy?
- ¿Cuántos turnos hizo cada persona?
- ¿Cuánto le toca a quien trabajó solo la mañana?
- ¿Qué días tuvo franco cada uno?

Propinapp responde todo eso de un vistazo, día a día, y con el mismo criterio para todo el equipo.

## Qué hace

- **Período de reparto a elección:** por día, por semana (de lunes a domingo), por quincena (1–15 y 16–fin de mes), por mes, o cada tantos días desde una fecha que elijas.
- **Pozo acumulado:** las propinas de cada día se van sumando hasta el cierre del período. Se puede ver cómo creció el pozo día por día.
- **Dos formas de dividir el pozo:**
  - **Según turnos:** cada turno trabajado (Mañana o Noche) vale una parte. Quien hizo un solo turno cobra la mitad que quien hizo los dos.
  - **Partes iguales:** cada día trabajado vale una parte, sin importar cuántos turnos se hicieron ese día.
- **Plantel:** se pueden agregar personas, darlas de baja conservando su historial, reincorporarlas o eliminarlas.
- **Liquidación por persona:** turnos de mañana y de noche, días trabajados, días sin trabajar y el monto que le corresponde a cada persona. Mientras el período está en curso, el monto se muestra como parcial.
- **Detalle de francos:** al pasar el cursor (o tocar, en el celular) sobre los días sin trabajar, aparece qué días no trabajó la persona y en qué días hizo un solo turno.
- **Acceso rápido por día:** la barra del período muestra cada día con su estado (con propina, sin propina, por venir). Tocando un día se abre su registro.
- **Funciona en el celular** y se adapta al modo claro u oscuro del dispositivo.

## Cómo se calcula el reparto

Un ejemplo con el modo **Según turnos**, en una quincena donde entraron **$90.000**:

| Persona | Turnos en la quincena | Parte del pozo | Le toca |
|---|---|---|---|
| Ana | 2 (Mañana y Noche) | 2 de 3 | $60.000 |
| Bruno | 1 (solo Mañana) | 1 de 3 | $30.000 |

El valor de cada turno es el pozo dividido por el total de turnos: $90.000 ÷ 3 = $30.000.

## Cómo usarla

1. **Armá el plantel:** en el panel *Plantel*, agregá a cada persona del equipo.
2. **Elegí el período:** arriba de todo, elegí cada cuánto se reparte (por ejemplo, *Quincena*).
3. **Cargá cada día:** en *Registro del día*, escribí la propina del día y marcá los turnos de quienes trabajaron.
4. **Mirá el cierre:** en *Liquidación por persona* está cuánto lleva cada uno y, al terminar el período, cuánto le toca.

## Tecnología

- **Un solo archivo** (`index.html`) con HTML, CSS y JavaScript, sin frameworks ni librerías externas. Solo usa tipografías de Google Fonts.
- **No necesita instalación ni compilación:** se abre directo en el navegador.
- **Datos:** en esta versión se guardan en el navegador de cada persona (`localStorage`). No se comparten entre dispositivos y no salen de tu computadora o celular.

### Probarla en tu computadora

Descargá el repositorio y abrí `index.html` con cualquier navegador. No hace falta nada más.

## Próximos pasos

- Conectarla a una base de datos en la nube para que todo el equipo vea y cargue la misma información desde distintos dispositivos.
- Exportar la liquidación de cada período.

## Autor

**Marcelo A. Guardia** · [github.com/MarceloAGuardia](https://github.com/MarceloAGuardia)
