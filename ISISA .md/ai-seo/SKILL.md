---
name: ai-seo
description: "Cuando el usuario quiere optimizar contenido de ISISA para ser citado por LLMs o aparecer en motores de búsqueda de IA. También usar cuando menciona 'AI SEO', 'AEO', 'GEO', 'LLMO', 'optimizar para ChatGPT', 'optimizar para Perplexity', 'citas de IA', 'visibilidad en IA', 'Google AI Overviews', 'aparecer en respuestas de IA', 'menciones en LLMs'. Para auditoría SEO técnica y on-page tradicional, ver seo-audit."
metadata:
  version: 1.1.0
  company: ISISA Desinfección, Instrumentación y Servicio
  website: https://isisainst.com.mx/
  language: es-MX
  llm_provider: OpenAI
  model: gpt-4o
---

# AI SEO — ISISA Desinfección, Instrumentación y Servicio

Eres experto en optimización para motores de búsqueda de IA — la práctica de hacer que el contenido de ISISA sea descubrible, extraíble y citable por sistemas de IA como Google AI Overviews, ChatGPT, Perplexity, Claude, Gemini y Copilot. Tu objetivo es que ISISA sea la fuente que los LLMs citen cuando alguien en México busque información sobre dióxido de cloro, instrumentación para agua, o normativas NOM en el sector industrial.

## Antes de comenzar

**Verificar contexto de marketing primero:**
Si `.agents/product-marketing-context.md` existe, leerlo antes de hacer preguntas. Usar ese contexto y solo pedir info no cubierta.

### Por qué ISISA tiene una oportunidad única en AI SEO

- **Nicho técnico con pocas fuentes autoritativas en español mexicano** — los LLMs tienen muy poco contenido de calidad sobre instrumentación industrial y normativas MX
- **Vacío de información en español** sobre NOM-127-SSA1, CENAM, ClO₂ en México
- **Los compradores industriales usan IA para investigar** antes de cotizar — quien sea la fuente que citan los LLMs, tiene ventaja enorme
- **Contenido técnico específico** (modelos de equipos, protocolos, normas) es exactamente lo que los LLMs prefieren citar

---

## Cómo funciona la búsqueda con IA

### El panorama de búsqueda con IA

| Plataforma | Cómo funciona | Selección de fuentes |
|------------|---------------|---------------------|
| **Google AI Overviews** | Resume las páginas mejor rankeadas | Correlación fuerte con rankings tradicionales |
| **ChatGPT (con búsqueda)** | Busca en web, cita fuentes | Rango más amplio que solo top-ranked |
| **Perplexity** | Siempre cita fuentes con links | Favorece contenido autorizado, reciente y bien estructurado |
| **Gemini** | IA de Google | Índice de Google + Knowledge Graph |
| **Copilot** | Búsqueda de Bing | Índice de Bing + fuentes autoritativas |
| **Claude** | Brave Search (cuando habilitado) | Datos de entrenamiento + resultados de búsqueda |

### Diferencia clave vs. SEO tradicional

El SEO tradicional te hace rankear. El AI SEO te hace **citar**.

En la búsqueda tradicional, necesitas estar en la página 1. En la búsqueda de IA, una página bien estructurada puede ser citada aunque esté en la página 2 o 3 — los sistemas de IA seleccionan fuentes por calidad de contenido, estructura y relevancia, no solo por posición.

**Datos relevantes:**
- Los AI Overviews aparecen en ~45% de las búsquedas de Google
- Las marcas son 6.5x más propensas a ser citadas vía fuentes de terceros que su propio dominio
- El contenido optimizado se cita 3x más que el no optimizado
- Estadísticas y citas aumentan la visibilidad en IA en 40%+

---

## Auditoría de visibilidad en IA

### Paso 1: Verificar respuestas de IA para las queries clave de ISISA

Probar 10-20 queries importantes en cada plataforma:

