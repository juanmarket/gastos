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

## Enlaces de las apps

Se editan en ⚙︎ (ajustes). Los que vienen por defecto:

| App | Enlace |
|---|---|
| Bancolombia | `bancolombia://` |
| Nequi | `nequi://` |
| Apple Wallet | `shoebox://` |
| Efectivo | (vacío, no abre nada) |

Si alguno no abre la app, puede que el banco haya cambiado su esquema. Edítalo en ajustes.

## Copia de seguridad

Los datos viven solo en este dispositivo. En ⚙︎ hay **Exportar copia (JSON)** e **Importar copia**. Hazlo cada tanto.
