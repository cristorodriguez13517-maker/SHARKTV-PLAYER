# SHARKTV PLAYER

Reproductor web independiente de SHARKTV para dos fuentes:

- **YouTube** mediante el reproductor oficial integrado de YouTube.
- **AllDebrid** mediante el Worker de SHARKTV y la verificación Cloudflare Turnstile.

## Publicación

En GitHub abre **Settings → Pages** y selecciona:
- **Deploy from a branch**
- Branch: **main**
- Folder: **/(root)**

La dirección prevista es:

https://cristorodriguez13517-maker.github.io/SHARKTV-PLAYER/

## Parámetros de entrada

YouTube:

`?source=youtube&url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DVIDEO_ID`

AllDebrid con enlace ya generado:

`?source=alldebrid&url=ENLACE_DIRECTO`

AllDebrid solicitando el enlace desde el Worker:

`?source=alldebrid&tipo=movie&magnet_id=ID&file_path=RUTA`

## Compatibilidad

La reproducción directa depende de los códecs y contenedores que admita el navegador/dispositivo. MP4/H.264 y HLS suelen ser los más compatibles. MKV, AVI, HEVC/H.265, DTS y otros formatos pueden no reproducirse en todos los navegadores. YouTube puede impedir la inserción de determinados vídeos por restricciones del propietario, edad o región.

El reproductor no almacena enlaces directos ni credenciales de AllDebrid.