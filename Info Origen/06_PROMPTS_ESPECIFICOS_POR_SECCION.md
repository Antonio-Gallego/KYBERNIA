# 📝 PROMPTS ESPECÍFICOS POR SECCIÓN (Copy-Paste Listo)

Usa este documento cuando construyas cada sección en Antigravity. Todos los textos están aquí + HTML específico por sección.

---

## SECCIÓN 1: HEADER (Ya construida - referencia)

**Status**: ✅ COMPLETADA Day 1

```html
<header class="sticky top-0 z-50 w-full border-b border-slate-200 dark:border-slate-800 bg-background-light/80 dark:bg-background-dark/80 backdrop-blur-md">
  <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
    <div class="flex items-center gap-3">
      <div class="bg-primary p-1.5 rounded-lg">
        <span class="material-symbols-outlined text-background-dark text-2xl font-bold">insights</span>
      </div>
      <h2 class="text-xl font-bold tracking-tight">AI Strategy Lab</h2>
    </div>
    <nav class="hidden md:flex items-center gap-10">
      <a class="text-sm font-medium hover:text-primary transition-colors" href="#propuesta">Propuesta</a>
      <a class="text-sm font-medium hover:text-primary transition-colors" href="#pilares">Pilares</a>
      <a class="text-sm font-medium hover:text-primary transition-colors" href="#servicios">Servicios</a>
      <a class="text-sm font-medium hover:text-primary transition-colors" href="#contacto">Contacto</a>
    </nav>
    <button class="bg-primary hover:bg-primary/90 text-background-dark text-sm font-bold py-2.5 px-6 rounded-lg transition-all transform hover:scale-105">
      Solicitar Sesión
    </button>
  </div>
</header>
```

---

## SECCIÓN 2: HERO (Ya construida - referencia)

**Status**: ✅ COMPLETADA Day 1

**Principales elementos**:
- Titular con color primario en "Segura y Estratégica"
- Subtítulo descriptivo (40 palabras)
- 2 botones: primario + secundario
- Glass card con 3 iconos (Gobernanza, Personas, Procesos)

---

## SECCIÓN 3: VALUE PROPOSITION

**Status**: ⏳ Day 2 - Lunes

**Anchor ID**: `id="propuesta"`

### Copy Exacto:

**Titular H2:**
```
La IA no es un Proyecto Tecnológico, es una Evolución Organizacional
```

**Cita Destacada (en card con border-left primary):**
```
"Ayudo a las empresas a navegar la complejidad del ecosistema 
de la IA mediante un enfoque integral que garantiza que cada 
implementación sea segura, ética y, sobre todo, generadora de 
resultados medibles."
```

**Párrafo de Contexto:**
```
La verdadera transformación no ocurre en los servidores, sino en 
la cultura de la empresa. Por ello, pongo la gestión del cambio y 
el desarrollo de las personas en el centro de la adopción 
tecnológica.
```

### HTML Específico:

```html
<!-- Value Proposition Section -->
<section class="py-24 bg-slate-50 dark:bg-background-dark/50" id="propuesta">
  <div class="container mx-auto px-6">
    <div class="max-w-3xl mb-16">
      <h2 class="text-3xl lg:text-4xl font-bold mb-6">
        La IA no es un Proyecto Tecnológico, es una Evolución Organizacional
      </h2>
      
      <!-- Cita destacada -->
      <div class="bg-white dark:bg-slate-900 border-l-4 border-primary p-6 rounded-lg mb-8">
        <p class="text-lg italic text-slate-700 dark:text-slate-300">
          "Ayudo a las empresas a navegar la complejidad del ecosistema de la IA mediante un 
          enfoque integral que garantiza que cada implementación sea segura, ética y, sobre 
          todo, generadora de resultados medibles."
        </p>
      </div>
      
      <p class="text-lg text-slate-500 dark:text-slate-400 leading-relaxed">
        La verdadera transformación no ocurre en los servidores, sino en la cultura de la empresa. 
        Por ello, pongo la gestión del cambio y el desarrollo de las personas en el centro de la 
        adopción tecnológica.
      </p>
    </div>
  </div>
</section>
```

---

## SECCIÓN 4: CORE EXPERTISE - 3 PILARES

**Status**: ⏳ Day 2 - Martes

**Anchor ID**: `id="pilares"`

### Copy Exacto por Pilar:

