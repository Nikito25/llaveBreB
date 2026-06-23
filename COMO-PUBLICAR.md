# Decodificador QR Bre-B

## Archivos
- **index.html** — la app (PWA, para publicar en GitHub Pages).
- **manifest.webmanifest**, **sw.js**, **icon.svg** — soporte PWA (offline + ícono).
- **decodificador-breb.html** — copia autónoma para usar local sin publicar nada.

Todo funciona **sin internet**: la librería de lectura de QR está incrustada.

## Uso local (offline, sin publicar)
Doble clic en `decodificador-breb.html`. Pegás (Ctrl+V), subís imagen o pegás el texto crudo.
> La **cámara** desde el navegador necesita HTTPS, así que en local puede no abrir.
> Para usar la cámara en el celular, publicá la app (abajo) y abrí el link.

## Publicar en GitHub Pages (link universal + offline en el celu)
1. Entrá a https://github.com/new
2. Nombre del repo: `llave-breb` (o el que quieras) · visibilidad **Public** · **Create repository**.
3. En el repo, clic en **"uploading an existing file"** (o Add file > Upload files).
4. Arrastrá estos 4 archivos y confirmá (**Commit changes**):
   - index.html
   - manifest.webmanifest
   - sw.js
   - icon.svg
5. **Settings** (del repo) > **Pages** > en *Source* elegí **Deploy from a branch** >
   Branch: **main** / carpeta **/(root)** > **Save**.
6. Esperá ~1 minuto. Tu link queda:
   `https://TU-USUARIO.github.io/llave-breb/`
7. Abrilo en el celular > menú del navegador > **"Agregar a pantalla de inicio"**.
   Queda como app y funciona **offline** tras la primera vez.

## Actualizar la app más adelante
Subí de nuevo el archivo cambiado y, en `sw.js`, subí la versión (`breb-v1` -> `breb-v2`)
para que los dispositivos tomen la nueva versión.
