# 🚀 PRIMER PROMPT PARA ANTIGRAVITY
## AI Strategy Lab — Website MVP

**Tu rol**: Eres un experto en no-code web design y desarrollo. Tu tarea es ayudar a construir el MVP del sitio web para "AI Strategy Lab", un consultor de gobernanza de IA enfocado en PYMES europeas.

**Contexto del cliente**: Antonio es un consultor especializado en:
- Adopción estratégica de IA para organizaciones medianas (200–500 empleados)
- Gobernanza de IA (AI Act, GDPR, ISO/IEC 42001)
- Frameworks de transformación y upskilling organizacional
- Público: C-suite (CEOs, CFOs, CTOs) en España y Europa

---

## 📋 PROYECTO: AI Strategy Lab Website

### 🎯 Objetivo Principal
Crear un sitio web **descriptivo y profesional** que:
1. Posicione a Antonio como experto en gobernanza + adopción de IA
2. Genere leads cualificados (reservas de sesiones de estrategia)
3. Sea responsive, accesible y SEO-optimizado
4. Cumpla con RGPD (formulario de contacto)

**Timeline**: MVP en 6-8 semanas
**Stack**: Antigravity + Tailwind CSS + Material Design Icons

---

## 🎨 DISEÑO & ESTILO

### Paleta de Colores
```
Primario:        #0db9f2  (cyan/teal - confianza tecnológica)
Secundario:      #101e22  (dark navy - profesionalidad)
Fondo oscuro:    #101e22  (default)
Fondo claro:     #f5f8f8  (alternativo para secciones)
Acentos:         Gradientes primary → primary/10
Texto primario:  #ffffff (en dark), #1f2937 (en light)
Texto secundario: #9ca3af (gris neutral)
```

### Tipografía
- **Font**: Inter (sans-serif)
- **Weights**: 400 (regular), 500 (medium), 600 (semibold), 700 (bold), 800 (extrabold)
- **H1**: 48px–72px, bold
- **H2**: 32px–48px, semibold
- **Body**: 16px, regular
- **Caption**: 12px–14px, medium

### Componentes Clave
**Botones**:
- Primario: `bg-primary hover:bg-primary/90 text-dark font-bold py-3 px-6 rounded-lg transition-all`
- Secundario: `border border-primary text-primary hover:bg-primary/10`
- Estados: hover, active, focus (ring-2 ring-primary/50)

**Cards**:
- Fondo: `bg-white dark:bg-slate-900 rounded-2xl p-8 border border-slate-200 dark:border-slate-800`
- Hover: `hover:shadow-xl transition-all`
- Glass cards (hero): `bg-slate-900/40 backdrop-blur-xl border border-primary/10`

**Iconografía**: Material Symbols Outlined (Google Fonts)

**Espaciado**: Sistema de 8px (0.5rem = 8px, 1rem = 16px, etc.)

---

## 📄 ESTRUCTURA DE CONTENIDO

### 1. Header/Navigation (Sticky)
```
├─ Logo + Brand Name: "AI Strategy Lab"
├─ Nav items (desktop): Expertise | About | Services | Contact
├─ CTA Button: "Book a Session"
└─ Mobile menu (hamburger)
```

