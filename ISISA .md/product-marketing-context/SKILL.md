---
name: product-marketing-context
description: "Cuando el usuario quiere crear o actualizar el documento base de estrategia de marketing de ISISA. También usar cuando el usuario menciona 'contexto de producto', 'contexto de marketing', 'configurar contexto', 'posicionamiento', 'quién es mi cliente', 'ICP', 'perfil de cliente ideal', o quiere evitar repetir información fundacional en tareas de marketing. Usar al inicio de cualquier proyecto nuevo antes de otros skills de marketing — crea `.agents/product-marketing-context.md` que todos los demás skills referencian."
metadata:
  version: 1.1.0
  company: ISISA Desinfección, Instrumentación y Servicio
  website: https://isisainst.com.mx/
  language: es-MX
  llm_provider: OpenAI
  model: gpt-4o
---

# Product Marketing Context — ISISA

Ayudas a crear y mantener el documento de contexto de marketing de ISISA Desinfección, Instrumentación y Servicio. Este documento captura información fundacional de posicionamiento y mensajería que los demás skills referencian.

El documento se guarda en `.agents/product-marketing-context.md`.

## Contexto base preconfigurado de ISISA

```
EMPRESA: ISISA — Desinfección, Instrumentación y Servicio
FUNDADOR: Ing. Químico Pedro Loredo
FUNDACIÓN: Hace más de una década (>10 años en el mercado)
SEDE: Coyoacán, CDMX (CP 04230) | Oficina: Querétaro
WEB: https://isisainst.com.mx/ | EMAIL: ventas@isisainst.com.mx
TEL: (55) 9313 1793 | QRO: (442) 4553 144 | WA: (56) 2657 8130

PROPUESTA DE VALOR: "Invertimos inteligencia para que tú no pierdas dinero."
PILARES: Enfoque al cliente | Mejora continua | Calidad integral

PRODUCTOS:
- CLOXIFREE® Dióxido de Cloro en polvo (10L / 20L / 50L / 100L)
- B&C Electronics: C 3630 (transmisor conductividad), C 3645 (controlador
  conductividad), C 7685 (analizador conductividad), CL 7685 (controlador
  cloro/ozono), C 8325.5 / C 8520.5 / C 8825.4 (sondas toroidales IP68
  RS485 Modbus), CL 7901 (celda flujo + sensor cloro libre), OD 8182
  (sonda O₂ disuelto con autolimpieza)

SERVICIOS: Desinfección ClO₂ | Sistemas de filtración | Calibración
           certificada | Análisis agua NOM-127-SSA1-2021 | Gabinetes
           inteligentes a medida | Puesta en marcha

NORMATIVAS: NOM-127-SSA1-2021 | NOM-012-SCFI | NOM-001-SEDE | CENAM
MERCADOS: Industrial | Comercial | Agrícola
```

## Workflow

### Paso 1: Verificar contexto existente

Primero verificar si `.agents/product-marketing-context.md` ya existe.

**Si existe:**
- Leerlo y resumir qué está capturado
- Preguntar qué secciones quiere actualizar
- Solo recopilar info para esas secciones

**Si no existe, ofrecer dos opciones:**

1. **Auto-draft desde contexto base** (recomendado): Usar el bloque de contexto de ISISA de arriba para generar un borrador V1. El usuario revisa y llena gaps. Más rápido que empezar de cero.

2. **Construir sección por sección**: Recorrer cada sección conversacionalmente, una a la vez.

La mayoría prefiere opción 1. Después del borrador, preguntar: "¿Qué necesita corregirse? ¿Qué falta?"

### Paso 2: Recopilar o confirmar información

**Si se usa auto-draft:**
1. Partir del contexto base preconfigurado
2. Complementar con info adicional del usuario
3. Presentar draft y preguntar qué ajustar
4. Iterar hasta satisfacción

**Si se construye desde cero:**
Recorrer secciones una a la vez. Buscar siempre el **lenguaje literal del cliente** — frases exactas de compradores industriales son más valiosas que descripciones pulidas.

---

## Secciones a capturar

### 1. Descripción del producto/servicio
- Descripción en una línea
- Qué hace (2-3 oraciones)
- Categoría de producto (cómo te buscan los clientes)
- Tipo de negocio (distribución, servicios, SaaS)
- Modelo de negocio

**Base ISISA:** Distribución de instrumentación industrial + servicios especializados para control de calidad del agua. Modelo: venta directa de equipos + servicios por contrato (calibración, mantenimiento, análisis).

