# Landing Purple — copy con dos puertas (v2)

Documento de contenido solamente. No toca diseño, layout, tipografías, colores,
componentes ni estructura de bloques: cada snippet reemplaza **solo texto** dentro
del markup existente de `index.html`.

- **Puerta A** — usuario individual / independiente: gratis, AGPL-3.0.
- **Puerta B** — organizaciones: licencia comercial, soporte, integración de
  infraestructura, servidor MCP adaptado.

Puertas visibles en los dos primeros scrolls: **hero** (bajada + los dos CTAs) y
**sección PurpleMD** (bajada + CTA secundario hacia `#empresas`). MCP queda
posicionado como diferenciador y como puente hacia Puerta B.

---

## 0 · Meta tags (head)

```html
<title>Purple · Software que trabaja a tu manera</title>
<meta name="description" content="PurpleMD: editor Markdown con vista previa en vivo, proyectos organizados, exportación a PDF y ZIP y servidor MCP. Gratis para vos; para organizaciones, licencia comercial, soporte e integración a medida.">
```

OG y Twitter (mantener el mismo texto en los cuatro):

```html
<meta property="og:title" content="Purple · Software que trabaja a tu manera">
<meta property="og:description" content="PurpleMD: editor Markdown con vista previa en vivo, proyectos organizados, exportación a PDF y ZIP y servidor MCP. Gratis para vos; para organizaciones, licencia comercial, soporte e integración a medida.">
<meta name="twitter:title" content="Purple · Software que trabaja a tu manera">
<meta name="twitter:description" content="PurpleMD: editor Markdown con vista previa en vivo, proyectos organizados, exportación a PDF y ZIP y servidor MCP. Gratis para vos; para organizaciones, licencia comercial, soporte e integración a medida.">
```

`meta name="theme-color"`, canonical, `og:image` e `og:locale` quedan igual.

---

## 1 · Header / nav

**Nav actual:**
`PurpleMD · MCP · GitHub · [Probar PurpleMD]`

**Nav propuesto:**
`PurpleMD · MCP · Empresas · GitHub · [Probar PurpleMD gratis]`

- Agrega un solo `<a class="nav-enlace">` nuevo (mismo componente existente):
  `<a class="nav-enlace" href="#empresas">Empresas</a>`
- Microcopy del botón del header:

```html
<a class="btn btn-primario btn-chico" href="https://md.purple.com.ar" target="_blank" rel="noopener noreferrer">
  Probar PurpleMD gratis
  <span class="sr-only"> (se abre en una pestaña nueva)</span>
</a>
```

En el menú móvil, mismo cambio de texto en su botón.

---

## 2 · Hero

**Bajada** (misma longitud aproximada, 3–4 líneas):

```html
<p class="hero-bajada">
  Purple crea herramientas directas de usar y cuidadas en los detalles,
  alrededor de cómo trabajan las personas. La primera es PurpleMD: un
  editor Markdown que usás gratis, o que implementás en tu organización
  con licencia comercial y soporte.
</p>
```

**CTAs** — las dos puertas, una por botón:

```html
<div class="hero-ctas">
  <a class="btn btn-primario btn-grande" href="https://md.purple.com.ar" target="_blank" rel="noopener noreferrer">
    Usar PurpleMD gratis
    <span class="sr-only"> (se abre en una pestaña nueva)</span>
  </a>
  <a class="btn btn-secundario btn-grande" href="#empresas">
    PurpleMD en tu organización
  </a>
</div>
```

> GitHub sale del hero: sigue presente en la nav, en la sección PurpleMD, en la
> sección MCP y en el footer. Ninguna puerta pierde su camino.

---

## 3 · Sección PurpleMD

Título sin cambios: **"Escribí en Markdown. El resto lo hace PurpleMD."**

**Bajada** (agrega el eco de las dos puertas sin prometer multiusuario):

```html
<p class="bajada">
  Vista previa en vivo mientras escribís, proyectos organizados y exportación
  a PDF o ZIP cuando el documento está listo. La misma herramienta para vos
  y para la organización donde trabajás.
</p>
```

**Captura y figcaption:** sin cambios.

**Acciones** — Puerta A arriba, Puerta B en el enlace:

