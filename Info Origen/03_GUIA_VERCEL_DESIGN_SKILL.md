# 🎨 Guía: Usando Vercel Design Skill para Iterar

Esta guía te ayuda a obtener el máximo valor de la **Vercel Design Skill** durante el desarrollo de tu sitio.

---

## ¿QUÉ HACE LA VERCEL DESIGN SKILL?

La Vercel Design Skill analiza código HTML/CSS y valida contra:
1. **Paleta de colores**: Contraste, consistencia, accesibilidad
2. **Tipografía**: Escala, weights, legibilidad
3. **Espaciado & Layout**: Sistema de 8px, alineación, responsive
4. **Componentes**: Botones, cards, formularios, inputs
5. **Responsive design**: Breakpoints, mobile-first
6. **Accesibilidad**: WCAG 2.1, focus states, aria labels
7. **Performance**: Imágenes, lazy-loading, transiciones

---

## FLUJO DE TRABAJO RECOMENDADO

### Paso 1: Después de cada sección completada
```
Tu cliente (Antonio) → Antigravity
├─ Copia el HTML/CSS de la sección
└─ Envía a Claude: "Valida esta sección con la Vercel Design Skill"

Claude → Vercel Skill
├─ Revisa contra guidelines
└─ Reporta: ✓ OK, ⚠️ Advertencias, ❌ Errores críticos

Resultado:
├─ List de issues encontrados
├─ Sugerencias de fix
└─ Ranking por prioridad (Crítico → Important → Nice-to-have)
```

### Paso 2: Solicitar validación específica
```
Antonio → Claude:
"Valida [sección] contra estas reglas de Vercel:
1. Contraste WCAG AA (4.5:1 mínimo)
2. Responsive: 320px, 768px, 1024px
3. Focus states en botones
4. Performance: no transition: all"

Claude → Vercel Skill
└─ Revisa solo esos aspectos, más detallado
```

### Paso 3: Después de un A/B test
```
Antonio → Claude:
"Tengo dos versiones de [componente]:
Versión A: [código]
Versión B: [código]
¿Cuál cumple mejor las reglas de Vercel?"

Claude → Vercel Skill
└─ Compara ambas, reporta ventajas/desventajas
```

---

## MOMENTO IDEAL PARA VALIDAR

| Momento | Qué validar | Frecuencia |
|---------|------------|-----------|
| **Después de estructura HTML** | Semántica, accesibilidad, ARIA | Inmediato |
| **Después de styling inicial** | Colores, contraste, tipografía | Inmediato |
| **Después de componentes** | Botones, cards, formularios | Cada componente |
| **Después de responsive** | Breakpoints, mobile-first | Cada sección |
| **Antes de testing QA** | Todo (análisis completo) | 1x |
| **Antes de deploy** | Último pass (WCAG, perf) | 1x |

---

## EJEMPLOS DE CONSULTAS EFECTIVAS

### ✓ BUENAS CONSULTAS

**1. "Valida esta tarjeta de servicio contra Vercel Design Skill"**
```html
<div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200">
  <h3>AI Readiness Assessment</h3>
  <p>A deep-dive audit...</p>
  <button class="py-3 rounded-lg">Select Plan</button>
</div>
```
→ Claude validará semántica, colores, espaciado, botón

**2. "¿Este componente cumple WCAG AA? Revisa:"**
```html
<button class="bg-primary text-white">Book Session</button>
```
→ Claude verificará:
- Contraste #0db9f2 vs #ffffff = ~4.2:1 ✓
- Focus state presente/ausente
- ARIA label si es icon-only

**3. "Compara estos dos botones contra Vercel Design Skill"**
- Opción A: `bg-primary hover:bg-primary/90 py-3 px-6`
- Opción B: `bg-primary hover:scale-105 py-3 px-6`
→ Claude dirá cuál es más accesible, performante, etc.

**4. "¿Esta paleta de colores tiene suficiente contraste?"**
```
Primario: #0db9f2
Secundario: #101e22
Fondo claro: #f5f8f8
```
→ Claude calcula ratios y avisa si hay issues

### ✗ CONSULTAS VAGAS (EVITAR)

❌ "¿Cómo se ve esto?"
→ Muy subjetivo, no es validación contra guidelines

❌ "¿Me gusta este diseño?"
→ Opinion-based, no checklist objective