### 2. Audiencia objetivo
- Tipo de empresa cliente (industria, tamaño)
- Tomadores de decisión (roles, departamentos)
- Caso de uso primario
- Jobs to be done (2-3)
- Casos de uso específicos

**Base ISISA:** Industrias de alimentos, farmacéutica, química, manufactura, municipal. Roles: Ing. de Planta, Jefe de Operaciones, Responsable de Calidad, Gerente de Mantenimiento, Director de Compras.

### 3. Personas B2B

| Persona | Se preocupa por | Reto principal | Valor que prometemos |
|---------|----------------|----------------|---------------------|
| Ingeniero de Planta | Cumplimiento normativo, continuidad operativa | Auditorías COFEPRIS, equipos sin calibración | Calibración CENAM + informes detallados |
| Jefe de Mantenimiento | Confiabilidad de equipos, costos de falla | Tiempo de inactividad, proveedores lentos | Soporte técnico ágil + repuestos disponibles |
| Responsable de Calidad | Parámetros dentro de norma, trazabilidad | Lecturas inconsistentes, falta de evidencia | Equipos certificados + análisis NOM-127 |
| Director de Compras | ROI, garantías, reputación del proveedor | Justificar inversión, riesgo de decisión | 10+ años de experiencia, distribuidores oficiales |
| Agrónomo / Gerente Agrícola | Eficiencia, no dañar cultivos | Concentraciones seguras de ClO₂ | Asesoría técnica + CLOXIFREE® |

### 4. Problemas y pain points
- Reto central antes de encontrarte
- Por qué las soluciones actuales se quedan cortas
- Costo para el cliente (tiempo, dinero, riesgo)
- Tensión emocional

**Base ISISA:** Equipos descalibrados → no conformidades; proveedores sin soporte post-venta; sistemas de desinfección ineficientes; falta de documentación CENAM; consecuencias: multas, paros de planta, riesgo sanitario.

### 5. Panorama competitivo
- **Directos**: Distribuidores Hach, YSI, Endress+Hauser en México
- **Secundarios**: Proveedores de químicos genéricos; laboratorios externos
- **Indirectos**: Mantenimiento interno sin especialización; importaciones directas

### 6. Diferenciación
- +10 años de experiencia en mercado mexicano
- Distribuidores oficiales de B&C Electronics y otras marcas líderes
- Soluciones a medida ("traje hecho a medida para cada cliente")
- Técnicos certificados con trazabilidad CENAM
- I+D+i interno (plataforma IIoT/SCADA en desarrollo)
- Cobertura CDMX + Querétaro
- Producto propio: CLOXIFREE®

### 7. Objeciones y anti-personas
- **Objeciones**: "Es muy caro vs. cloro tradicional", "¿Tienen soporte rápido?", "¿Sus calibraciones tienen validez oficial?"
- **Anti-persona**: Solo buscan precio más bajo sin importar trazabilidad; proyectos únicos sin mantenimiento

### 8. Dinámica de cambio (JTBD Four Forces)
- **Push**: Proveedor actual sin soporte, equipos sin calibración válida, fallas en auditorías
- **Pull**: Solución integral, técnicos certificados, producto ClO₂ propio
- **Hábito**: "Siempre usamos cloro normal", "Ya tenemos proveedor conocido"
- **Ansiedad**: "¿Qué pasa si el nuevo sistema falla?", "¿Pueden atender emergencias?"

### 9. Lenguaje del cliente
- **Cómo describen el problema**: "No pasa la auditoría", "El equipo da lecturas raras", "Necesito certificado CENAM"
- **Cómo describen ISISA**: "Los de los equipos B&C", "Los especialistas en agua"
- **Palabras a usar**: dióxido de cloro, instrumentación, calibración certificada, NOM-127, trazabilidad CENAM, dosificación
- **Palabras a evitar**: "revolucionario", "el mejor" (sin evidencia)
- **Glosario**:

| Término | Significado |
|---------|-------------|
| ClO₂ | Dióxido de cloro |
| 4-20 mA | Señal estándar de instrumentación industrial |
| IP68 | Protección total contra inmersión en agua |
| Modbus RS485 | Protocolo de comunicación industrial |
| CENAM | Centro Nacional de Metrología (calibración oficial MX) |
| NOM-127 | Norma de calidad del agua para consumo humano |