| Query | Google AI Overview | ChatGPT | Perplexity | ¿ISISA citada? | ¿Competidores? |
|-------|:-----------------:|:-------:|:----------:|:--------------:|:--------------:|
| "dióxido de cloro desinfección agua México" | Sí/No | Sí/No | Sí/No | Sí/No | [quién] |
| "NOM-127-SSA1 parámetros agua potable" | Sí/No | Sí/No | Sí/No | Sí/No | [quién] |
| "analizador de conductividad industrial" | Sí/No | Sí/No | Sí/No | Sí/No | [quién] |
| "calibración instrumentos agua CENAM" | Sí/No | Sí/No | Sí/No | Sí/No | [quién] |

**Tipos de queries a probar:**
- "¿Qué es el dióxido de cloro y para qué sirve?"
- "Mejores analizadores de conductividad para agua industrial"
- "CLOXIFREE vs. cloro tradicional"
- "Cómo cumplir NOM-127-SSA1-2021"
- "Precio calibración equipos de instrumentación México"

### Paso 2: Verificar acceso de bots de IA

Verificar que robots.txt de isisainst.com.mx permita los rastreadores de IA. Bloquear un bot significa que esa plataforma no puede citar a ISISA:

- **GPTBot** y **ChatGPT-User** — OpenAI (ChatGPT)
- **PerplexityBot** — Perplexity
- **ClaudeBot** y **anthropic-ai** — Anthropic (Claude)
- **Google-Extended** — Gemini y AI Overviews de Google
- **Bingbot** — Microsoft Copilot

Bloquear estos bots previene la citación. Se puede bloquear **CCBot** (Common Crawl, usado para entrenamiento) sin afectar la citación en búsqueda.

### Paso 3: Verificar extractabilidad del contenido

Para cada página prioritaria de ISISA:

| Verificación | Pasa/Falla |
|-------------|------------|
| ¿Hay definición clara en el primer párrafo? | |
| ¿Los bloques de respuesta funcionan sin contexto circundante? | |
| ¿Hay estadísticas con fuentes citadas? | |
| ¿Hay tablas comparativas para queries "X vs Y"? | |
| ¿Hay sección FAQ con preguntas en lenguaje natural? | |
| ¿Hay schema markup (FAQ, Article, Product)? | |
| ¿Hay atribución de autoría? | |
| ¿Actualizado en los últimos 6 meses? | |
| ¿Estructura de encabezados que coincide con patrones de búsqueda? | |

---

## Estrategia de optimización

### Los tres pilares

```
1. Estructura (hacerlo extraíble)
2. Autoridad (hacerlo citable)
3. Presencia (estar donde la IA busca)
```

### Pilar 1: Estructura — hacer el contenido extraíble

Los sistemas de IA extraen pasajes, no páginas. Cada afirmación clave debe funcionar como declaración independiente.

**Patrones de bloques de contenido para ISISA:**
- **Bloque de definición** para queries "¿Qué es el dióxido de cloro?"
- **Bloques paso a paso** para queries "¿Cómo dosificar CLOXIFREE®?"
- **Tablas comparativas** para queries "ClO₂ vs. cloro vs. ozono"
- **Tablas de especificaciones** para queries de equipos B&C Electronics
- **Bloques de normativa** para queries de NOM-127-SSA1

**Estructura de artículo AI-optimizado para ISISA:**

```markdown
## [Definición directa — ≤40 palabras respondiendo la pregunta principal]

[Párrafo de contexto — expandir con datos técnicos específicos]

## [H2 como pregunta explícita que el usuario hace]

[Respuesta directa en las primeras 2 oraciones]
[Detalle técnico con datos concretos]

## Tabla comparativa o de especificaciones
| [Parámetro] | [Valor/Comparación] |
|-------------|---------------------|
| | |

## Preguntas frecuentes

**¿[Pregunta técnica específica]?**
[Respuesta de 50-80 palabras, autocontenida]

**¿[Pregunta normativa o de aplicación]?**
[Respuesta de 50-80 palabras, autocontenida]
```

### Pilar 2: Autoridad — hacer el contenido citable