**PILAR I: Estrategia y Gobernanza Sólida**
```
Definición Estratégica
Alineamiento de la IA con los objetivos macro de la organización.

Modelos Operativos y Organizativos
Diseño de estructuras que permitan escalar la IA con control.

Políticas de Uso y Cumplimiento
Establecimiento de guías claras de uso y alineamiento con 
requerimientos regulatorios (EU AI Act, GDPR).

IA Responsable
Marcos éticos para mitigar riesgos y asegurar la transparencia.
```

**PILAR II: Cultura, Personas y AI-Fluency**
```
Evolución de Roles
Identificación y diseño de los nuevos perfiles profesionales necesarios.

Programas de AI-Fluency
Formación técnica y funcional para elevar las capacidades del equipo.

Gestión del Cambio Cultural
Transformación de la mentalidad organizacional para una adopción 
natural y sin fricciones.

AI Champions
Creación de redes internas de expertos para traccionar la innovación.
```

**PILAR III: Optimización de Procesos e Innovación**
```
Más Allá de las Herramientas
Enfoque en la reingeniería de procesos para una eficiencia real.

Mejora Continua e Innovación
Aplicación de IA para optimizar flujos de trabajo existentes 
y crear nuevos modelos de valor.

Medición del Impacto (ROI)
Establecimiento de KPIs para validar que la innovación se traduce 
en rentabilidad.
```

### HTML Específico:

```html
<!-- Core Expertise - 3 Pilares -->
<section class="py-24" id="pilares">
  <div class="container mx-auto px-6">
    <div class="text-center max-w-2xl mx-auto mb-16">
      <h2 class="text-3xl lg:text-4xl font-bold mb-4">Los Tres Pilares de la Transformación de IA</h2>
    </div>
    
    <div class="grid md:grid-cols-3 gap-8">
      
      <!-- PILAR I -->
      <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 border-l-4 border-l-primary hover:shadow-xl transition-all">
        <h3 class="text-xl font-bold mb-6 text-primary">Estrategia y Gobernanza Sólida</h3>
        
        <div class="space-y-4 text-sm text-slate-600 dark:text-slate-400">
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Definición Estratégica</h4>
            <p>Alineamiento de la IA con los objetivos macro de la organización.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Modelos Operativos y Organizativos</h4>
            <p>Diseño de estructuras que permitan escalar la IA con control.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Políticas de Uso y Cumplimiento</h4>
            <p>Establecimiento de guías claras de uso y alineamiento con requerimientos regulatorios (EU AI Act, GDPR).</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">IA Responsable</h4>
            <p>Marcos éticos para mitigar riesgos y asegurar la transparencia.</p>
          </div>
        </div>
      </div>
      
      <!-- PILAR II -->
      <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 border-l-4 border-l-primary hover:shadow-xl transition-all">
        <h3 class="text-xl font-bold mb-6 text-primary">Cultura, Personas y AI-Fluency</h3>
        
        <div class="space-y-4 text-sm text-slate-600 dark:text-slate-400">
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Evolución de Roles</h4>
            <p>Identificación y diseño de los nuevos perfiles profesionales necesarios.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Programas de AI-Fluency</h4>
            <p>Formación técnica y funcional para elevar las capacidades del equipo.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Gestión del Cambio Cultural</h4>
            <p>Transformación de la mentalidad organizacional para una adopción natural y sin fricciones.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">AI Champions</h4>
            <p>Creación de redes internas de expertos para traccionar la innovación.</p>
          </div>
        </div>
      </div>
      
      <!-- PILAR III -->
      <div class="bg-white dark:bg-slate-900 p-8 rounded-2xl border border-slate-200 dark:border-slate-800 border-l-4 border-l-primary hover:shadow-xl transition-all">
        <h3 class="text-xl font-bold mb-6 text-primary">Optimización de Procesos e Innovación</h3>
        
        <div class="space-y-4 text-sm text-slate-600 dark:text-slate-400">
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Más Allá de las Herramientas</h4>
            <p>Enfoque en la reingeniería de procesos para una eficiencia real.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Mejora Continua e Innovación</h4>
            <p>Aplicación de IA para optimizar flujos de trabajo existentes y crear nuevos modelos de valor.</p>
          </div>
          <div>
            <h4 class="font-semibold text-slate-900 dark:text-white mb-1">Medición del Impacto (ROI)</h4>
            <p>Establecimiento de KPIs para validar que la innovación se traduce en rentabilidad.</p>
          </div>
        </div>
      </div>
      
    </div>
  </div>
</section>
```

---

