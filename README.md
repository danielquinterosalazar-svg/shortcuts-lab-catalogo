# Catálogo de skills de AS Shortcuts Lab

Lista de skills (slash commands) de Claude Code que la app **AS Shortcuts Lab** puede descargar
con el botón «Buscar novedades». Es solo texto: un archivo JSON, sin código ni claves.

## Qué hay aquí
- `catalogo-skills.json`: el catálogo. Cada skill trae `nombre` (`/algo`), `queHace`, `servicio`
  (qué ventaja hay detrás), y opcionalmente `seParece` y `loUsasCuando` (la vista «Transición»).

## Por qué un repositorio aparte
La app funciona sin internet. El catálogo vive aparte para poder **añadir skills sin tocar ni
republicar la app**, y para que lo descargado sea solo datos validados, nunca código.

## Reglas del archivo (la app las valida y descarta lo inválido)
- `app` = `as-shortcuts-lab-catalogo-skills`, `esquema` = `1`, `version` entera, `fecha` AAAA-MM-DD, `origen` con texto.
- `nombre`: empieza con `/`, solo minúsculas, números, `-`, `_` y `:`, máximo 40 caracteres.
- Textos de hasta 400 caracteres; máximo 500 skills y 200 000 caracteres en total.

Todo el contenido está «por revisar» hasta que una persona lo verifique contra la documentación oficial.
