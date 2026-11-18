# Horas Extra

App de una sola página para registrar horas extra sobre la hora normal de salida.

**Abrir:** https://eljara2002.github.io/horas-extra/

## Cómo funciona

- En día laborable no se marca entrada: el extra es `salida real − hora normal de salida`, más el extra de la mañana si usas «Entré antes».
- En días de descanso y festivos de Portugal se marca ENTRADA y SALIDA, y todo el rango cuenta como extra.
- Los laborables pasados sin salida marcada quedan pendientes de confirmar y no entran en el informe.
- Cada corrección a mano queda registrada con el valor anterior y el nuevo.
- Importe estimado = horas extra × valor de la hora × (1 + recargo del tipo de día).

## Direcciones para automatizar

| Acción | Dirección |
| --- | --- |
| Salida en día laborable | `https://eljara2002.github.io/horas-extra/?accion=termine` |
| Entrada en descanso o festivo | `https://eljara2002.github.io/horas-extra/?accion=entrada` |
| Salida en descanso o festivo | `https://eljara2002.github.io/horas-extra/?accion=salida` |

Abrir una de ellas guarda la hora en ese momento. En iPhone se usan con Atajos (automatización de Lugar → Al salir → Abrir URL) y en Android con MacroDroid (geovalla → Abrir sitio web). Los pasos están en la pestaña **Automatizar** de la app.

## Datos

Se guardan en el `localStorage` del navegador donde abras la página: no hay servidor ni cuenta. Usa siempre el mismo navegador y guarda de vez en cuando la copia de seguridad que aparece en Ajustes.