## SECCIÓN 5: SERVICIOS (3 Packs)

**Status**: ⏳ Day 3 - Miércoles

**Anchor ID**: `id="servicios"`

### Copy Exacto por Servicio:

**SERVICIO 1: Diagnóstico de Madurez y Gobernanza de IA**
```
Análisis profundo de tu posición actual en gobernanza, 
regulación y preparación tecnológica/organizacional.

INCLUYE:
• Evaluación de Marco Gobernanza Actual
• Análisis de Cumplimiento (EU AI Act, GDPR)
• Evaluación de Capacidades de Personas
• Identificación de Quick Wins
```

**SERVICIO 2 (DESTACADO): Programa de Transformación Integral**
```
Acompañamiento de 6-12 meses con gobernanza, upskilling, 
reingeniería de procesos y medición de ROI.

INCLUYE:
• Definición de Estrategia y Gobernanza
• Diseño de Modelos Operativos
• Programas de AI-Fluency y Change Management
• Identificación de Casos de Uso de Alto Impacto
• Framework de Medición de ROI
```

**SERVICIO 3: Sesiones Estratégicas Ejecutivas**
```
Talleres intensivos para C-suite sobre gobernanza, 
oportunidades de IA y gestión de riesgos.

INCLUYE:
• Sesiones de Alineamiento Estratégico
• Talleres sobre Riesgos y Gobernanza de IA
• Exploración de Casos de Uso de Alto Impacto
• Diseño de Roadmap de Corto Plazo
```

### HTML Específico:

```html
<!-- Services Section -->
<section class="py-24 bg-slate-100 dark:bg-slate-900/40" id="servicios">
  <div class="container mx-auto px-6">
    <div class="text-center max-w-2xl mx-auto mb-16">
      <h2 class="text-3xl lg:text-4xl font-bold mb-4">Servicios de Consultoría Estratégica</h2>
      <p class="text-slate-500 dark:text-slate-400">
        Engagements estructurados para llevar tu organización desde la curiosidad inicial 
        hasta la adopción integral y sostenible de IA.
      </p>
    </div>
    
    <div class="grid md:grid-cols-3 gap-8">
      
      <!-- SERVICIO 1 -->
      <div class="bg-white dark:bg-background-dark p-8 rounded-2xl border border-slate-200 dark:border-slate-800 flex flex-col h-full shadow-sm hover:shadow-xl transition-all">
        <h3 class="text-xl font-bold mb-4">Diagnóstico de Madurez y Gobernanza de IA</h3>
        <p class="text-slate-500 dark:text-slate-400 mb-8 flex-grow">
          Análisis profundo de tu posición actual en gobernanza, regulación y preparación 
          tecnológica/organizacional.
        </p>
        <ul class="space-y-3 mb-8">
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Evaluación de Marco Gobernanza Actual
          </li>
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Análisis de Cumplimiento (EU AI Act, GDPR)
          </li>
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Evaluación de Capacidades de Personas
          </li>
        </ul>
        <button class="w-full py-3 rounded-lg border border-primary text-primary font-bold hover:bg-primary hover:text-background-dark transition-all">
          Solicitar Sesión de Descubrimiento
        </button>
      </div>
      
      <!-- SERVICIO 2 - DESTACADO -->
      <div class="bg-white dark:bg-background-dark p-8 rounded-2xl border-2 border-primary flex flex-col h-full shadow-2xl transform scale-105 z-10">
        <div class="absolute -top-4 left-1/2 -translate-x-1/2 bg-primary text-background-dark px-4 py-1 rounded-full text-xs font-black uppercase">
          Más Popular
        </div>
        <h3 class="text-xl font-bold mb-4">Programa de Transformación Integral</h3>
        <p class="text-slate-500 dark:text-slate-400 mb-8 flex-grow">
          Acompañamiento de 6-12 meses con gobernanza, upskilling, reingeniería de procesos 
          y medición de ROI.
        </p>
        <ul class="space-y-3 mb-8">
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Definición de Estrategia y Gobernanza
          </li>
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Diseño de Modelos Operativos
          </li>
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Programas de AI-Fluency y Change Management
          </li>
        </ul>
        <button class="w-full py-3 rounded-lg bg-primary text-background-dark font-bold hover:bg-primary/90 transition-all">
          Solicitar Sesión de Descubrimiento
        </button>
      </div>
      
      <!-- SERVICIO 3 -->
      <div class="bg-white dark:bg-background-dark p-8 rounded-2xl border border-slate-200 dark:border-slate-800 flex flex-col h-full shadow-sm hover:shadow-xl transition-all">
        <h3 class="text-xl font-bold mb-4">Sesiones Estratégicas Ejecutivas</h3>
        <p class="text-slate-500 dark:text-slate-400 mb-8 flex-grow">
          Talleres intensivos para C-suite sobre gobernanza, oportunidades de IA 
          y gestión de riesgos.
        </p>
        <ul class="space-y-3 mb-8">
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Sesiones de Alineamiento Estratégico
          </li>
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Talleres sobre Riesgos y Gobernanza de IA
          </li>
          <li class="flex items-center gap-2 text-sm text-slate-600 dark:text-slate-400">
            <span class="material-symbols-outlined text-primary text-lg">check_circle</span> 
            Exploración de Casos de Uso
          </li>
        </ul>
        <button class="w-full py-3 rounded-lg border border-primary text-primary font-bold hover:bg-primary hover:text-background-dark transition-all">
          Solicitar Sesión de Descubrimiento
        </button>
      </div>
      
    </div>
  </div>
</section>
```