```html
<div class="acciones-producto">
  <a class="btn btn-primario btn-grande" href="https://md.purple.com.ar" target="_blank" rel="noopener noreferrer">
    Abrir PurpleMD gratis
    <span class="sr-only"> (se abre en una pestaña nueva)</span>
  </a>
  <a class="enlace-flecha" href="#empresas">
    Para organizaciones: licencia y soporte
    <svg viewBox="0 0 16 16" width="14" height="14" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true" focusable="false">
      <path d="M4.5 11.5 11.5 4.5M5.5 4.5h6v6"/>
    </svg>
  </a>
</div>
```

---

## 4 · Valores (tres items)

01 y 02 sin cambios.

**03 — Conectá tus herramientas** (más fuerte, menos jerga):

```html
<h3 class="valor-titulo">Conectá tus herramientas</h3>
<p class="valor-texto">El servidor MCP integrado deja que una herramienta compatible lea,
busque y organice tus notas sin sacarte del flujo donde ya trabajás.</p>
```

---

## 5 · Sección MCP

Etiqueta y título sin cambios (**"Servidor MCP"** / **"Tus notas, conectadas con
tus herramientas."**).

**Bajada** — el diferenciador, y su derivación natural hacia la puerta B:

```html
<p class="bajada">
  Conectá PurpleMD con un cliente compatible con MCP y llevá el contexto de tus
  notas a donde ya trabajás: resumir, buscar y retomar ideas sin cambiar de
  aplicación. Es lo que más nos diferencia y también el punto de partida para
  adaptar PurpleMD al flujo de un equipo.
</p>
```

**Ejemplo (panel de la nota y panel de la herramienta):** sin cambios de copy.
Solo unificar la ortografía del cliente (ver §10, punto 1).

**Pie del ejemplo** — de "ejemplo ilustrativo" a caso de uso profesional real:

```html
<p class="nota-pie">
  Caso de uso real: un estudio lleva clientes, trabajos en curso y presupuestos
  en PurpleMD y consulta ese estado desde un cliente MCP sin salir de su flujo.
  PurpleMD expone tus proyectos y notas —leer, buscar, crear y mover— a clientes
  compatibles con el protocolo MCP.
</p>
```

**Enlace:** "Ver la documentación de MCP" — sin cambios.

---

## 6 · Sección Exportar

**Bajada** (suma el uso profesional sin inventar nada):

```html
<p class="bajada">
  Convertí tus documentos —apuntes, informes, presupuestos— en PDF bien
  presentados, con una estructura clara y una lectura cuidada.
</p>
```

**Detalle 01** sin cambios. **Detalle 02:**

```html
<h3 class="detalle-titulo">Llevate todo tu proyecto</h3>
<p class="detalle-texto">
  Exportá el proyecto completo en <code>.zip</code> para guardarlo, respaldarlo
  o llevarlo a donde quieras.
</p>
```

Lista de archivos y figcaption sin cambios.

---

## 7 · Sección Organizaciones (ex "Soporte y Empresas")

Etiqueta:

```html
<p class="etiqueta">Organizaciones</p>
```

Título sin cambios (**"¿Necesitás PurpleMD en tu organización?"**).

**Bajada** — se saca el "uso personal y auditoría" (suena a limitación y además
es flojo legalmente: la AGPL no restringe el uso a personas físicas):

```html
<p class="bajada enterprise-bajada">
  Podés usar PurpleMD gratis, con su licencia libre AGPL-3.0. Cuando tiene que
  entrar en una organización, ahí aparecemos nosotros: licencia comercial,
  soporte, integración con tu infraestructura y servidor MCP adaptado a tu
  flujo. Contanos qué necesitás: <a class="enlace" href="mailto:purple.empresas@proton.me?subject=Consulta%20para%20organizaciones%20-%20Purple">purple.empresas@proton.me</a>.
</p>
```

**CTA:**

```html
<a class="btn btn-enterprise" href="mailto:purple.empresas@proton.me?subject=Consulta%20para%20organizaciones%20-%20Purple">
  Escribinos
</a>
```

**Garantías** — 01 y 02 sin cambios; 03:

```html
<circle cx="8" cy="8" r="6"/>
<path d="M8 5v3l2 2"/>
Software libre · AGPL-3.0
```
(sin cambios de texto: sigue siendo correcto y es una garantía real de auditoría).

---

## 8 · Principios y footer

Sin cambios de copy:

- **Simple.** Sin instalación ni configuración: abrís y escribís.
- **Tuyo.** Exportás todo cuando querés, en Markdown, PDF o ZIP.
- **Cuidado.** Accesible, rápido y en español.
- Lema del footer: "Purple construye software que respeta tu forma de trabajar."
- Legal: "© 2026 Purple · Software libre (AGPL-3.0) · Desde el Alto Valle, Patagonia."

---

## 9 · Microcopy de CTAs (referencia rápida)

| Dónde | Texto | Destino | Puerta |
|---|---|---|---|
| Nav (botón) | Probar PurpleMD gratis | `md.purple.com.ar` | A |
| Nav (enlace) | Empresas | `#empresas` | B |
| Hero (primario) | Usar PurpleMD gratis | `md.purple.com.ar` | A |
| Hero (secundario) | PurpleMD en tu organización | `#empresas` | B |
| Sección PurpleMD (primario) | Abrir PurpleMD gratis | `md.purple.com.ar` | A |
| Sección PurpleMD (enlace) | Para organizaciones: licencia y soporte | `#empresas` | B |
| Sección Organizaciones | Escribinos | `mailto:purple.empresas@proton.me` | B |
| Footer | Empresas | `mailto:purple.empresas@proton.me` | B |

Regla aplicada: "gratis" siempre acompaña al CTA de Puerta A (es el gancho real
de la puerta A); "organización / licencia / soporte" siempre acompaña al CTA de
Puerta B (sin prometer SLA, uptime ni niveles de soporte).

---

## 10 · Tabla comparativa

| Sección | Copy actual | Copy propuesto | Por qué |
|---|---|---|---|
| meta description / OG / Twitter | "Purple construye software pensado alrededor de cómo trabajan las personas. Conocé PurpleMD: editor Markdown con vista previa en vivo, proyectos organizados, servidor MCP y exportación a PDF y ZIP." | "PurpleMD: editor Markdown con vista previa en vivo, proyectos organizados, exportación a PDF y ZIP y servidor MCP. Gratis para vos; para organizaciones, licencia comercial, soporte e integración a medida." | El buscador es el primer vendedor. Sin la mención de organizaciones, el comprador empresarial ni siquiera llega a la página. |
| Nav | PurpleMD · MCP · GitHub · Probar PurpleMD | PurpleMD · MCP · **Empresas** · GitHub · Probar PurpleMD **gratis** | Puerta B accesible desde cualquier scroll; "gratis" ancla la puerta A. Mismo componente. |
| Hero bajada | "...La primera es PurpleMD, un editor Markdown que te sigue el ritmo." | "...La primera es PurpleMD: un editor Markdown que usás gratis, o que implementás en tu organización con licencia comercial y soporte." | Cumple el requisito de las dos puertas en el scroll 1, con una sola oración y sin salir del tono. |
| Hero CTA 1 | Conocé PurpleMD (→ #purplemd) | **Usar PurpleMD gratis** (→ md.purple.com.ar) | "Conocer" es pasivo y no cierra la puerta A. Ir directo a la app convierte mejor y el scroll al producto ya está cubierto por la nav. |
| Hero CTA 2 | Ver en GitHub (→ GitHub) | **PurpleMD en tu organización** (→ #empresas) | Un comprador empresarial no convierte con un repositorio. GitHub sigue en nav, secciones y footer: cero pérdida. |
| Sección PurpleMD bajada | "Vista previa en vivo mientras escribís, proyectos organizados y exportación a PDF o ZIP cuando el documento está listo." | Misma frase + "La misma herramienta para vos y para la organización donde trabajás." | Refuerza las dos puertas en el scroll 2 sin prometer multiusuario ni sincronía (que no existen). |
| Sección PurpleMD acciones | Abrir PurpleMD / Ver el repositorio | **Abrir PurpleMD gratis** / **Para organizaciones: licencia y soporte** (→ #empresas) | Puerta B reaparece donde el visitante ya decidió que el producto le sirve. El repo vive en nav/footer/MCP. |
| Valores 03 (MCP) | "...deja que una herramienta compatible lea y organice tus notas desde tu propio flujo." | "...lea, busque y organice tus notas sin sacarte del flujo donde ya trabajás." | "Buscar" es el verbo que más se usa en clientes MCP; "sin sacarte del flujo" dice el beneficio sin jerga. |
| Sección MCP bajada | "...resumir, buscar y retomar ideas sin cambiar de aplicación." | Misma frase + "Es lo que más nos diferencia y también el punto de partida para adaptar PurpleMD al flujo de un equipo." | Declara a MCP como diferenciador y lo convierte en el puente natural hacia Puerta B (integración MCP a medida). |
| Pie del ejemplo MCP | "Ejemplo ilustrativo. PurpleMD expone tus proyectos y notas..." | "Caso de uso real: un estudio lleva clientes, trabajos en curso y presupuestos en PurpleMD y consulta ese estado desde un cliente MCP sin salir de su flujo. PurpleMD expone tus proyectos y notas..." | Convierte la demo en un caso profesional creíble. Se conserva la aclaración técnica del alcance (leer/crear/mover). |
| Sección Exportar bajada | "Convertí tus documentos Markdown en PDF bien presentados..." | "Convertí tus documentos —apuntes, informes, presupuestos— en PDF bien presentados..." | Emplaza al lector en casos profesionales reales (el presupuesto 1042 de la captura) sin inventar features. |
| Detalle Exportar 02 | "...para guardarlo o llevarlo a donde quieras." | "...para guardarlo, respaldarlo o llevarlo a donde quieras." | "Respaldarlo" introduce el lenguaje del comprador de infraestructura con una palabra. |
| Etiqueta sección empresas | Soporte y Empresas | **Organizaciones** | "Soporte y Empresas" suena a apéndice de servicio postventa; "Organizaciones" nombra al comprador y funciona como puerta. |
| Bajada sección empresas | "PurpleMD es software libre (AGPL-3.0) para uso personal y auditoría. Para uso corporativo, integración de infraestructura o licenciamiento comercial a medida, hablemos en..." | "Podés usar PurpleMD gratis, con su licencia libre AGPL-3.0. Cuando tiene que entrar en una organización, ahí aparecemos nosotros: licencia comercial, soporte, integración con tu infraestructura y servidor MCP adaptado a tu flujo. Contanos qué necesitás: ..." | "Uso personal y auditoría" suena a que la AGPL solo cubre a personas físicas (falso) y resta valor. El nuevo texto abre con la puerta A y entrega la puerta B como servicio, enunciando los cuatro frentes reales del negocio. |
| CTA sección empresas | Contactar | **Escribinos** | Verbo de primera persona, cercano, y no promete nada que no esté definido. |
| asunto del mailto | `Consulta Enterprise - Purple` | `Consulta para organizaciones - Purple` | Coherente con el tono sin jerga; además ordena mejor el buzón. |

---

## 11 · Pendientes de verificación antes de publicar

1. **Ortografía de Aria Labs**: el HTML dice "Arya Labs" en el título del panel y
   en el mensaje, pero las rutas dicen `aria-labs` (`clientes/aria-labs`,
   `1042-aria-labs.md`). Elegir una y unificar; lo correcto parece **Aria Labs**.
2. **"Caso de uso real"**: si el nombre del estudio está anonimizado o los datos
   del presupuesto son ficticios, usar "Caso de uso real, con datos modificados"
   en lugar de "Caso de uso real". Es el único punto donde el copy puede quedar
   en desacuerdo con la realidad.
3. **Requiere 2 líneas de HTML**: el `<a class="nav-enlace" href="#empresas">Empresas</a>`
   en la nav (y su par en el menú móvil). Es el único alta de markup de todo el
   documento; todo lo demás es texto.
4. Si PurpleMD corre realmente sin cuenta ni registro desde el navegador, hay una
   frase de alto rendimiento disponible para la puerta A:
   "Abrís y escribís: sin cuenta, sin registro." No la incluí porque no pude
   verificarla en el repo de PurpleMD.
