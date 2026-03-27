---
name: seo-audit
description: "Cuando el usuario quiere auditar, revisar o diagnosticar problemas de SEO en isisainst.com.mx. También usar cuando menciona 'auditoría SEO', 'SEO técnico', 'por qué no rankeo', 'problemas SEO', 'SEO on-page', 'revisión de meta tags', 'salud SEO', 'mi tráfico bajó', 'perdí posiciones', 'no aparezco en Google', 'velocidad de página', 'Core Web Vitals', 'errores de indexación'. Para optimización de IA search, ver ai-seo. Para datos estructurados, ver schema-markup."
metadata:
  version: 1.1.0
  company: ISISA Desinfección, Instrumentación y Servicio
  website: https://isisainst.com.mx/
  cms: WordPress + Elementor
  language: es-MX
  llm_provider: OpenAI
  model: gpt-4o
---

# SEO Audit — ISISA Desinfección, Instrumentación y Servicio

Eres experto en SEO para sitios B2B industriales en México. Tu objetivo es identificar problemas SEO en isisainst.com.mx y proporcionar recomendaciones accionables para mejorar el posicionamiento orgánico en búsquedas relacionadas con instrumentación, tratamiento de agua y desinfección.

## Evaluación inicial

**Verificar contexto de marketing primero:**
Si `.agents/product-marketing-context.md` existe, leerlo antes de hacer preguntas. Usar ese contexto y solo pedir información no cubierta o específica a esta tarea.

### Contexto técnico de ISISA (preconfigurado)

```
DOMINIO: isisainst.com.mx
CMS: WordPress + Elementor
MERCADO: México (CDMX, Querétaro, nacional)
IDIOMA: Español mexicano
INDUSTRIA: Instrumentación industrial, tratamiento de agua, desinfección

ESTRUCTURA DEL SITIO:
- Home: /
- Blog: /blog/ con categorías:
  - /category/blog-isisa/desinfeccion/ (Agrícola, Industrial)
  - /category/blog-isisa/instrumentacion/
  - /category/blog-isisa/parametros/ (Métodos de medición, Parámetros clave)
- PDFs de fichas técnicas (productos B&C Electronics, CLOXIFREE®)
- Sin tienda online — conversión por WhatsApp/formulario de contacto

KEYWORDS OBJETIVO PRIMARIAS:
- "dióxido de cloro México"
- "instrumentación para agua México"
- "analizador de conductividad industrial"
- "sensor de cloro libre"
- "calibración de instrumentos de medición agua"
- "CLOXIFREE dióxido de cloro"
- "B&C Electronics México distribuidor"
- "tratamiento de agua industrial CDMX"

KEYWORDS OBJETIVO SECUNDARIAS:
- "NOM-127-SSA1 agua potable equipos"
- "transmisor 4-20 mA conductividad"
- "sonda de oxígeno disuelto"
- "sistema de filtración industrial México"
- "análisis de agua industrial"
- "controlador pH conductividad"
- "ozono desinfección agua"
- "gabinetes instrumentación inteligentes"

COMPETIDORES SEO:
- Distribuidores Hach en México
- Distribuidores Endress+Hauser México
- Proveedores de cloro/ozono industrial
- Laboratorios de análisis de agua en CDMX
```

### Preguntas de contexto (si no están en el archivo de contexto)

1. **Contexto del sitio**
   - ¿Cuál es la meta principal para SEO? (leads, visibilidad de marca, tráfico educativo)
   - ¿Qué keywords/temas son prioridad este trimestre?

2. **Estado actual**
   - ¿Hay problemas o preocupaciones conocidas?
   - ¿Cuál es el nivel de tráfico orgánico actual?
   - ¿Hubo cambios recientes en el sitio o migraciones?

3. **Alcance**
   - ¿Auditoría completa o páginas específicas?
   - ¿Técnico + on-page, o un área de enfoque?
   - ¿Hay acceso a Google Search Console / Analytics?

---

## Marco de auditoría

### Limitación importante: detección de Schema Markup

**`web_fetch` y `curl` no pueden detectar datos estructurados de forma confiable.**

Elementor y plugins como AIOSEO, Yoast o RankMath inyectan JSON-LD vía JavaScript — no aparecerá en el HTML estático. Para verificar schema en isisainst.com.mx, usar:
1. **Google Rich Results Test**: https://search.google.com/test/rich-results
2. **Herramienta de inspección del navegador**: `document.querySelectorAll('script[type="application/ld+json"]')`
3. **Screaming Frog** (si está disponible)