❌ "Haz que se vea mejor"
→ Sin criterios claros, múltiples interpretaciones

❌ "Revisa todo"
→ Demasiado amplio, mejor seccionar

---

## CHECKLIST DE ASPECTOS A VALIDAR

Usa esto como referencia para solicitar validaciones puntuales:

### Accesibilidad
- [ ] Ratios de contraste ≥4.5:1 (texto), ≥3:1 (UI)
- [ ] Focus visible en botones/links (ring-* o outline)
- [ ] ARIA labels en botones icon-only
- [ ] Semantic HTML (`<button>` no `<div onClick>`)
- [ ] Form labels linked (htmlFor)
- [ ] Headings jerárquicos (H1 → H2 → H3)

### Tipografía
- [ ] Escala consistente (Inter, weights: 400/500/600/700/800)
- [ ] Línea-altura adecuada (1.5–1.6 para body)
- [ ] Tamaño mínimo 16px (mobile)
- [ ] Contraste suficiente (4.5:1)

### Espaciado & Layout
- [ ] Sistema de 8px respetado (p-2, p-4, p-8, etc.)
- [ ] Máximo ancho (max-w-7xl)
- [ ] Grid/Flex correctos (md:grid-cols-3, etc.)
- [ ] Padding/margin balanceado

### Colores
- [ ] Primario: #0db9f2 OK en botones, accents
- [ ] Secundario: #101e22 OK para fondos oscuros
- [ ] Grises: Escalada consistente (slate-100 → slate-900)
- [ ] Modo oscuro: Todos los colores testeados

### Responsive
- [ ] Mobile: 320px–640px (stacked, full-width)
- [ ] Tablet: 768px–1024px (2 columnas)
- [ ] Desktop: 1024px+ (full layout)
- [ ] No scrolling horizontal

### Componentes
- [ ] Botones: Primario, secundario, estados (hover, active, focus)
- [ ] Cards: Sombra, border, hover effect
- [ ] Formulario: Labels, inputs validados, error states
- [ ] Icons: Tamaño consistente, color primario

### Performance
- [ ] `transition: all` → specific properties (transform, opacity)
- [ ] Imágenes: lazy-loading para below-fold
- [ ] Animations: respetar prefers-reduced-motion
- [ ] Font loading: display=swap

---

## CÓMO SOLICITAR VALIDACIÓN EN LA PRÁCTICA

### Formato recomendado:

```markdown
## Validación: [Nombre de sección]

**Sección**: Hero
**Estado**: Primera iteración
**Cambios**: Agregué glass-card con iconos

**Código**:
[copiar HTML/CSS aquí]

**Preguntas específicas**:
1. ¿Contraste OK en el título sobre fondo gradiente?
2. ¿Focus states listos en botones?
3. ¿Mobile responsive en 320px?

**Prioridad**: IMPORTANTE (bloquea a siguiente sección)

**Resultado esperado**:
- ✓ Lista de issues (críticos first)
- ✓ Sugerencias de fix (código específico)
- ✓ Referencias a reglas Vercel (link o nombre)
```

### Ejemplos en acción:

**Ejemplo 1: Validación de color**
```
## Validación: Contraste de titulares

Tengo:
- Titular: blanco (#ffffff)
- Fondo: gradiente dark (#101e22 → #0db9f2)

¿El contraste en la zona donde gradiente es más claro OK?
Usa Vercel Design Skill para verificar.
```

**Ejemplo 2: Validación de componente**
```
## Validación: Botón primario

Código actual:
<button class="bg-primary hover:bg-primary/90 py-3 px-6 rounded-lg transition-all">
  Book a Session
</button>

Revisa:
1. ¿Contraste OK? (#0db9f2 sobre blanco)
2. ¿Focus state visible?
3. ¿Transición OK (no transition: all)?
4. ¿Accesible sin label?
```

**Ejemplo 3: Validación comparativa**
```
## Validación: Dos versiones de card

Versión A: bg-white dark:bg-slate-900 rounded-2xl shadow-lg
Versión B: bg-white dark:bg-slate-900 rounded-xl shadow-md

¿Cuál cumple mejor Vercel guidelines para:
- Espaciado?
- Sombra (depth)?
- Responsive?
```

---

