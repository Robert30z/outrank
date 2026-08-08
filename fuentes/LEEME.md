# Tipografia de OUTRANK

Auto-hospedada a proposito. Nada de Google Fonts ni CDN: se sirve desde
outrankpr.com, no hay peticion a terceros, no se puede caer y no filtra
visitantes a otro dominio.

| Archivo | Familia | Uso | Peso |
|---|---|---|---|
| `archivo.woff2` | Archivo Variable | Titulares y cuerpo | 100 a 900 |
| `jetbrains-mono.woff2` | JetBrains Mono Variable | Datos, etiquetas, cifras | 100 a 800 |

Las dos son **variables**: un solo archivo cubre todos los pesos. Juntas
pesan 75 KB, menos que una sola foto del sitio.

## Licencia

Ambas bajo **SIL Open Font License 1.1**, que permite uso comercial y
auto-hospedaje. Copias completas en `LICENSE-Archivo.txt` y
`LICENSE-JetBrainsMono.txt`. No se pueden vender por separado y hay que
conservar el aviso de copyright, cosa que estos archivos hacen.

## Si hay que regenerarlas

    curl -o archivo.woff2 https://cdn.jsdelivr.net/npm/@fontsource-variable/archivo/files/archivo-latin-wght-normal.woff2
    curl -o jetbrains-mono.woff2 https://cdn.jsdelivr.net/npm/@fontsource-variable/jetbrains-mono/files/jetbrains-mono-latin-wght-normal.woff2

Son el subconjunto **latin**. Si algun dia hace falta otro alfabeto, hay
que bajar el subconjunto correspondiente y anadir un `@font-face` con su
`unicode-range`.
