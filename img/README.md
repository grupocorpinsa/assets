# Logotipos — Grupo Corpinsa

Archivos oficiales de marca. Cualquier pieza que represente al Grupo debe tomarlos de
aquí y no de una copia suelta.

## Colores institucionales

Leídos del EPS maestro de Illustrator (10/08/2004). El archivo declara solo tres
planchas — magenta, amarillo y negro. No hay cian y no hay color spot.

| | CMYK | Hex | RGB |
|---|---|---|---|
| Naranja Corpinsa | 0 · 60 · 100 · 0 | `#FF6600` | 255 · 102 · 0 |
| Negro Corpinsa | 0 · 0 · 0 · 100 | `#000000` | 0 · 0 · 0 |

**La marca no usa azul.**

### Variantes que no deben usarse

`#F58120` · `#E97118` · `#F36F21` · `#F37022` · `#F97316`

Todas son derivas del maestro por reexportaciones sucesivas. Si encuentras una de
estas en una plantilla, un correo o una pieza impresa, reemplázala por `#FF6600`.

### Pendiente

El equivalente en vinilo aún no está fijado. El maestro es cuatricromía de proceso,
no color spot. El candidato más cercano es Pantone 158 C (0 · 61 · 97 · 0), pero es
una aproximación calculada: debe confirmarse contra guía física y muestra impresa
del proveedor antes de cortar vinilo.

## Archivos

| Archivo | Formato | Uso |
|---|---|---|
| `logo-corpinsa.svg` | Vector | **Fuente de verdad.** Impresión, rotulación, cualquier tamaño |
| `logo-corpinsa-1200.png` | 1200 × 1016, transparente | Presentaciones, portadas |
| `logo-corpinsa-512.png` | 512 × 434, transparente | Web, encabezados |
| `logo-corpinsa-256.png` | 256 × 217, transparente | Correo, firmas, avatares |
| `logo-tecnogruas-642.png` | 642 × 110, transparente | Todo uso de Tecnogrúas |
| `logo-corpinsa-ia-342.png` | 342 × 331, transparente | Corpinsa IA: paneles de los asistentes, herramientas internas, cabecera de los correos automáticos |

### Sobre el vectorial de Corpinsa

Reconstruido desde el EPS original de 2004: 24 trazados Bézier, con el nombre
convertido a curvas. No depende de ninguna fuente instalada y escala sin pérdida
desde un favicon hasta el contrapeso de una torre grúa.

### Sobre Tecnogrúas

**No existe vectorial de esta marca.** Solo mapas de bits. La versión de aquí tiene
642 × 110 px útiles y el fondo blanco recortado a transparencia. Sirve para pantalla
y correo; **no la amplíes más allá de su tamaño nativo** — a tamaño de pluma o cabina
produce bordes dentados. La tipografía del logotipo está viva, no convertida a
curvas, y aún no se ha identificado cuál es. Recuperar o rehacer este vectorial es
trabajo pendiente.

### Sobre Corpinsa IA

Marca de los asistentes y las automatizaciones, no del Grupo. Es la única pieza de
esta carpeta que **no** usa el naranja institucional: su original está en `#F48B2D`,
otra deriva del maestro. Se subió tal cual para no alterar una marca en uso sin
decidirlo antes; queda pendiente resolver si se corrige a `#FF6600` o si el tono
propio es deliberado.

**Tampoco existe vectorial.** El origen era un JPG de 342 × 331 con fondo blanco; la
transparencia se obtuvo resolviendo la mezcla sobre blanco píxel a píxel, no
recortando, así que el antialias del borde se conserva intacto. No lo amplíes por
encima de su tamaño nativo.

El logotipo lleva bastante aire por arriba: la marca ocupa la mitad inferior del
lienzo. Sobre blanco no se nota, pero si lo colocas sobre un fondo de color queda
visiblemente bajo dentro de su caja.

La palabra `corpinsa IA` es casi negra (`#1E1E1D`), así que **sobre fondo oscuro se
pierde**. En cabeceras oscuras, colócalo dentro de una tarjeta blanca.

## Reglas de uso

Un equipo, documento o interfaz lleva el logotipo de la empresa que lo opera, nunca
los dos. El vínculo con el grupo ya está dentro del logo de Tecnogrúas, en el endoso
`GRUPO CORPINSA`; repetir el logo de Corpinsa al lado es redundante.

El isotipo del óvalo no se usa suelto: siempre acompaña a la palabra.

Deja alrededor del logotipo un área libre equivalente a la altura de su letra
inicial, en los cuatro lados.

## Cómo enlazarlos

Para uso de bajo volumen, la URL cruda del repositorio:

```
https://raw.githubusercontent.com/grupocorpinsa/assets/main/img/logo-corpinsa-256.png
```

Para correos masivos y aplicaciones con tráfico, GitHub desaconseja `raw` como CDN y
puede limitar la tasa de peticiones. Usa jsDelivr, que sirve el mismo repositorio con
caché y sin límite práctico:

```
https://cdn.jsdelivr.net/gh/grupocorpinsa/assets@main/img/logo-corpinsa-256.png
```

En HTML de correo, fija la altura y deja el ancho en `auto`. Nunca conviertas los
logos a base64: infla el HTML y Gmail bloquea las imágenes con `data:` URI.