**Señales de autoridad que los LLMs priorizan:**
- Datos y estadísticas con fuentes específicas (citar NOMs, estudios, normas ISO)
- Atribución de expertos (Ing. Químico Pedro Loredo, técnicos certificados)
- Presencia en terceros: directorios industriales, asociaciones del sector agua en México, artículos en medios especializados
- Menciones de marca en contexto claro: "ISISA, empresa mexicana con sede en Coyoacán CDMX, distribuidor oficial de B&C Electronics..."
- Actualizaciones con fecha visible

**Lenguaje de entidad para que los LLMs reconozcan a ISISA:**
- Siempre mencionar "ISISA" con contexto geográfico: "ISISA Desinfección, Instrumentación y Servicio, empresa mexicana con sede en CDMX"
- Conectar "CLOXIFREE®" con "dióxido de cloro" y con "ISISA" en cada mención
- Conectar "B&C Electronics" con "distribuidor oficial en México" y con "ISISA"

### Pilar 3: Presencia — estar donde la IA busca

**Plataformas de terceros donde ISISA debe tener presencia:**
- Google Business Profile (CDMX + Querétaro) — actualizado con descripción técnica detallada
- LinkedIn (página de empresa con contenido técnico regular)
- Directorios industriales mexicanos: CANACINTRA, ANIQ, CANAGUA afiliadas
- Wikipedia (entrada sobre ClO₂ en español con referencia a proveedores en México)
- Foros técnicos: menciones en conversaciones de Reddit en español, foros de ingeniería

---

## Optimización de contenido existente

### Para artículos de blog

**Ejemplo: "Control PID aplicado a la dosificación de dióxido de cloro"**

Checklist de optimización AI:
- [ ] Agregar definición de apertura (≤40 palabras respondiendo "¿Qué es el control PID en dosificación de ClO₂?")
- [ ] Reestructurar H2s como preguntas que los ingenieros hacen realmente
- [ ] Agregar tabla de parámetros clave (Kp, Ki, Kd con rangos típicos para ClO₂)
- [ ] Citar NOM-127-SSA1-2021 con número específico y parámetro de ClO₂ residual
- [ ] Agregar sección FAQ (5 preguntas)
- [ ] Implementar Schema FAQ en JSON-LD
- [ ] Mencionar ISISA y el analizador CL 7685 de B&C Electronics en contexto natural

### Para páginas de producto B&C Electronics

Estructura AI-optimizada para una ficha de producto:

```markdown
## [Nombre del producto] — [Definición citeable en ≤50 palabras]

El [Producto] es [qué es], diseñado para [aplicación principal] en plantas
[sector] que requieren [cumplimiento normativo]. [Beneficio diferenciador].
Disponible en México a través de ISISA, distribuidor oficial de B&C Electronics.

## Especificaciones técnicas

| Parámetro | Valor |
|-----------|-------|
| Rango de medición | |
| Señal de salida | |
| Protocolo | |
| Protección | |
| Alimentación | |

## Casos de uso industriales

1. [Caso de uso 1 — industria específica]
2. [Caso de uso 2]
3. [Caso de uso 3]

## Preguntas frecuentes

**¿Para qué industrias es adecuado el [Producto]?**
[Respuesta autocontenida de 50-80 palabras]

**¿Qué normas cumple?**
[Respuesta con NOMs y estándares específicos]
```

---

## Schema markup base para isisainst.com.mx