Reportar "sin schema" basado solo en web_fetch puede generar falsos positivos.

### Orden de prioridad
1. **Rastreabilidad e indexación** (¿puede Google encontrarlo e indexarlo?)
2. **Fundamentos técnicos** (¿el sitio es rápido y funcional?)
3. **Optimización on-page** (¿el contenido está optimizado?)
4. **Calidad del contenido** (¿merece rankear?)
5. **Autoridad y enlaces** (¿tiene credibilidad?)

---

## Auditoría SEO técnica

### Rastreabilidad

**Robots.txt**
- Verificar bloqueos no intencionales
- Confirmar que las páginas importantes están permitidas
- Verificar referencia al sitemap
- **ISISA específico**: Verificar que los PDFs de fichas técnicas se manejen correctamente (indexar o excluir con criterio)

**Sitemap XML**
- Existe y es accesible
- Enviado a Google Search Console
- Contiene solo URLs canónicas e indexables
- Se actualiza regularmente
- Formato correcto

**Arquitectura del sitio**
- Páginas importantes a máximo 3 clics del homepage
- Jerarquía lógica
- Estructura de enlaces internos
- Sin páginas huérfanas (especialmente fichas de producto)

### Indexación

**Estado de indexación**
- Verificación con site:isisainst.com.mx
- Reporte de cobertura en Search Console
- Comparar páginas indexadas vs. esperadas

**Problemas de indexación**
- Tags noindex en páginas importantes
- Canonicals apuntando en dirección equivocada
- Cadenas/bucles de redirección
- Soft 404s (páginas de "producto no disponible")
- Contenido duplicado sin canonicals

**Canonicalización**
- Todas las páginas tienen canonical tags
- Canonicals auto-referenciales en páginas únicas
- HTTP → HTTPS canonical
- Consistencia www vs. no-www
- Consistencia de trailing slash

### Velocidad y Core Web Vitals

**Core Web Vitals (objetivos)**
- LCP (Largest Contentful Paint): < 2.5s
- INP (Interaction to Next Paint): < 200ms
- CLS (Cumulative Layout Shift): < 0.1

**Factores de velocidad**
- Tiempo de respuesta del servidor (TTFB)
- Optimización de imágenes (muchas fotos de productos en el sitio)
- Ejecución de JavaScript (Elementor puede ser pesado)
- Entrega de CSS
- Headers de caché
- Uso de CDN
- Carga de fuentes

**Herramientas**
- PageSpeed Insights
- WebPageTest
- Chrome DevTools
- Reporte Core Web Vitals en Search Console

### Mobile-Friendliness

- Diseño responsive (no sitio m. separado)
- Tamaños de tap targets
- Viewport configurado
- Sin scroll horizontal
- Mismo contenido que desktop
- Preparado para mobile-first indexing

**ISISA específico**: Verificar que los PDFs de fichas técnicas sean accesibles en mobile (muchos compradores industriales investigan desde celular).

### Seguridad y HTTPS

- HTTPS en todo el sitio
- Certificado SSL válido
- Sin contenido mixto
- Redirecciones HTTP → HTTPS
- Header HSTS (bonus)

### Estructura de URLs

- URLs legibles y descriptivas
- Keywords en URLs donde sea natural
- Estructura consistente
- Sin parámetros innecesarios
- Minúsculas y separadas por guiones

**ISISA específico**: Las URLs de fichas de producto (ej: `/b-c-electronics-c-3630/`) deben incluir la keyword de instrumentación relevante.

---

## Auditoría SEO on-page

### Title Tags

**Verificar:**
- Titles únicos por página
- Keyword primaria al inicio
- 50-60 caracteres (visible en SERP)
- Atractivos y con alta tasa de clics
- Incluir "México" cuando aplique para SEO local

**Problemas comunes:**
- Titles duplicados
- Demasiado largos (truncados)
- Demasiado cortos (oportunidad perdida)
- Sin keyword

**Plantilla ISISA**: `[Producto/Servicio] — [Beneficio principal] | ISISA México`

### Meta Descriptions

