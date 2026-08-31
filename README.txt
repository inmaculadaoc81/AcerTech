AcerTech ONE PAGE

Dominio:
https://reparaciondeportatilesmadrid.com.es/

Teléfono SOLO en caja de información:
+34 910 05 40 41

Teléfono en todos los botones:
+34 914 46 85 03

Diagnóstico:
GRATUITO

Variables SMTP compartidas en Vercel:
SMTP_HOST=cp7124.webempresa.eu
SMTP_PORT=465
SMTP_SECURE=true
SMTP_USER=soporte@kelatos.com
SMTP_PASS=[configurada únicamente en Vercel]
CONTACT_EMAIL=soporte@kelatos.com

El correo no aparece visible en la web; solo se utiliza en /api/contacto.

Google Analytics:
G-V5SXVC3M37

HISTORIAL: el repositorio era multipágina (7 páginas /modelos/ de
gamas Acer y varias páginas /servicios/) y se convirtió a one-page;
esas páginas fueron eliminadas en commits anteriores. Como ya no
existen en el sitemap actual, se ha añadido middleware.mjs para
redirigir (301) cualquier URL antigua a la home, evitando 404 en
enlaces indexados o backlinks antiguos. Excluye /api/* y cualquier
ruta con extensión de archivo. Se añadió "@vercel/functions": "^2.0.3"
a package.json como dependencia de esta función.

Dominio revisado contra el resto de dominios de la familia en esta
sesión (incluido AcerGlobal, globalacer.com.es): sin colisión.

REVISIÓN (fixes aplicados en esta pasada):
- Ya estaba bien: banner de cookies, schema.org LocalBusiness (ya
  usaba correctamente el teléfono de la caja de información,
  +34 910 05 40 41, no el de los botones), sección SEO "Sobre Acer",
  api/contacto.js con SMTP + nodemailer. No se ha modificado ninguno
  de estos, ni ninguno de los dos números de teléfono.
- Google Analytics: no existía. Añadido G-V5SXVC3M37.
- Meta robots: no existía. Añadido.
- .navcall: el texto largo ("Atención Telefónica 24 horas 365 días")
  deformaba la píldora del menú. Acortado a solo el número (mismo
  número de los botones, +34 914 46 85 03) y añadido
  white-space:nowrap como salvaguarda.
- H1 de portada reescrito, corto, directo y totalmente afirmativo
  (sin interrogación ni condicionales), incluye la marca: "Tu Acer no
  funciona. Te damos una solución clara." Tamaño del H1 aumentado:
  clamp(38-58px) → clamp(46-74px) en escritorio, 40px → 48px en
  móvil.

REVISIÓN ADICIONAL (checklist unificado de la familia, a petición del cliente):
- H1 repetía la plantilla "no funciona" usada en varios repos.
  Reescrito con estructura de una sola frase, imperativa: "Repara tu
  Acer con diagnóstico claro y rápido." (8 palabras).
- BUG REAL — dos textos decorativos gigantes sin reducción de tamaño
  en móvil/tablet: ".problems::after" ("ACER", 180px) y
  ".hardware-art::before" ("HARDWARE", 82px). Añadida reducción en
  tablet (110px/60px) y móvil (64px/42px).
- Enlace de política de privacidad: la casilla existía pero sin
  enlace. Añadido a https://kelatos.com/privacy-policy/, en azul y
  subrayado.
- El aviso de servicio independiente solo estaba en letra pequeña del
  footer. Añadida la franja destacada bajo el menú.
- Añadido "Sábados, domingos y días festivos estamos cerrados" debajo
  del horario.
- Botón "Atención Telefónica..." sin icono, a diferencia del de
  WhatsApp. Añadido.
- Verificado: schema.org ya usaba correctamente el teléfono de la
  caja de información; formulario correctamente conectado a
  /api/contacto. Sin cambios en ninguno de estos.

REVISIÓN ADICIONAL (a petición del cliente, tras ver captura en vivo):
- Quitada la pestaña/etiqueta rotada (.hero-chip, "Portátiles · PCs ·
  All-in-One Acer") que sobresalía y se solapaba con la caja de
  información en anchos de tablet/escritorio medio. Se deja como
  regla para toda la familia: no volver a añadir este tipo de
  elemento decorativo.
