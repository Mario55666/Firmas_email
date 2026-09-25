# Firmario

Estudio de firmas corporativas para correo electrónico. Es una sola página HTML, CSS y JavaScript que genera firmas con **tablas y estilos en línea**, el formato que aceptan Gmail, Outlook, Apple Mail, Yahoo Mail y Thunderbird.

- **Página publicada:** https://claude.ai/artifact/FpC3t7uZka5H1usxSx5mwq
- **Demo:** Hogar de Niños Posada de Belén (Callao, Perú)

---

## Contenido de la carpeta

| Archivo | Descripción |
|---|---|
| `index.html` | La aplicación completa: estructura, estilos, lógica, logo de demostración y guía de instalación. No necesita servidor ni dependencias. |
| `logo-posada-de-belen.png` | Logo de la demo con fondo transparente (360 × 360 px), listo para subirlo al sitio web y usarlo como URL pública. |
| `README.md` | Este documento. |

Para usarla, abre `index.html` en Chrome, Edge, Firefox o Safari.

---

## Funciones

### 20 estilos de diseño
Cada estilo usa solo recursos que un correo admite: tipografía, paleta, tipo de filete divisorio, marco del logo, iconografía y una franja de colores de marca.

| N.º | Estilo | Rasgos principales |
|---|---|---|
| 01 | Minimalism | Una familia tipográfica, gris cálido, filete de 1 px |
| 02 | Maximalism | Paleta de joyas, serif de alto contraste, franja de cinco colores |
| 03 | Surreal design | Serif lírica, violeta onírico, filete punteado |
| 04 | Swiss design | Grotesca pesada, rojo señal, filete negro de 3 px |
| 05 | Y2K design | Plata y azul eléctrico con acento magenta |
| 06 | Editorial | Cursiva Playfair, versalitas espaciadas, tono vino |
| 07 | Pixel art | Nombre en tipografía de 8 bits e iconos pixelados |
| 08 | Clay style | Formas redondeadas, lila y coral |
| 09 | Glassmorphism | Panel azul hielo con bordes finos |
| 10 | Cyberpunk | Mayúsculas técnicas, monoespaciada, neón contenido |
| 11 | Pop art | Primarios planos y contorno negro |
| 12 | Retro | Atardecer setentero en franjas |
| 13 | Collage art | Máquina de escribir y papeles superpuestos |
| 14 | Vector art | Geometría plana, azul y coral |
| 15 | Futuristic | Mayúsculas espaciadas, oro fino, azul noche |
| 16 | Handwritten | Nombre manuscrito en tinta azul sobre datos formales |
| 17 | Bohemian | Cursiva Cormorant, salvia y óxido |
| 18 | Graffiti | Nombre en rotulador con acentos urbanos |
| 19 | Aurora | Azul profundo y franja de cinco tonos boreales |
| 20 | Victorian style | Serif antigua, doble filete dorado, monograma fraktur |

### Organización de la firma
| Familia | Variantes |
|---|---|
| **Horizontal** | Clásica (logo, divisor, datos) · Tres columnas (logo, identidad, contacto) |
| **Vertical** | Alineada a la izquierda · Centrada |
| **Lateral** | Panel de marca a la izquierda · Panel de marca a la derecha |

### Identidad de marca
- Subida de logo en **PNG o SVG**. Los SVG se convierten automáticamente a PNG nítido, porque Gmail y Outlook no muestran SVG.
- Control del ancho del logo (56–220 px).
- Campo **URL pública del logo**: si se completa, la firma copiada enlaza la imagen en vez de incrustarla (necesario para Gmail y Yahoo).
- Sin logo, se muestra un monograma con las iniciales de la institución.

### Iconos de contacto
- **Según el estilo** (predeterminado): cada estilo tiene su propia iconografía (forma, grosor de trazo, color y marco).
- **Sin iconos · Etiquetas · Símbolos:** son texto y funcionan en cualquier cliente.
- **Línea · Sólido · Círculo · Cuadrado:** iconos en imagen PNG, generados con los colores de cada estilo.
- Cubren correo, celular, teléfono, web, dirección, Facebook, LinkedIn, Instagram, TikTok y X.

### Datos disponibles
Nombre, cargo, institución, correo, celular, teléfono fijo, sitio web, dirección, Facebook, LinkedIn, Instagram, TikTok, X, lema y aviso legal o de confidencialidad. Los datos se guardan en el navegador (`localStorage`).

### Exportación
- **Copiar firma:** copia la firma formateada para pegarla en el editor de firmas.
- **Copiar HTML:** copia el código fuente para Thunderbird, Outlook clásico o Apple Mail.
- **Contador de caracteres:** avisa si se supera el límite de 10 000 caracteres de Gmail.

---

## Datos de la demo

| Campo | Valor |
|---|---|
| Nombre | Fernando Eslava |
| Cargo | Director del Hogar |
| Institución | Hogar de Niños Posada de Belén |
| Correo | hermanatierracallao@yahoo.es |
| Celular | 999 124 794 |
| Teléfono | (511) 429 6307 |
| Web | www.hogarposadadebelen.org.pe |
| Dirección | Av. 2 de Mayo 771, Cercado del Callao 07021, Perú |
| Facebook | https://www.facebook.com/PosadaDeBelenCallao |
| Instagram | https://www.instagram.com/hogarposadadebelen_oficial |
| TikTok | https://www.tiktok.com/@posadadebelen |

