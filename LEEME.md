# Pádel de los viernes — versión Netlify

## Qué hay en la carpeta
- `public/index.html`: la ficha.
- `netlify/functions/state.mjs`: guarda y lee las marcas en Netlify Blobs (ya trae cargado lo marcado hasta hoy).
- `netlify.toml` y `package.json`: configuración para Netlify.

Importante: arrastrar la carpeta a Netlify Drop NO sirve, porque así no se activa la función que guarda. Usá una de estas dos opciones.

## Opción A: con GitHub (la más cómoda)
1. Creá un repositorio nuevo en GitHub y subí todo el contenido de esta carpeta (incluida la carpeta `netlify`).
2. En Netlify: Add new site → Import an existing project → GitHub → elegí el repositorio.
3. No cambies nada en la configuración (la toma de `netlify.toml`) y tocá Deploy.

## Opción B: con la línea de comandos
Necesitás Node 22 o más nuevo.
1. Abrí una terminal en esta carpeta.
2. `npm install`
3. `npx netlify-cli login`
4. `npx netlify-cli deploy --build --prod` (la primera vez te pide crear o elegir el sitio).

## Para tener en cuenta
- Cualquiera que tenga el link puede marcar. Compartilo solo con el grupo.
- La ficha se actualiza sola cada 20 segundos y cuando volvés a la pestaña.
- Si dos guardan al mismo tiempo, se guardan los dos cambios: el servidor los aplica casillero por casillero.
- Los borradores sin guardar quedan en el teléfono de cada uno aunque cierre la página.