---

## SECCIÓN 6: SOCIAL PROOF

**Status**: ⏳ Day 3 - Viernes

### Copy Exacto:

```
Confiado por Líderes en Transformación Digital
```

### HTML Específico (Logos Mock):

```html
<!-- Social Proof Section -->
<section class="py-16 border-b border-slate-200 dark:border-slate-800">
  <div class="container mx-auto px-6 text-center">
    <p class="text-xs font-bold uppercase tracking-[0.3em] text-slate-400 mb-10">
      Confiado por Líderes en Transformación Digital
    </p>
    <div class="flex flex-wrap justify-center items-center gap-12 md:gap-20 opacity-60 grayscale hover:grayscale-0 transition-all duration-500">
      <span class="text-2xl font-black text-slate-800 dark:text-slate-200">Telefónica</span>
      <span class="text-2xl font-black text-slate-800 dark:text-slate-200">BBVA</span>
      <span class="text-2xl font-black text-slate-800 dark:text-slate-200">Inditex</span>
      <span class="text-2xl font-black text-slate-800 dark:text-slate-200">Mapfre</span>
      <span class="text-2xl font-black text-slate-800 dark:text-slate-200">Endesa</span>
    </div>
  </div>
</section>
```

---

## SECCIÓN 7: FINAL CTA + FORMULARIO

**Status**: ⏳ Day 4 - Próximo lunes

**Anchor ID**: `id="contacto"`

### Copy Exacto:

**Titular:**
```
¿Está su Organización Preparada para la Siguiente Etapa de la IA?
```

**Descripción:**
```
Iniciemos una conversación estratégica para identificar sus oportunidades 
de optimización y asegurar un despliegue responsable.
```

**Campos del Formulario:**
```
1. Nombre y Apellidos (required, text)
2. Empresa / Cargo (required, text)
   Ej: "Google / Director de Transformación Digital"
3. Email de Trabajo (required, email)
4. ¿Cuál es su principal reto actual con la IA? (required, select)
   - Estrategia y Gobernanza
   - Adopción Organizacional
   - Optimización de Procesos
   - Otro
   - Prefiero discutirlo
5. Mensaje Adicional (optional, textarea)
6. Consentimiento RGPD (required, checkbox)
   "Acepto recibir comunicaciones sobre consultoría IA y gobernanza"

CTA Button: "Solicitar Sesión de Descubrimiento"
```

### HTML Específico:

