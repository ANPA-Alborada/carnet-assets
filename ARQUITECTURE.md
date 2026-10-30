# ARQUITECTURE

## Vision general

Este repositorio almacena assets estaticos reutilizables para proyectos relacionados con el carnet de ANPA Alborada.

Repositorio remoto: `git@github.com:ANPA-Alborada/carnet-assets.git`

## Modulos

### Logo principal

- Archivo: `LogoAnpa.png`
- Formato: PNG RGBA
- Dimensiones: 679 x 640 px
- Uso: identidad visual principal del carnet y aplicaciones relacionadas.

### Tira grafica

- Archivo: `strip.png`
- Formato: PNG RGBA
- Dimensiones: 1125 x 432 px
- Uso: recurso grafico complementario para piezas visuales del carnet.

### Imagen de fiesta

- Archivo: `Fiesta.jpeg`
- Formato: JPEG RGB
- Dimensiones: 259 x 194 px
- Uso: recurso visual para comunicaciones de fiesta y piezas relacionadas.

### Banner de evento

- Archivo: `banner-evento.png`
- Formato: PNG
- Dimensiones: 1032 x 812 px
- Uso: recurso visual para cabeceras y comunicaciones de eventos.
- Original: `banner-eventoPRueba.png`, incorporado el 30 de octubre de 2026.
- Sustitucion solicitada expresamente, sin recortes ni transformaciones.
- Autotest local: `cmp banner-eventoPRueba.png banner-evento.png`.

### Banner de Halloween 2026

- Archivo: `banner-eventoHalloween2026.png`.
- Formato: PNG.
- Dimensiones: 1032 × 812 px, proporcion recomendada para eventos Google Wallet.
- Distribucion: URL HTTPS directa de `raw.githubusercontent.com`, rama `main`.
- Independiente del banner anterior; cada pase referencia su propia URL.
- Actualizado el 30 de octubre de 2026 con `banner-eventoPRueba.png`, manteniendo la URL que utilizan los pases existentes.
- Autotest de sustitucion: `cmp banner-eventoPRueba.png banner-eventoHalloween2026.png`.
- Verificacion local: `sips -g pixelWidth -g pixelHeight banner-eventoHalloween2026.png`.
- Autotest publico: `curl --fail --location --output /dev/null "https://raw.githubusercontent.com/ANPA-Alborada/carnet-assets/main/banner-eventoHalloween2026.png"`.

## Reglas de evolucion

- Mantener los assets originales sin sobrescribirlos con versiones derivadas.
- Documentar nuevas categorias de assets como modulos separados.
- Evitar placeholders o datos simulados.
