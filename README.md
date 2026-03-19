# KYBERNIA — AI Governance & Strategy Consulting Website

## Stack
- **HTML5** + **Vanilla CSS** (sin frameworks)
- **JavaScript** vanilla (ES6+)
- **Google Fonts**: Inter
- **Despliegue targets**: GitHub Pages / Vercel

## Estructura del proyecto

```
/
├── src/
│   ├── index.html          ← Página principal (única)
│   ├── css/
│   │   └── styles.css      ← Sistema de diseño + todos los estilos
│   ├── js/
│   │   └── main.js         ← Navegación, animaciones, formulario
│   └── assets/
│       ├── favicon.png
│       ├── logo-dark.png   ← Logo sobre fondo oscuro (default)
│       ├── logo-light.png  ← Logo sobre fondo claro
│       ├── logo-nombre.png ← Logo + nombre completo
│       └── consultant.png  ← Foto del consultor
├── Img/                    ← Logos originales (fuente)
├── Info Origen/            ← Documentación y plan del proyecto
└── README.md
```

## Secciones de la web (single-page)

| Sección | ID | Descripción |
|---------|-----|-------------|
| Header | `#header` | Navegación sticky + logo + CTA |
| Hero | `#hero` | Propuesta principal + glass card |
| Propuesta | `#propuesta` | Value proposition + highlights |
| Pilares | `#pilares` | 3 pilares de expertise |
| Servicios | `#servicios` | 3 packs de consultoría |
| Sobre mí | `#antonio` | Bio del consultor |
| Contacto | `#contacto` | Formulario + contacto directo |
| Footer | `#footer` | Links + legal + copyright |

## Design System

| Token | Valor |
|-------|-------|
| Color primario | `#0db9f2` (cyan) |
| Fondo principal | `#101e22` (dark navy) |
| Fondo secundario | `#0d1a1e` |
| Texto primario | `#f0f8ff` |
| Texto secundario | `#8ba5ad` |
| Fuente | Inter (400/500/600/700/800/900) |
| Grid base | 8px |

## Branding

- **Logo/imagen**: siempre en MAYÚSCULAS → `KYBERNIA`
- **En texto**: siempre capitalizado → `KybernIA` (K e IA en mayúsculas)

## Despliegue

### Opción A — GitHub Pages

1. El fichero `index.html` debe estar en la raíz del repositorio O en `/docs`
2. En GitHub: Settings → Pages → Source: `main` branch, `/docs` folder (o raíz)
3. Si usas `/docs` como carpeta de publicación:
   ```bash
   cp -r src/* docs/
   ```
4. URL resultante: `https://[usuario].github.io/KYBERNIA/`

```yaml
# .github/workflows/deploy.yml (opcional, para CI/CD)
name: Deploy to GitHub Pages
on:
  push:
    branches: [main]
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Deploy
        uses: JamesIves/github-pages-deploy-action@v4
        with:
          folder: src
```

### Opción B — Vercel (recomendada)

1. Conectar repositorio GitHub en vercel.com
2. Framework preset: **Other** (static site)
3. Root directory: `src`
4. Build command: (vacío)
5. Output directory: `.` (raíz del src)
6. Vercel detectará automáticamente el `index.html`

Para dominio personalizado `kybernia.com`:
- En Vercel: Settings → Domains → Add `kybernia.com`
- En tu DNS: añadir CNAME `www` → `cname.vercel-dns.com`
- Añadir A record para apex: `76.76.21.21`

## Modificar contenido

Cada sección tiene comentarios claros en `index.html`:
```html
<!-- ══════════════════════════════════════════
     HERO SECTION
══════════════════════════════════════════ -->
```

Para modificar textos: busca la sección en `index.html` y edita directamente.
Para modificar estilos: usa las CSS custom properties en `:root` en `styles.css`.

## Futuras expansiones (Fase 2)

- [ ] Blog (Ghost o markdown-based)
- [ ] Casos de estudio (portfolio)
- [ ] Recursos descargables
- [ ] Integración Calendly (CTA booking)
- [ ] Google Analytics 4
- [ ] Política de Privacidad / RGPD completa
- [ ] Versión en inglés (i18n)
- [ ] Backend formulario (Formspree / Resend)

## Contacto / LinkedIn

[Antonio Gallego Castillo](https://www.linkedin.com/in/antoniogallegocastillo/)