## INTERPRETANDO RESULTADOS DE VERCEL

Cuando Claude reporta usando Vercel Design Skill:

### ✓ TODO OK
```
Hero Section
✓ Semantic HTML correct
✓ Contrast ratios WCAG AA
✓ Focus states visible
✓ Responsive layout OK
✓ Performance: no issues
```
→ **Acción**: Procede a siguiente sección

### ⚠️ ADVERTENCIAS (Important)
```
Value Prop Cards
✓ Layout OK
⚠️ Hover state on cards could be more prominent
⚠️ Icon size (24px) vs body (16px) - ratio could be larger
✓ Contrast OK
```
→ **Acción**: Mejora pero no bloqueante. Agenda para siguiente iteración.

### ❌ CRÍTICO (Bloqueante)
```
Final CTA Section
❌ Form input contrast: #0db9f2 on #101e22 = 2.1:1 (min 4.5:1)
❌ Submit button: no focus state (outline-none sin replacement)
⚠️ Form labels not properly associated
```
→ **Acción**: Fix antes de proceder. Proporciona código actualizado para re-validar.

---

## ITERACIÓN TÍPICA

### Ciclo de 1 semana:

**Lunes–Martes**: Construyes una sección (HTML + CSS)
```
Antonio → Claude:
"Terminé [sección]. Valida con Vercel Design Skill."
```

**Martes–Miércoles**: Claude valida
```
Claude:
"[Sección] tiene 2 issues críticos:
1. Contraste en X
2. Focus state falta

Sugerencias [código específico]"
```

**Miércoles–Jueves**: Corriges + re-validas
```
Antonio:
"Actualicé. Aquí está el código nuevo. Re-valida?"

Claude:
"✓ Todos los issues resolvidos. Procede a siguiente."
```

**Viernes**: Feedback visual + UX testing
```
Antonio:
"¿Cómo se ve en mobile/tablet? Feedback de amigos."

Claude:
"Basado en feedback, sugiero [changes]"
```

---

## TIPS PARA MAXIMIZAR VALOR

### 1. Sección por sección
No envíes todo el HTML de golpe. Valida cada sección completada.

### 2. Código limpio
Antes de validar, asegúrate de que el código está bien formateado.
```
❌ <button class="bg-primary  py-3  px-6">
✓ <button class="bg-primary py-3 px-6">
```

### 3. Contexto claro
Siempre menciona:
- Qué sección es
- Qué cambios hiciste
- Qué aspecto validas

### 4. Seguimiento
Si Claude reporta 5 issues, no ignores los "Important". Agenda fix.

### 5. Documentar decisiones
Si decides NO seguir una sugerencia, documéntalo:
```
Vercel sugirió: Aumentar tamaño de icono a 32px
Decisión: Mantener en 24px (consistencia con Material Symbols)
```

---

## CUÁNDO ESCALAR A VERCEL DESIGN SKILL

**SÍ, usa Vercel Design Skill para**:
- ✓ Validaciones de accesibilidad (contraste, focus)
- ✓ Componentización (botones, cards, forms)
- ✓ Responsive breakpoints
- ✓ Colores & tipografía
- ✓ Comparaciones de dos opciones
- ✓ Performance (transiciones, imágenes)

**NO necesitas Vercel Design Skill para**:
- ✗ Cambios de copy/texto
- ✗ Opiniones sobre colores (es subjetivo)
- ✗ Decisiones de contenido
- ✗ Estructura de la empresa

---

## RECURSOS DE REFERENCIA

- **Vercel Design Docs**: https://vercel.com/design
- **WCAG 2.1 Contrast Checker**: https://webaim.org/resources/contrastchecker/
- **Tailwind CSS**: https://tailwindcss.com (referencia de utilidades)
- **Material Design Icons**: https://fonts.google.com/icons
- **Lighthouse**: Chrome DevTools → Lighthouse

---

## PRÓXIMA SEMANA: ACCIÓN

Cuando empieces con Antigravity:

1. **Primero**: Manda el header/navigation
   → Claude valida con Vercel Design Skill
   → Recibe feedback
   → Itera

2. **Luego**: Hero section
   → Validación
   → Feedback

3. **Patrón**: Sección → Validación → Iterate → Merge

---

**¿Listo? ¡Comienza con la sección que tengas más clara y valida!** 🚀