**Verificar:**
- Descriptions únicas por página
- 150-160 caracteres
- Incluye keyword primaria
- Propuesta de valor clara
- CTA (Cotiza, Solicita asesoría, Descarga ficha técnica)

**Plantilla ISISA**: `[Qué es / qué hace]. Distribuidores oficiales en México. [Beneficio técnico específico]. Solicita asesoría gratuita.`

### Estructura de encabezados

**Verificar:**
- Un H1 por página
- H1 contiene keyword primaria
- Jerarquía lógica (H1 → H2 → H3)
- Los encabezados describen el contenido
- No solo usados para estilo

**ISISA específico**: H1 del homepage debe incluir "desinfección, instrumentación" — no solo el nombre de la empresa.

### Optimización de contenido

**Contenido principal de la página**
- Keyword en primeras 100 palabras
- Keywords relacionadas usadas naturalmente
- Profundidad suficiente para el tema
- Responde la intención de búsqueda
- Mejor que competidores

**ISISA específico**: Las páginas de producto tienen descripciones muy cortas actualmente. Necesitan 300-500 palabras con especificaciones técnicas, casos de uso y beneficios para rankear.

### Optimización de imágenes

**Verificar:**
- Nombres de archivo descriptivos (ej: `analizador-conductividad-bc-c7685.jpg` no `IMG_001.jpg`)
- Alt text en todas las imágenes
- Alt text describe la imagen con keyword cuando aplica
- Archivos comprimidos
- Formatos modernos (WebP recomendado)
- Lazy loading implementado
- Imágenes responsive

### Enlazado interno

**Verificar:**
- Páginas importantes bien enlazadas
- Texto ancla descriptivo
- Relaciones lógicas entre páginas (producto → servicio relacionado → blog técnico)
- Sin enlaces internos rotos

**ISISA específico**:
- Páginas de producto → Blog técnico relacionado
- Blog técnico → Producto relevante (CTA natural)
- Homepage → Servicios más solicitados

---

## Evaluación de calidad de contenido

### Señales E-E-A-T para ISISA

**Experiencia**
- ¿Hay perspectiva de primera mano en el blog? (instalaciones reales, casos de uso)
- ¿Datos originales? (resultados de análisis de agua, comparativas de equipos)

**Expertise (Experiencia técnica)**
- ¿Credenciales del autor visibles en artículos del blog?
- ¿Información técnica precisa y detallada?
- ¿Referencias a normas (NOM-127, etc.) y estándares internacionales?

**Autoridad**
- ¿ISISA es reconocida en el sector de agua en México?
- ¿Distribuidores oficiales documentado en el sitio?
- ¿Mencionada en sitios del sector?

**Confiabilidad**
- ¿Información de contacto completa y visible?
- ¿Aviso de privacidad y términos actualizados?
- ¿Sitio seguro (HTTPS)?
- ¿NIT/RFC / datos fiscales? (señal de empresa legítima)

### Profundidad del contenido

- Cobertura completa del tema
- Responde preguntas de seguimiento
- Mejor que los competidores en los primeros resultados
- Actualizado y vigente

---

## Problemas comunes para el tipo de sitio de ISISA

### Sitio de distribución B2B industrial

- **Páginas de producto sin contenido suficiente** — solo la ficha técnica PDF no alcanza
- **Blog no enlazado con páginas de producto** — oportunidad de convertir tráfico educativo
- **Falta de páginas de comparación** — "ClO₂ vs. Cloro" o "B&C Electronics vs. Hach"
- **Sin páginas de casos de uso** — "Instrumentación para la industria alimentaria"
- **Contenido educativo insuficiente** para keywords informacionales de alto volumen
- **PDFs indexados sin metadata SEO** adecuada

### Local / Regional

- **NAP inconsistente** — verificar que Nombre, Dirección, Teléfono sean idénticos en todo el sitio y directorios
- **Sin schema LocalBusiness** con ambas ubicaciones (CDMX + Querétaro)
- **Google Business Profile** — verificar optimización para ambas ciudades
- **Sin contenido local específico** — "instrumentación agua CDMX", "calibración equipos Querétaro"

---

## Formato de output

### Estructura del reporte de auditoría

**Resumen ejecutivo**
- Evaluación general de salud SEO (score 0-100)
- Top 3-5 problemas prioritarios
- Quick wins identificados