```html
<!-- Final CTA Section -->
<footer class="pt-24 pb-12 bg-background-light dark:bg-background-dark" id="contacto">
  <div class="container mx-auto px-6">
    <div class="grid lg:grid-cols-2 gap-16 mb-20 items-center bg-slate-900 rounded-[2rem] p-12 overflow-hidden relative">
      <div class="absolute right-0 top-0 w-1/2 h-full bg-primary/10 blur-[120px] pointer-events-none"></div>
      
      <!-- Left Column -->
      <div>
        <h2 class="text-4xl lg:text-5xl font-bold text-white mb-6">
          ¿Está su Organización Preparada para la Siguiente Etapa de la IA?
        </h2>
        <p class="text-slate-400 text-lg mb-10">
          Iniciemos una conversación estratégica para identificar sus oportunidades 
          de optimización y asegurar un despliegue responsable.
        </p>
      </div>
      
      <!-- Right Column - Form -->
      <div class="bg-white/5 backdrop-blur-md rounded-2xl p-8 border border-white/10">
        <form class="space-y-4">
          
          <div class="grid grid-cols-2 gap-4">
            <input 
              class="bg-background-dark/50 border border-slate-700 text-white rounded-lg focus:ring-2 focus:ring-primary focus:border-primary w-full p-3" 
              placeholder="Nombre" 
              type="text"
              required
            />
            <input 
              class="bg-background-dark/50 border border-slate-700 text-white rounded-lg focus:ring-2 focus:ring-primary focus:border-primary w-full p-3" 
              placeholder="Apellidos" 
              type="text"
              required
            />
          </div>
          
          <input 
            class="bg-background-dark/50 border border-slate-700 text-white rounded-lg focus:ring-2 focus:ring-primary focus:border-primary w-full p-3" 
            placeholder="Empresa / Cargo (Ej: Google / Director de Transformación)" 
            type="text"
            required
          />
          
          <input 
            class="bg-background-dark/50 border border-slate-700 text-white rounded-lg focus:ring-2 focus:ring-primary focus:border-primary w-full p-3" 
            placeholder="Email de Trabajo" 
            type="email"
            required
          />
          
          <select 
            class="bg-background-dark/50 border border-slate-700 text-white rounded-lg focus:ring-2 focus:ring-primary focus:border-primary w-full p-3"
            required
          >
            <option value="">¿Cuál es su principal reto actual con la IA?</option>
            <option value="estrategia">Estrategia y Gobernanza</option>
            <option value="adopcion">Adopción Organizacional</option>
            <option value="procesos">Optimización de Procesos</option>
            <option value="otro">Otro</option>
            <option value="discutir">Prefiero discutirlo</option>
          </select>
          
          <textarea 
            class="bg-background-dark/50 border border-slate-700 text-white rounded-lg focus:ring-2 focus:ring-primary focus:border-primary w-full p-3" 
            placeholder="Mensaje adicional (opcional)" 
            rows="3"
          ></textarea>
          
          <label class="flex items-center gap-3 text-sm text-slate-300">
            <input type="checkbox" required class="w-4 h-4 rounded" />
            <span>Acepto recibir comunicaciones sobre consultoría IA y gobernanza</span>
          </label>
          
          <button 
            type="submit"
            class="w-full bg-primary text-background-dark font-bold py-4 rounded-lg hover:bg-primary/90 transition-all shadow-xl shadow-primary/20"
          >
            Solicitar Sesión de Descubrimiento
          </button>
          
        </form>
      </div>
      
    </div>
    
    <!-- Footer Links -->
    <div class="flex flex-col md:flex-row justify-between items-center border-t border-slate-200 dark:border-slate-800 pt-12">
      <div class="flex items-center gap-3 mb-8 md:mb-0">
        <div class="bg-primary p-1 rounded-lg">
          <span class="material-symbols-outlined text-background-dark text-xl font-bold">insights</span>
        </div>
        <h2 class="text-lg font-bold">AI Strategy Lab</h2>
      </div>
      <div class="flex gap-8 text-sm text-slate-500">
        <a class="hover:text-primary transition-colors" href="#privacidad">Política de Privacidad</a>
        <a class="hover:text-primary transition-colors" href="#terminos">Términos de Servicio</a>
        <a class="hover:text-primary transition-colors" href="#">LinkedIn</a>
        <a class="hover:text-primary transition-colors" href="#">Twitter</a>
      </div>
      <p class="text-xs text-slate-500 mt-8 md:mt-0">
        © 2025 AI Strategy Lab. Todos los derechos reservados.
      </p>
    </div>
  </div>
</footer>
```

---

## REFERENCIA RÁPIDA: Orden de Construcción

```
DÍA 1 (Monday):
☐ Header
☐ Hero

DÍA 2 (Martes-Miércoles):
☐ Value Proposition
☐ Core Expertise (3 Pilares)

DÍA 3 (Jueves-Viernes):
☐ Services
☐ Social Proof

DÍA 4 (Próximo Lunes):
☐ Final CTA + Formulario
☐ Footer
```

---

**Cada sección tiene**: 
- ✅ Copy exacto (no necesitas pensar en palabras)
- ✅ HTML listo para copiar-pegar
- ✅ Anchor IDs para navegación
- ✅ Clases Tailwind apropiadas
- ✅ Iconos Material Symbols especificados

**Solo copia + pega + adapta a tu Antigravity setup.**
