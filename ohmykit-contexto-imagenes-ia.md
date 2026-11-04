# Oh my Kit — Contexto para generación de imágenes con IA

> Este archivo reúne todo lo necesario para generar imágenes de marca con IA (fotos de producto, flatlays, texturas) para la landing B2B de Oh my Kit. Pégalo o resume sus apartados en el prompt del generador según lo que necesites.

## 1. Qué es Oh my Kit

Empresa de **kits y packs de regalo personalizados para empresas**, montados a mano. No vende merchandising genérico de catálogo: cada kit se diseña para una ocasión concreta (lanzamiento de producto, feria, campaña de marketing, welcome pack) y no se repite de un cliente a otro.

Origen de la marca: empezaron haciendo kits para bodas, cumpleaños y despedidas. El negocio se ha reorientado a B2B puro, pero conserva ese origen artesanal y personal — es la diferencia que quieren transmitir frente a una caja de swag corporativo impersonal.

**Titular de marca:** «El kit que hace decir "oh, my".»
**Lo que define el producto:** cuidado de regalo personal, hecho a mano, a escala de empresa. No es producción industrial ni dropshipping de merchandising.

## 2. Tono visual — qué buscar y qué evitar

**Buscar:**
- Fotografía de producto tipo **flatlay editorial** (cenital o en ángulo suave), con buena luz natural o de estudio cálida.
- Materiales reales y con textura: cartón kraft, papel, tela, cerámica, madera clara. Nada de plástico brillante genérico.
- Composición cuidada pero no perfecta — con aire de "hecho a mano", no de render 3D ni de catálogo de Amazon.
- Paleta cálida y suave (ver sección 3): fondos en rosa empolvado, lino, papel crudo.
- Una caja abierta o semiabierta con 3-5 objetos dispuestos alrededor, nunca un muro de producto.

**Evitar:**
- Nada de merchandising genérico (bolígrafos con logo, llaveros, USB) como protagonista.
- Nada de iconografía o ilustración plana tipo "stock corporativo" (apretones de manos, bombillas de idea, gráficas).
- Nada de plástico de burbujas, poliespán ni packaging industrial a la vista.
- Evitar el look "generado por IA" típico: simetría perfecta, texto ilegible superpuesto, brillos artificiales, manos deformes si aparecen personas.
- No usar colores saturados ni neón — la marca es suave, nunca vibrante.

## 3. Paleta de color (activa: Rosa empolvado)

| Variable | Hex | Uso |
|---|---|---|
| `--paper` | `#F7EFEA` | Fondo principal, papel cálido claro |
| `--paper-deep` | `#EFDFD8` | Fondo secundario, superficies de producto |
| `--label` | `#FFFAF7` | Blanco cálido, etiquetas |
| `--field` | `#DDA7A2` | **Rosa empolvado — color de marca principal**, bloques grandes |
| `--accent` | `#93453F` | Granate, acentos y detalles |
| `--btn-face` / `--dark` | `#5E3B3C` / `#4A3032` | Ciruela oscuro, texto y superficies oscuras |
| `--ink` / `--ink-deep` | `#3E2A2B` / `#2B1B1C` | Casi negro cálido (texto, nunca negro puro) |
| `--ink-soft` | `#7A5F60` | Gris rosado para texto secundario |

**Resumen para el prompt:** *rosa empolvado (#DDA7A2), ciruela oscuro (#4A3032 / #2B1B1C), granate (#93453F), sobre fondo papel cálido (#F7EFEA). Sin negro puro, sin blanco puro, sin colores fríos.*

## 4. Tipografía (por si el generador compone texto o para mantener coherencia de marca)

- Titulares: **Gloock** — serif de alto contraste, elegante, con un punto gastronómico/premium.
- Texto corrido: **Hanken Grotesk** — sans-serif neutra.
- Datos y etiquetas pequeñas: **DM Mono**.

(En general, mejor generar las imágenes *sin* texto y añadir cualquier rótulo después en el HTML — los generadores de imagen no reproducen bien estas tipografías.)

## 5. Qué imágenes hacen falta

### A) Carrusel del hero (4 imágenes) — formato vertical 2:3, mínimo 900×1350 px
Van en `fotos/`, ver `fotos/LEEME.txt`. Una composición tipo flatlay por kit, fondo en tonos papel/rosa empolvado:

1. **Kit de lanzamiento** — caja abierta, muestra de producto, carta de presentación. Props sugeridos: caja rígida, tarjeta/carta con sello de lacre o similar, un objeto "producto" genérico bien presentado.
2. **Kit de feria** — bolsa de tela, algo para picar (ej. una chocolatina o café de especialidad), tarjeta con QR.
3. **Welcome pack** — caja, taza de cerámica, libreta, nota de bienvenida manuscrita.
4. **Campaña de marketing** — caja de envío, producto protagonista, tarjeta con mensaje de campaña.

### B) Galería "Algunos kits" — formato 3:2 (la primera, más grande, es flexible/vertical también sirve)
Mismo criterio que el carrusel pero con más aire alrededor, como foto de portfolio:
1. Kit de lanzamiento (foto grande/destacada)
2. Kit de feria
3. Welcome pack

## 6. Referencias de estilo (sólo para calibrar el nivel, no para copiar)

Marcas de regalo corporativo B2B usadas como referencia de diseño general (no necesariamente de fotografía): **Teak & Twine**, **&Open**, **Bestowe Gifting**. El denominador común: fotografía de producto limpia, mucho aire, sin precios ni checkout a la vista, foco en el objeto real por encima de ilustración o iconografía genérica.

## 7. Prompt base sugerido (punto de partida, ajustar por imagen)

> Editorial flatlay product photography of a curated corporate gift box, warm dusty-rose and plum color palette (#DDA7A2, #4A3032, #93453F) on a warm cream paper background (#F7EFEA), soft natural daylight, slight overhead angle, handmade artisanal feel, textured materials (kraft cardboard, fabric, ceramic), minimal props arranged with care, no text, no logos, no plastic packaging, muted and warm tones, shot on film, shallow depth of field