**Detalles**:
- Sticky top con backdrop blur
- Logo: Icono + texto (usar Material Symbol "insights")
- Links anclan a secciones (#expertise, #about, #services, #contact)
- Responsive: Hamburger en mobile

### 2. Hero Section
```
Left column (60%):
├─ Etiqueta: "🚀 Transformación Responsable"
├─ H1: "Liderando la Adopción Segura y Estratégica de la IA en la Empresa"
│   (con "Segura" y "Estratégica" en color primary)
├─ Descripción: "Definición de marcos de gobernanza, cumplimiento regulatorio 
│   y transformación cultural para convertir la Inteligencia Artificial 
│   en un motor de valor real, responsable y sostenible."
└─ Botones:
    ├─ Primario: "Descubre el Valor de la IA"
    └─ Secundario: "Ver Casos de Estudio" (futura)

Right column (40%):
├─ Glass card con mockup (3 iconos: Gobernanza, Personas, Procesos)
└─ Fondo: Gradiente radial con brillo primary
```

**Altura**: min-h-screen (full height)
**Fondo**: Gradiente dark + subtle grid pattern
**Tono**: Consultivo, profesional, enfocado en transformación organizacional (no solo tech)

### 3. Value Proposition Section
```
H2: "La IA no es un Proyecto Tecnológico, es una Evolución Organizacional"

Cita destacada (card con border-left primary, fondo secondary):
"Ayudo a las empresas a navegar la complejidad del ecosistema de la IA 
mediante un enfoque integral que garantiza que cada implementación sea 
segura, ética y, sobre todo, generadora de resultados medibles."

Párrafo de contexto:
"La verdadera transformación no ocurre en los servidores, sino en la cultura 
de la empresa. Por ello, pongo la gestión del cambio y el desarrollo de las 
personas en el centro de la adopción tecnológica."
```

**Fondo**: light gray (slate-50 dark:slate-900/50)
**Estilo**: Cita prominente con diseño consultivo, no corporativo

### 4. Core Expertise Section (3 Pilares Estratégicos)
```
H2: "Los Tres Pilares de la Transformación de IA"

PILAR I: Estrategia y Gobernanza Sólida
├─ Definición Estratégica: Alineamiento de la IA con objetivos organizacionales
├─ Modelos Operativos: Diseño de estructuras para escalar IA con control
├─ Políticas de Cumplimiento: Guías de uso + EU AI Act + GDPR
└─ IA Responsable: Marcos éticos y transparencia

PILAR II: Cultura, Personas y AI-Fluency
├─ Evolución de Roles: Nuevos perfiles profesionales
├─ Programas AI-Fluency: Formación técnica y funcional
├─ Gestión del Cambio: Transformación de mentalidad organizacional
└─ AI Champions: Redes internas de expertos

PILAR III: Optimización de Procesos e Innovación
├─ Reingeniería de Procesos: Más allá de herramientas
├─ Mejora Continua: Aplicación de IA en flujos existentes
└─ Medición de Impacto: KPIs y ROI validado
```

**Layout**: 3 cards (grid md:grid-cols-3) o columna en mobile
**Fondo**: white dark:bg-background-dark
**Estilo**: Cards con borde left en color primary, sin iconos (puramente texto)

### 5. Services Section
```
H2: "Servicios de Consultoría Estratégica"
Descripción: "Engagements estructurados para llevar tu organización desde 
la curiosidad inicial hasta la adopción integral y sostenible de IA."

3 cards (grid md:grid-cols-3):

Card 1: "Diagnóstico de Madurez y Gobernanza de IA"
├─ Descripción: Análisis profundo de tu posición actual en gobernanza, 
│   regulación y preparación tecnológica/organizacional
├─ Incluye:
│   ├─ Evaluación de Marco Gobernanza Actual
│   ├─ Análisis de Cumplimiento (EU AI Act, GDPR)
│   └─ Evaluación de Capacidades de Personas
└─ Button: "Solicitar Sesión de Descubrimiento"

Card 2: "Programa de Transformación Integral" (DESTACADA - scale-105, border-2 primary)
├─ Badge: "Más Popular"
├─ Descripción: Acompañamiento de 6-12 meses con gobernanza, upskilling, 
│   reingeniería de procesos y medición de ROI
├─ Incluye:
│   ├─ Definición de Estrategia y Gobernanza
│   ├─ Diseño de Modelos Operativos
│   ├─ Programas de AI-Fluency y Change Management
│   └─ Framework de Medición de ROI
└─ Button: "Solicitar Sesión de Descubrimiento" (bg-primary)

Card 3: "Sesiones Estratégicas Ejecutivas"
├─ Descripción: Talleres intensivos para C-suite sobre gobernanza, 
│   oportunidades de IA y gestión de riesgos
├─ Incluye:
│   ├─ Sesiones de Alineamiento Estratégico
│   ├─ Talleres sobre Riesgos y Gobernanza de IA
│   └─ Exploración de Casos de Uso de Alto Impacto
└─ Button: "Solicitar Sesión de Descubrimiento"
```

### 6. Social Proof Section
```
H3: "Trusted by Global Innovators"
├─ Logos: STRATOS | NEXUS AI | FORGE.CO | VELOCITY | QUANTUM
└─ Efecto: Grayscale + hover para color (opacity-50 → opacity-100)
```

### 7. Final CTA Section (2 columnas)
```
Left (50%):
├─ H2: "¿Está su organización preparada para la siguiente etapa de la IA?"
├─ Descripción: "Iniciemos una conversación estratégica para identificar 
│   sus oportunidades de optimización y asegurar un despliegue responsable."
├─ Avatares de clientes (mock images)
└─ "Uniéndose a líderes en transformación IA"

Right (50%):
└─ Formulario de contacto:
    ├─ Nombre y Apellidos (required, text)
    ├─ Empresa / Cargo (required, text) [IMPORTANTE: Filtro C-Level]
    ├─ Email de Trabajo (required, email)
    ├─ ¿Cuál es su principal reto actual con la IA? (required, select/textarea)
    │   └─ Opciones: Estrategia / Gobernanza / Adopción / Procesos / Otro
    ├─ Mensaje adicional (optional, textarea, 4 rows)
    ├─ Consentimiento RGPD (checkbox required)
    └─ Button: "Solicitar Sesión de Descubrimiento" (bg-primary, full width)

Fondo: dark card (slate-900) con blur y border primary sutil
```

**Nota importante**: El campo Empresa/Cargo actúa como filtro pre-calificación. Incluye instrucción clara de que debe incluir cargo actual para sesión efectiva.

### 8. Footer
```
├─ Logo + Brand Name
├─ Links: Privacy Policy | Terms of Service | LinkedIn | Twitter
└─ Copyright: "© 2024 AI Strategy Lab. All rights reserved."
```

---

## ⚙️ FUNCIONALIDADES & COMPORTAMIENTO

### Navigation
- [x] Links anclados a IDs (#expertise, #about, #services, #contact)
- [x] Hover states (text-primary, transition-colors)
- [x] Mobile menu responsivo (hamburger en <768px)
- [x] Sticky header (top-0 z-50)

### Buttons & Interactions
- [x] Primarios: hover scale (transform hover:scale-105)
- [x] Secundarios: hover border color change
- [x] Focus states: ring-2 ring-primary/50
- [x] Transiciones suaves (transition-all, duración 200-300ms)

### Formulario de Contacto
```
Campos:
├─ Nombre y Apellidos (required, text)
├─ Empresa / Cargo (required, text)
│  └─ Placeholder: "Ej: Google / Director de Transformación Digital"
├─ Email de Trabajo (required, email)
├─ Principal Reto Actual con IA (required, select)
│  └─ Opciones:
│      ├─ Estrategia y Gobernanza
│      ├─ Adopción Organizacional
│      ├─ Optimización de Procesos
│      ├─ Otro
│      └─ Prefiero discutirlo
├─ Mensaje Adicional (optional, textarea, 4 rows)
│  └─ Placeholder: "Comparte más detalles sobre tu contexto..."
├─ Consentimiento RGPD (required, checkbox)
│  └─ "Acepto recibir comunicaciones sobre consultoría IA y gobernanza"
└─ Button: "Solicitar Sesión de Descubrimiento" (bg-primary)

Validación:
├─ Client-side: HTML5 validation + custom feedback
├─ Server-side: Backend validation (Antigravity)
└─ Mensaje de éxito: "¡Gracias! Te contactaremos en las próximas 48 horas para agendar tu sesión."

Envío:
├─ Email al consultor (Antonio)
├─ Auto-respuesta al cliente
└─ Almacenamiento: Base de datos Antigravity (encriptado)

**Pre-calificación**: El campo Empresa/Cargo es crítico para filtrar leads C-level
```

### Responsive Design
- [x] Mobile: 320px–640px (stacked layout)
- [x] Tablet: 768px–1024px (2 columnas)
- [x] Desktop: 1024px+ (full grid layout)
- [x] Test en: iPhone 12, iPad, Desktop 1920px

---

## 🔍 SEO & META TAGS

```html
<title>AI Governance & Strategic Transformation | AI Strategy Lab</title>
<meta name="description" content="Expert consulting for mid-sized organizations. 
AI Act, GDPR, ISO 42001 compliance. Strategic roadmaps, training, governance frameworks.">
<meta name="keywords" content="AI governance, AI adoption, AI Act, GDPR, 
mid-market consulting, strategic AI transformation">
<meta property="og:title" content="AI Strategy Lab | AI Governance Consulting">
<meta property="og:description" content="...">
<meta property="og:image" content="[hero image URL]">
<meta property="og:url" content="[site URL]">
<meta name="theme-color" content="#0db9f2">
```

**Estructura de headings**:
- H1: Uno por página (hero principal)
- H2: Secciones principales (4–5)
- H3: Subsecciones (si aplica)

**Schema markup**:
- Organization schema
- LocalBusiness schema (si se ofrece servicio local)
- FAQPage schema (futuro)

---

## ♿ ACCESIBILIDAD (WCAG 2.1 AA)

- [x] **Contraste**: Ratios ≥4.5:1 para texto, ≥3:1 para UI
- [x] **Focus visible**: Todos los botones/links con focus ring
- [x] **Keyboard navigation**: Tab, Shift+Tab, Enter para activar
- [x] **Alt text**: En todas las imágenes (decorativas: alt="")
- [x] **ARIA labels**: Botones solo-icono con aria-label
- [x] **Semantic HTML**: `<button>`, `<a>`, `<label>`, no `<div onClick>`
- [x] **Skip to main content**: Link en header (visible en focus)
- [x] **Form labels**: Linked via htmlFor o wrapping
- [x] **Color no es único**: No confiar solo en color para info

**Testing**:
- Usar WAVE, Axe DevTools, Lighthouse
- Target: Score >90

---

## 🔐 SEGURIDAD & COMPLIANCE

### RGPD (EU)
- [x] Formulario con checkbox de consentimiento (opt-in)
- [x] Enlace a Política de Privacidad en footer
- [x] Almacenamiento seguro (HTTPS, encriptación)
- [x] Email de respuesta con datos del usuario
- [x] Opción para solicitar "derecho a ser olvidado"

### Técnico
- [x] HTTPS obligatorio
- [x] Security headers (CSP, X-Frame-Options, HSTS)
- [x] Validación server-side en formularios
- [x] Rate limiting en formulario (prevenir spam)
- [x] Sanitización de inputs

---

## 📊 ANALYTICS & EVENTOS

**Google Analytics 4 (GA4)**:
- Evento: "book_a_session" (clic en CTA primario)
- Evento: "contact_form_submitted"
- Evento: "scroll_depth" (25%, 50%, 75%, 100%)
- Conversión: Contact form submission

**Hotjar** (optional):
- Heatmaps de secciones
- Session recordings (primeros 100 visitantes)
- Feedback widget (opcional)

---

## 📦 RECURSOS & REFERENCIAS

**Mockup proporcionado**: [Archivo screen.png adjunto]
**Código base**: [Archivo code.html adjunto]
**Design skill**: Usar "Vercel Design Skill" para validar:
- Paleta de colores
- Espaciado y tipografía
- Responsive breakpoints
- Componentes (botones, cards, formularios)

**Documentación útil**:
- Tailwind CSS: https://tailwindcss.com
- Material Symbols: https://fonts.google.com/icons
- Antigravity docs: [tu URL]

---

## ✅ CHECKLIST DE ENTREGABLES

### MVP (Semanas 4-6)
- [ ] Header responsivo + navegación funcional
- [ ] Hero section con copy + icono/mockup
- [ ] Value prop section (3 cards)
- [ ] Core expertise section (4 cards)
- [ ] Services section (3 cards, con "Most Popular" destacada)
- [ ] Social proof (logos)
- [ ] Final CTA + formulario
- [ ] Footer con links + copyright
- [ ] Formulario funcional (envío de email)
- [ ] Responsive en mobile/tablet/desktop
- [ ] Accesibilidad: WCAG 2.1 AA pass
- [ ] SEO básico: metas, schema, sitemap
- [ ] RGPD: Privacy policy link + consentimiento

### QA & Polish (Semanas 6-7)
- [ ] Test de todos los links
- [ ] Test del formulario (envío real)
- [ ] Lighthouse score >90 (Performance, Accessibility, Best Practices, SEO)
- [ ] Core Web Vitals: LCP <2.5s, FID <100ms, CLS <0.1
- [ ] Validación HTML/CSS sin errores críticos
- [ ] Testing en 5+ dispositivos reales
- [ ] Screenshots para documentación

### Deploy (Semana 8)
- [ ] Dominio personalizado configurado
- [ ] SSL certificate activo
- [ ] Analytics (GA4) configurado
- [ ] Email de contacto funcionando
- [ ] Backup automático habilitado
- [ ] Monitoreo de uptime activo

---

## 🎯 PRÓXIMOS PASOS

1. **Ahora**: Aprueba este prompt y el plan del proyecto
2. **Semana 1**: Crea proyecto en Antigravity, configura dominio
3. **Semana 2-3**: Construye header + hero + primeras secciones
4. **Semana 4**: Feedback y ajustes (usa Vercel Design Skill)
5. **Semana 5**: Integración de formulario + backend
6. **Semana 6**: Testing completo
7. **Semana 7**: Deploy + lanzamiento
8. **Semana 8+**: Analytics + iteraciones basadas en datos

---

## 💬 COMUNICACIÓN DURANTE EL PROYECTO

**Formato de feedback de Antonio**:
- Cambios de copy: Proporciona el nuevo texto (inglés + español si aplica)
- Cambios de diseño: Describe el cambio + proporciona referencias visuales
- Funcionalidad: Detalla qué esperas que haga + casos de uso
- Prioridad: Marca como CRÍTICO, IMPORTANTE, o NICE-TO-HAVE

**Formato de entregables**:
- Screenshots de cada sección completada
- Links a secciones implementadas (mobile + desktop)
- Notas técnicas (cambios, decisiones de diseño)
- Bloqueadores/preguntas claras

---

## 📝 NOTAS FINALES

- **Tono**: Profesional, consultivo, empoderante (no salesy)
- **Idioma**: Inglés para web (versión español futura)
- **Diferenciación**: Enfoque en **gobernanza + adopción**, frameworks regulatorios (AI Act, GDPR, ISO)
- **Público**: C-suite en PYMES (200–500 empleados) en EU
- **Objetivo**: Generar leads cualificados para sesiones de estrategia
- **Futuro**: Fase 2 incluirá blog, casos de estudio, recursos descargables

---

**¿Listo para empezar? ¡Vamos! 🚀**