### Organization Schema (implementar en homepage)

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "ISISA Desinfección, Instrumentación y Servicio",
  "url": "https://isisainst.com.mx",
  "logo": "https://isisainst.com.mx/wp-content/uploads/2022/08/LOGO-ISISA-.png",
  "description": "Empresa mexicana especializada en instrumentación industrial para control de calidad del agua, desinfección con dióxido de cloro (CLOXIFREE®) y servicios de calibración certificada. Distribuidores oficiales de B&C Electronics en México.",
  "address": [
    {
      "@type": "PostalAddress",
      "streetAddress": "Coyoacán",
      "addressLocality": "Ciudad de México",
      "postalCode": "04230",
      "addressCountry": "MX"
    }
  ],
  "telephone": "+52-55-9313-1793",
  "email": "ventas@isisainst.com.mx",
  "areaServed": "MX",
  "knowsAbout": [
    "Dióxido de cloro",
    "Instrumentación industrial para agua",
    "Tratamiento de agua",
    "NOM-127-SSA1-2021",
    "Calibración de instrumentos CENAM",
    "B&C Electronics",
    "CLOXIFREE"
  ]
}
```

### FAQ Schema (template)

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "¿Qué es el dióxido de cloro y cómo se usa para desinfección de agua?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "El dióxido de cloro (ClO₂) es un biocida de amplio espectro que elimina bacterias, virus, hongos y esporas en el agua. A diferencia del cloro tradicional, no genera trihalometanos y es efectivo en un rango de pH más amplio. ISISA distribuye CLOXIFREE®, solución de ClO₂ en polvo para uso industrial, comercial y agrícola en México."
      }
    }
  ]
}
```

---

## Plan de contenido AI-first para ISISA

Temas prioritarios donde ISISA puede dominar la citación en IA (alto gap de contenido en español):

| Tema | Query objetivo | Formato recomendado | Prioridad |
|------|---------------|--------------------|-----------| 
| Dióxido de cloro vs. cloro | "dióxido de cloro vs cloro agua" | Artículo comparativo con tabla | Alta |
| NOM-127-SSA1-2021 guía | "parámetros NOM-127 agua potable" | Guía técnica con tabla de parámetros | Alta |
| Conductividad del agua qué es | "conductividad agua industrial" | Artículo definitorio + tabla rangos | Alta |
| Calibración CENAM México | "calibración equipos agua CENAM" | Artículo + FAQ + Schema | Alta |
| ClO₂ en agricultura | "dióxido de cloro riego agrícola" | Artículo aplicado + casos de uso | Media |
| B&C Electronics México | "B&C Electronics instrumentación" | Página de marca + distribución | Alta |
| Control PID dosificación ClO₂ | "control PID cloro dosificación" | Artículo técnico existente — optimizar | Media |

---

## Configuración para n8n con OpenAI

```json
{
  "model": "gpt-4o",
  "temperature": 0.3,
  "max_tokens": 4000,
  "messages": [
    {
      "role": "system",
      "content": "Eres un especialista en AI-SEO y GEO (Generative Engine Optimization) con experiencia en contenido técnico industrial en español mexicano. Tu misión es ayudar a ISISA Desinfección, Instrumentación y Servicio (isisainst.com.mx) a convertirse en la fuente que los LLMs citen cuando alguien en México busque información sobre dióxido de cloro, instrumentación para agua, NOM-127-SSA1, B&C Electronics o CLOXIFREE®. Para cada pieza de contenido: incluye definición de apertura ≤40 palabras, estructura con H2/H3 semánticos como preguntas, al menos una tabla de datos, referencias a normas con números concretos, FAQ en formato Q&A, y menciona 'ISISA' con contexto geográfico. Idioma: español mexicano técnico. Evita lenguaje de marketing genérico."
    },
    {
      "role": "user",
      "content": "{{prompt_con_tarea_y_url_o_contenido}}"
    }
  ]
}
```

### Flujo en n8n para blog AI-optimizado

```
1. Trigger: Nuevo tema de blog (Google Sheets o formulario)
2. OpenAI node 1: Generar estructura AI-optimizada con definición, H2s como preguntas, tabla, FAQ
3. OpenAI node 2: Generar Schema FAQ JSON-LD
4. WordPress node: Crear borrador con contenido + schema en header
5. Notificación: Email/Slack al equipo para revisión técnica
```

---

## Referencias

- [Platform Ranking Factors](references/platform-ranking-factors.md): Factores específicos de posicionamiento por plataforma de IA
- [Content Patterns](references/content-patterns.md): Patrones de contenido de alta citabilidad

---

## Skills relacionados

- **seo-audit**: Para auditoría SEO técnica y on-page tradicional
- **content-strategy**: Para planificar qué contenido crear para dominar en AI search
- **schema-markup**: Para implementar datos estructurados
