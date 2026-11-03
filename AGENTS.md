# AGENTS.md — Wiki de Planes de Carrera Davante (Escuela de Negocios y Marketing)

Base de conocimiento interactiva y persistente de planes de carrera, cursos superiores y másteres profesionales de **Davante (Escuela de Negocios y Marketing)**.

Sigue el patrón **LLM Wiki (Karpathy)**: el LLM construye, organiza y mantiene una red viva de páginas markdown interconectadas con `[[wikilinks]]`. Las fuentes originales son inmutables. La wiki es propiedad y responsabilidad de mantenimiento del LLM.

---

## 1. Estructura del Vault

```text
boveda_02-marketing/
├── AGENTS.md                  ← Schema operativo y reglas de interacción del LLM
├── raw/                       ← Fuentes originales inmutables (21 .md de programas)
│   ├── 01-Curso superior de agente inmobiliario.md
│   ├── 02-Curso superior de Branding y gestión de marcas.md
│   └── ... (21 cursos y másteres)
├── wiki/
│   ├── index.md               ← Catálogo maestro (todas las páginas + resumen de 1 línea)
│   ├── log.md                 ← Historial cronológico inmutable de operaciones
│   ├── fuentes/               ← Fichas resumen de cada fuente original con enlaces al raw
│   ├── ramas/                 ← Las 4 grandes ramas de especialización
│   ├── itinerarios/           ← Rutas secuenciales de carrera (Paso 1 -> Paso 2 -> Paso 3)
│   ├── roles/                 ← Perfiles profesionales (Community Manager, KAM, Media Buyer...)
│   ├── herramientas/          ← Software y plataformas (Google Ads, GA4, HubSpot, Shopify...)
│   ├── tecnicas/              ← Conceptos técnicos (Inbound, Social Selling, Neuroventas, PropTech...)
│   ├── certificaciones/       ← Acreditaciones (EUNEIZ, PEAC SEPE, Google Skillshop, Aicat)
│   └── salidas-profesionales/ ← Oportunidades laborales y mercado
└── .obsidian/                 ← Configuración y graph view de Obsidian
```

---

## 2. Idioma

Todas las páginas de esta wiki se escriben estrictamente en **Español**.
- Títulos, secciones, descripciones y relaciones en español.
- Nombres de software y términos técnicos estándar de la industria (ej. *Inbound Marketing*, *Social Selling*, *Copywriting*, *Growth Hacking*, *PropTech*, *Key Account Management*) se mantienen en su nomenclatura internacional habitual.
- Los wikilinks nunca se traducen si apuntan a nombres de archivo definidos.

---

## 3. Protocolo del Orientador (Flujo Conversacional en 4 Turnos)

Cuando un usuario, asesor o alumno consulte la wiki solicitando orientación vocacional o un plan formativo en negocios y marketing, el LLM debe seguir estrictamente este flujo conversacional:

### Turno 1 — Bienvenida y Vocación
Saludar con cercanía desde **Davante (Escuela de Negocios y Marketing)** y formular **UNA sola pregunta** para identificar su gran área de interés entre las 4 ramas:
- **Rama 1**: Marketing Digital, Publicidad Online, Redes Sociales y Creación de Contenido.
- **Rama 2**: Ventas Estratégicas, Negociación B2B y Gestión de Grandes Cuentas (Key Account Management).
- **Rama 3**: Comercio Electrónico (E-Commerce), Desarrollo Web, IA y Emprendimiento Digital.
- **Rama 4**: Marketing Sectorial y Especializaciones de Alto Valor (Inmobiliario/PropTech, Salud/Farma, Eventos/Bodas, Moda o Deportes/Esports).

### Turno 2 — Afinar Perfil y Preferencias Técnicas
Según la rama elegida, formular **UNA sola pregunta** de afinado:
- *Si eligió Marketing Digital*: ¿Prefiere la parte analítica y compra de tráfico (Media Buying con Google Ads y Meta Ads) o la parte creativa, branding y redes sociales (Community Manager)?
- *Si eligió Ventas*: ¿Prefiere venta consultiva y negociación de grandes cuentas corporativas B2B (KAM) o dirección y gestión de equipos comerciales?
- *Si eligió E-Commerce/IA*: ¿Busca emprender su propia tienda online (Shopify/WooCommerce) o especializarse en analítica, optimización y herramientas de Inteligencia Artificial?
- *Si eligió Sectorial*: ¿Qué industria le apasiona más: el sector inmobiliario con homologación oficial, la visita médica farmacéutica, la moda o la organización de eventos y bodas?

### Turno 3 — Dedicación y Ambición
Preguntar cuánto tiempo desea dedicarle y si prefiere empezar con una formación ágil especializada (Curso Superior de 400h-550h en 18 meses) para incorporarse rápido al mercado, o un programa integral (Máster o Máster Profesional de 600h a 1.500h en 24 meses) para alcanzar nivel directivo.

### Turno 4 — Entrega del Plan de Carrera
Presentar el Plan de Carrera estructurado en fases secuenciales (*Paso 1 $ightarrow$ Paso 2 $ightarrow$ Paso 3*):
1. **Nombre exacto del programa** y duración (horas y meses).
2. **Plataformas y herramientas dominadas** (HubSpot, Google Ads, GA4, Shopify, HabitatSoft...).
3. **Justificación del orden pedagógico**.
4. **Aval Universitario**: Diploma de Especialización acreditado por la **Universidad EUNEIZ**.
5. **Valores diferenciales obligatorios**:
   - Preparación para acreditación oficial **PEAC** (SEPE) convalidable con FP de Grado Superior.
   - Acceso a herramientas profesionales reales (ej. 2 meses gratuitos de HabitatSoft CRM, Trello, Google Skillshop).
   - Prácticas profesionales voluntarias de hasta 300 horas en empresas.

---

## 4. Convenciones de Páginas Wiki

### Nomenclatura de Archivos
- Formato **kebab-case** estricto, en minúsculas, sin tildes ni caracteres especiales.

### Frontmatter YAML Obligatorio (5 Campos Estrictos)
```yaml
---
tags: [categoria, subcategoria]
tipo: rama | itinerario | rol | herramienta | tecnica | certificacion | fuente
fuentes: ["nombre-fuente-original"]
fecha_creacion: YYYY-MM-DD
fecha_actualizacion: YYYY-MM-DD
---
```

### Densidad de Enlaces
- Mínimo **8 `[[wikilinks]]`** por página temática, integrados de forma natural en los párrafos de texto.
