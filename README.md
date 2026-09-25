# Firmario

Firmario es una aplicación web de un solo archivo (`index.html`) que genera firmas de correo electrónico en HTML. Las firmas usan tablas y estilos en línea, con un ancho máximo de 600 px.

## Uso

1. Abrir `index.html` en un navegador de escritorio. No requiere instalación ni servidor.
2. Completar los datos de contacto.
3. Cargar un logo en PNG o SVG, o indicar su URL pública.
4. Elegir la organización, el estilo y el tipo de iconos.
5. Pulsar **Copiar firma** (texto enriquecido) o **Copiar HTML** (código).
6. Pegar la firma en la configuración del cliente de correo, según las instrucciones de la sección «Cómo insertar la firma en tu correo».

## Campos de datos

Nombre y apellido, cargo, empresa o área, correo, celular, teléfono fijo, sitio web, dirección, Facebook, LinkedIn, Instagram, TikTok, X, lema (opcional) y aviso legal o de confidencialidad (opcional).

## Logo

- Formatos admitidos: PNG y SVG. El archivo se convierte a PNG dentro del navegador.
- Ancho de visualización: de 56 a 220 px, en pasos de 2 px. Valor inicial: 104 px.
- Sin logo, la firma muestra un monograma con las iniciales de la empresa.
- Campo **URL pública del logo**: la firma enlaza la imagen alojada en lugar de incrustarla. Es el método indicado para Gmail y Thunderbird.

## Organizaciones

| Familia | Variantes |
|---|---|
| Horizontal | Clásica, Tres columnas |
| Vertical | Alineada, Centrada |
| Lateral | Panel izquierdo, Panel derecho |

## Estilos

20 estilos: Minimalism, Maximalism, Surreal design, Swiss design, Y2K design, Editorial, Pixel art, Clay style, Glassmorphism, Cyberpunk, Pop art, Retro, Collage art, Vector art, Futuristic, Handwritten, Bohemian, Graffiti, Aurora y Victorian style.

## Iconos de contacto

8 modos: Según el estilo, Sin iconos, Etiquetas, Símbolos, Línea, Sólido, Círculo y Cuadrado.

## Clientes de correo documentados

- Gmail (navegador)
- Outlook web y nuevo Outlook (outlook.com, Microsoft 365 y app nueva de Windows)
- Outlook clásico para Windows (editor o archivo `.htm`)
- Apple Mail para macOS (Ajustes o archivo `.mailsignature`)
- Yahoo Mail (navegador)
- Thunderbird (código HTML pegado directamente)
- Móviles iPhone y Android (soporte limitado)

Gmail admite firmas de hasta 10 000 caracteres. La interfaz muestra un contador de caracteres junto a los botones de copia.

## Datos de ejemplo

El archivo trae precargada una marca ficticia: Molle & Grano · Tostadores de café (firmante: Lucía Paredes, Jefa de Tostado), con logo de muestra. El dominio `molleygrano.pe`, los teléfonos, la dirección y los perfiles de redes son inventados. El botón **Restaurar datos y logo de ejemplo** vuelve a cargar estos valores.

## Almacenamiento

Los datos del formulario, el estilo, la organización y el logo cargado se guardan en el `localStorage` del navegador con la clave `firmario-demo-molle-1`. No se envían a ningún servidor. El logo de muestra no se guarda.

## Dependencias externas

Tipografías de Google Fonts (`fonts.googleapis.com`). Sin conexión, el navegador usa las fuentes de respaldo declaradas en cada estilo.