### 10. Voz de marca
- **Tono**: Técnico pero accesible, confiable, orientado a resultados
- **Estilo**: Directo, específico, con datos concretos — nunca marketing genérico
- **Personalidad**: Experto de confianza, socio técnico, riguroso y práctico

### 11. Pruebas y evidencias
- Más de 10 años en el mercado mexicano
- Distribuidores oficiales de marcas líderes internacionales
- Fichas técnicas detalladas de todos los productos
- Cumplimiento NOM-127-SSA1-2021
- Trazabilidad CENAM en calibraciones

### 12. Objetivos
- **Meta**: Posicionarse como integrador líder de soluciones de control de agua en México; expansión con plataforma IIoT SaaS
- **Conversión clave**: Solicitar asesoría gratuita → Cotización → Instalación/servicio
- **Canales activos**: Web, WhatsApp, email, referencias

---

## Paso 3: Crear el documento

```markdown
# Contexto de Marketing — ISISA
# Desinfección, Instrumentación y Servicio

*Última actualización: [fecha]*
*Web: https://isisainst.com.mx/*

## Descripción del producto/servicio
**Una línea:**
**Qué hace:**
**Categoría:**
**Tipo de negocio:**
**Modelo de negocio:**

## Audiencia objetivo
**Empresas objetivo:**
**Tomadores de decisión:**
**Caso de uso primario:**
**Jobs to be done:**
-
**Casos de uso específicos:**
-

## Personas B2B
| Persona | Se preocupa por | Reto | Valor que prometemos |
|---------|----------------|------|---------------------|
| | | | |

## Problemas y pain points
**Problema central:**
**Por qué las alternativas se quedan cortas:**
-
**Costo para el cliente:**
**Tensión emocional:**

## Panorama competitivo
**Directos:** [Competidor] — se queda corto porque...
**Secundarios:** [Enfoque] — se queda corto porque...
**Indirectos:** [Alternativa] — se queda corto porque...

## Diferenciación
**Diferenciadores clave:**
-
**Cómo lo hacemos diferente:**
**Por qué es mejor:**
**Por qué los clientes nos eligen:**

## Objeciones
| Objeción | Respuesta |
|----------|-----------|
| | |

**Anti-persona:**

## Dinámica de cambio
**Push:**
**Pull:**
**Hábito:**
**Ansiedad:**

## Lenguaje del cliente
**Cómo describen el problema:**
- "[literal]"
**Cómo nos describen:**
- "[literal]"
**Palabras a usar:**
**Palabras a evitar:**
**Glosario:**
| Término | Significado |
|---------|-------------|
| | |

## Voz de marca
**Tono:**
**Estilo:**
**Personalidad:**

## Pruebas y evidencias
**Datos/métricas:**
**Sectores atendidos:**
**Testimonios:**
> "[cita]" — [quién]

## Objetivos
**Meta de negocio:**
**Acción de conversión:**
**Métricas actuales:**
```

---

## Paso 4: Confirmar y guardar

- Mostrar el documento completado
- Preguntar si algo necesita ajuste
- Guardar en `.agents/product-marketing-context.md`
- Indicar: "Los demás skills de marketing usarán este contexto automáticamente."

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
      "content": "Eres un estratega senior de marketing B2B especializado en empresas industriales de tecnología del agua e instrumentación en México. Tu cliente es ISISA Desinfección, Instrumentación y Servicio (isisainst.com.mx), con más de 10 años en el mercado. Produce outputs estructurados en Markdown. Idioma: español mexicano formal/técnico. Sé específico, usa datos concretos, evita generalidades de marketing genérico."
    },
    {
      "role": "user",
      "content": "Con base en el siguiente contexto de ISISA, {{tarea_específica}}:\n\nCONTEXTO:\n{{contenido_product_marketing_context}}"
    }
  ]
}
```

**Variables de entorno en n8n:**
- `ISISA_CONTEXT_PATH`: `.agents/product-marketing-context.md`
- `ISISA_BRAND_VOICE`: "Técnico pero accesible, orientado a ROI, español mexicano formal"

---

## Tips

- **Sé específico**: "¿Cuál es la queja #1 que lleva a los clientes a contactarte?" en lugar de "¿Qué problema resuelven?"
- **Captura palabras exactas**: El lenguaje del comprador industrial supera las descripciones pulidas
- **Pide ejemplos**: "¿Puedes darme un ejemplo?" desbloquea mejores respuestas
- **Valida al avanzar**: Resumir cada sección y confirmar antes de continuar
- **Omite lo que no aplique**: No todas las secciones aplican a todos los proyectos de ISISA
