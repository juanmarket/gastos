# Gastos

App web mínima para anotar qué gasté hoy y con qué pagué. Un solo archivo, sin servidor, los datos quedan en el teléfono.

## Cómo se usa

1. Escribe el valor.
2. Toca el método con el que vas a pagar (Bancolombia, Nequi, Efectivo, o una tarjeta de Apple Wallet).
3. La app guarda el gasto, **copia el valor al portapapeles** y abre la app correspondiente. Pegas el número y listo.

Si te equivocaste, el aviso de abajo tiene **Deshacer** por unos segundos. También puedes borrar cualquier gasto del día con la ×.

## Subirla a GitHub Pages

1. Crea un repo en GitHub (por ejemplo `gastos`).
2. Sube `index.html`, `icon.png` y este `README.md` a la rama `main`.
3. En el repo: **Settings → Pages → Source: Deploy from a branch → main / (root)** → Save.
4. En un minuto queda en `https://TU_USUARIO.github.io/gastos/`.

## Ponerla como app en el iPhone

Abre la URL en Safari → botón Compartir → **Agregar a pantalla de inicio**. Abre a pantalla completa y conserva los datos aunque cierres Safari.

## Presupuesto diario y cuadre

Los días se calculan en hora de Colombia, sin importar la zona horaria del teléfono. Arriba siempre ves **Hoy · jueves, 12 de nov**, lo gastado, el presupuesto del día y cuánto te queda (o cuánto te pasaste), con una barra.

El botón **Cuadre** cierra el día: muestra gastado y saldo, deja editar el presupuesto de hoy, copia el gasto real para pegarlo en el Excel, y pide el **presupuesto de mañana**. A las 00:00 hora Colombia la app arranca con ese presupuesto. Si no pones uno, mañana aparece "Sin presupuesto para hoy".

En "Últimos 7 días" cada día muestra gastado, presupuesto y saldo (verde si sobró, rojo si faltó).

## Detalle de un gasto

Toca cualquier gasto de la lista de hoy para ver y editar la nota completa, la hora y la ubicación donde pagaste (con enlace a Mapas). Se puede borrar desde ahí.

## Ubicación (GPS)

Activada por defecto en ⚙︎. Al registrar un gasto la app pide la ubicación en segundo plano y la guarda con el gasto. La primera vez iOS pregunta si permites la ubicación. El nombre del lugar se consulta a OpenStreetMap solo cuando abres el detalle.

## Enlaces de las apps

Se editan en ⚙︎ (ajustes). Los que vienen por defecto:

| App | Enlace |
|---|---|
| Nequi | `nequi://` |
| Bancolombia | `shortcuts://run-shortcut?name=Bancolombia` |
| Tarjetas (Apple Wallet) | (vacío) |
| Efectivo | (vacío, no abre nada) |

Bancolombia no tiene un enlace público que abra su app, así que se usa un **Atajo de iOS**. Hay que crearlo una vez:

1. Abre la app **Atajos** → **+** → busca la acción **Abrir app** → elige **Mi Bancolombia**.
2. Nómbralo exactamente **Bancolombia** y guarda.

Las tarjetas de Apple Wallet no abren nada: la pantalla de pago (Face ID + acercar al lector) solo se abre con doble clic al botón lateral, y ninguna app puede dispararla. El botón de la tarjeta guarda el gasto y te avisa que ya puedes hacer el doble clic.

## Copia de seguridad

Los datos viven solo en este dispositivo. En ⚙︎ hay **Exportar copia (JSON)** e **Importar copia**. Hazlo cada tanto.