Configuración inicial: organización **Lateral · Panel izquierdo**, estilo **Handwritten**, iconos **Según el estilo**. El botón «Restaurar datos y logo de ejemplo» vuelve a estos valores.

---

## Cómo instalar la firma

### Paso previo: publicar el logo
1. Sube `logo-posada-de-belen.png` al sitio web, por ejemplo `https://www.hogarposadadebelen.org.pe/logo-firma.png`.
2. Comprueba que la dirección empiece por `https://` y se abra en una ventana privada sin iniciar sesión. Los enlaces para compartir de Google Drive o Dropbox no sirven, porque abren una página de vista previa y no la imagen.
3. Pega la dirección en **URL pública del logo**.

### Métodos
- **Método A, «Copiar firma»:** pegar con `Ctrl+V` / `⌘+V` en el editor de firmas del cliente.
- **Método B, «Copiar HTML»:** insertar el código fuente. Solo en Thunderbird, Outlook clásico (archivo `.htm`) y Apple Mail (archivo `.mailsignature`).

| Cliente | Método | Logo | Iconos recomendados |
|---|---|---|---|
| Gmail (web) | A | URL pública | Etiquetas o Símbolos |
| Yahoo Mail (web) | A | URL pública | Etiquetas o Símbolos |
| Outlook web y nuevo Outlook | A | URL pública o incrustado | Cualquiera |
| Outlook clásico (Windows) | A, o B con `.htm` | URL pública o incrustado | Cualquiera |
| Apple Mail (macOS) | A, o B con `.mailsignature` | URL pública o incrustado | Cualquiera |
| Thunderbird | B | URL pública | Cualquiera |

### Yahoo Mail
1. Pulsa **Copiar firma**.
2. En mail.yahoo.com: **⚙ Configuración → Más configuración → Escribir correo electrónico**.
3. En **Firma**, activa el interruptor de la cuenta.
4. Pega en el cuadro; los cambios se guardan solos.

### Gmail
1. Pulsa **Copiar firma**.
2. **⚙ → Ver toda la configuración → General → Firma → + Crear nueva**.
3. Pega en el cuadro.
4. En **Valores predeterminados de firma**, elígela para mensajes nuevos y para respuestas.
5. Pulsa **Guardar cambios** al final de la página.

### Outlook web y nuevo Outlook
1. **⚙ Configuración → Cuentas → Firmas → + Nueva firma**.
2. Pega, asígnala como predeterminada y pulsa **Guardar**.

### Outlook clásico (Windows)
- **Opción 1:** **Archivo → Opciones → Correo → Firmas → Nueva**, pega y acepta.
- **Opción 2:**
  1. Cierra Outlook.
  2. Pulsa `Win+R`, escribe `%APPDATA%\Microsoft\Signatures` y pulsa Enter.
  3. Guarda el HTML como `Firma corporativa.htm` (UTF-8) en esa carpeta.
  4. Abre Outlook y elige la firma en **Firmas**.

### Apple Mail
- **Opción 1:**
  1. **Mail → Ajustes → Firmas → +**.
  2. Desmarca «Usar siempre mi fuente predeterminada del mensaje».
  3. Pega la firma.
- **Opción 2:**
  1. Crea una firma provisional y cierra Mail.
  2. Abre `~/Library/Mail/V…/MailData/Signatures/`.
  3. Reemplaza el cuerpo del `.mailsignature` más reciente por el HTML, conservando los encabezados.
  4. Guarda y bloquea el archivo (`⌘+I`).

### Thunderbird
1. **☰ → Configuración de cuentas → Texto de la firma**.
2. Marca **Usar HTML** y pega el código.

### Móviles
Las apps de Gmail, Outlook y Mail de iPhone solo guardan firmas de formato básico. Para que se use la firma configurada en la web, deja vacía la firma de la app móvil de Gmail.

---

## Compatibilidad y limitaciones

- **Imágenes incrustadas:** Gmail y Yahoo pueden eliminarlas al pegar. Usa la URL pública del logo y los iconos Etiquetas o Símbolos.
- **Límite de Gmail:** 10 000 caracteres. Si se supera, quita el aviso legal o las redes, o elige «Sin iconos».
- **Fuentes web:** se ven en Apple Mail y en algunos clientes. El resto usa la fuente de respaldo de cada estilo (Arial, Georgia, Verdana…).
- **Outlook clásico:** ignora las esquinas redondeadas.
- **Modo oscuro:** algunos clientes invierten los colores. Conviene un logo con buen contraste o con contorno claro.
- **Ancho máximo:** 600 px.

---

## Personalización para desarrolladores

Todo está en `index.html`, dentro del bloque `<script>`:

| Constante | Qué define |
|---|---|
| `DEFAULTS` | Datos de la demo |
| `STYLES` | Los 20 estilos: tipografías (`font`, `nf`), colores (`fg`, `mut`, `acc`, `co`, `tint`), filete (`rule`), tamaños, franja (`strip`) y monograma (`mono`) |
| `ICO` | Iconografía de cada estilo: modo, grosor (`sw`), radio (`r`), colores (`col`, `gc`, `lc`), borde (`ring`), `pixel` |
| `LAYOUTS` | Las seis organizaciones y sus miniaturas |
| `SAMPLE_LOGO` | Logo de demostración en base64 |
| `buildSignature()` | Genera el HTML final de la firma con tablas y estilos en línea |

Para añadir un estilo, agrega un objeto a `STYLES` con un `id` nuevo y su entrada en `ICO`.

---

## Créditos

Diseñado por **d3magindesign-2026** · Mg Mario Quiroz Martinez
