# Bitalier

Sitio web de **Bitalier**, una agencia de tecnología y marketing digital: desarrollo de software, marketing, diseño UX/UI, estrategia digital, SEO/SEM y branding.

Hecho con **React 19 + TypeScript + Vite + Tailwind CSS v4**.

## Páginas

| Ruta | Contenido |
|---|---|
| `/` | Inicio: hero con lluvia binaria animada, concepto, servicios, misión y visión, llamada a la acción |
| `/servicios` | Detalle de los seis servicios |
| `/nosotros` | Quiénes somos, misión y visión |
| `/contacto` | Llamada a contactar |

Incluye enlaces a Facebook e Instagram y Google Tag Manager para la analítica.

## Puesta en marcha

Requiere Node.js 20 o posterior.

```bash
npm install
npm run dev       # servidor de desarrollo
npm run build     # compila a dist/
npm run preview   # sirve la compilación
```

### Organigrama en PDF

`scripts/generar-pdf.js` dibuja con jsPDF el organigrama jerárquico de la empresa, siguiendo el modelo *stream-aligned* de Team Topologies. Se hizo como tarea académica.

```bash
node scripts/generar-pdf.js   # genera bitalier-organigrama.pdf
```

## Estructura

```
src/
├── pages/        # Home, ServicesPage, AboutPage, ContactPage
├── components/   # Navbar, Hero, BinaryRain, ServicesSection, ConceptSection,
│                 # MissionVisionSection, CTASection, Footer, NoiseOverlay
├── constants.ts  # Servicios, estadísticas y colores de marca
├── styles/       # Tema, fuentes y Tailwind
└── assets/       # Logos
scripts/
└── generar-pdf.js
```

### Colores de marca

| Nombre | Hex |
|---|---|
| Lima | `#A5F000` |
| Azul profundo | `#03045E` |
| Oscuro | `#0A0C10` |