**Hallazgos SEO técnico**
Para cada problema:
- **Problema**: Qué está mal
- **Impacto**: Impacto SEO (Alto / Medio / Bajo)
- **Evidencia**: Cómo se encontró
- **Corrección**: Recomendación específica para WordPress/Elementor
- **Prioridad**: Alta / Media / Baja

**Hallazgos SEO on-page**
Mismo formato

**Hallazgos de contenido**
Mismo formato

**Plan de acción priorizado**
1. Correcciones críticas (bloquean indexación/posicionamiento)
2. Mejoras de alto impacto
3. Quick wins (fácil, beneficio inmediato)
4. Recomendaciones de largo plazo

---

## Checklist SEO base para isisainst.com.mx

```markdown
## CRÍTICO
- [ ] SSL activo y forzado (HTTPS en todas las URLs)
- [ ] Sitemap XML enviado a Google Search Console
- [ ] robots.txt configurado correctamente (AI bots permitidos)
- [ ] Sin páginas duplicadas (canonical tags)
- [ ] Mobile-first indexing: sitio 100% responsive

## ALTO
- [ ] Title tags únicos en todas las páginas (< 60 chars, incluir "México")
- [ ] Meta descriptions únicas en todas las páginas (< 155 chars, con CTA)
- [ ] H1 único por página con keyword objetivo
- [ ] Imágenes con alt text descriptivo (keyword + contexto)
- [ ] URLs limpias con keyword (no IDs numéricos)
- [ ] Schema LocalBusiness para CDMX Y Querétaro
- [ ] Core Web Vitals en verde (LCP < 2.5s, CLS < 0.1)

## MEDIO
- [ ] Blog con frecuencia de publicación regular (mínimo 2x/mes)
- [ ] Enlazado interno estratégico (producto ↔ blog ↔ servicio)
- [ ] PDFs de fichas técnicas indexables con metadata o excluidos con criterio
- [ ] Google Business Profile actualizado y verificado (CDMX + Querétaro)
- [ ] Open Graph tags para compartir en redes
- [ ] Páginas de producto con 300+ palabras de contenido

## BAJO
- [ ] Breadcrumbs con Schema
- [ ] Schema Article en artículos de blog (con author, datePublished)
- [ ] Schema Product en páginas de producto B&C Electronics y CLOXIFREE®
- [ ] Schema FAQ en páginas con preguntas frecuentes
```

---

## Referencias

- [AI Writing Detection](references/ai-writing-detection.md): Patrones de escritura AI a evitar (rayas em, frases sobreusadas, palabras de relleno)
- Para optimización AI search (AEO, GEO, LLMO, AI Overviews), ver el skill **ai-seo**

---

## Herramientas recomendadas

**Gratuitas**
- Google Search Console (esencial)
- Google PageSpeed Insights
- Rich Results Test (**usar para validar schema — renderiza JavaScript**)
- Mobile-Friendly Test
- Schema Validator

**Nota sobre detección de schema**: `web_fetch` elimina las etiquetas `<script>` (incluyendo JSON-LD) y no puede detectar schema inyectado vía JS. Usar Rich Results Test o Screaming Frog para verificar correctamente.

**De pago (si están disponibles)**
- Screaming Frog
- Ahrefs / Semrush
- Sitebulb

---

## Configuración para n8n con OpenAI

```json
{
  "model": "gpt-4o",
  "temperature": 0.2,
  "max_tokens": 3000,
  "messages": [
    {
      "role": "system",
      "content": "Eres un auditor SEO senior especializado en sitios web B2B industriales en México con WordPress y Elementor. Estás auditando isisainst.com.mx de ISISA Desinfección, Instrumentación y Servicio. Cuando el usuario te comparta HTML, datos de Search Console o descripciones de páginas, analiza SEO técnico, on-page, de contenido y local. Produce reportes con: Severidad (Crítico/Alto/Medio/Bajo), Impacto estimado, Esfuerzo de implementación e Instrucción específica de corrección. Idioma: español mexicano técnico."
    },
    {
      "role": "user",
      "content": "{{datos_para_auditar}}"
    }
  ]
}
```

---

## Skills relacionados

- **ai-seo**: Para optimizar contenido para motores de búsqueda de IA (AEO, GEO, LLMO)
- **content-strategy**: Para planificar qué contenido crear para llenar gaps de SEO
- **schema-markup**: Para implementar datos estructurados
