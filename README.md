# PBP Consulting — Web Corporativa

## 📋 Descripción
Web corporativa premium para **PBP Consulting**, una consultora especializada en la gestión integral de ayudas, subvenciones y financiación para proyectos de I+D+i en España. Fundada por Carlos Ruzafa Silvestre y Víctor M. Serrano Martínez, investigadores con experiencia real en INESCOP, CDTI, IVACE+i y AEI.

## 🎯 Objetivo
Captar empresas que quieran subcontratar la preparación y gestión de:
- Solicitudes de ayudas públicas (CDTI, IVACE+i, ENISA, etc.)
- Memorias técnicas y planes de explotación
- Estrategias integrales de financiación I+D+i
- Gestión del Sello PYME Innovadora e informes motivados
- Seguimiento y justificación de proyectos financiados

---

## ✅ Funcionalidades implementadas

### Secciones de la web
- **Hero** — Propuesta de valor principal con CTA a reunión gratuita
- **Barra de instituciones** — Programas con los que trabaja PBP Consulting
- **Propuesta de valor** — 4 pilares diferenciadores + alerta de impacto CDTI
- **Servicios** — 6 servicios detallados con listas de entregables
- **Programas de financiación** — 9 programas (CDTI I+D, LIC, NEOTEC, IVACE PIDI-CV, INNOVA-CV, ENISA, Sello PYME, Misiones Ciencia, Deducciones Fiscales)
- **Cifras de impacto** — Estadísticas animadas con IntersectionObserver
- **Proceso de trabajo** — 4 pasos desde diagnóstico hasta justificación
- **Equipo** — Perfiles detallados de Carlos Ruzafa y Víctor Serrano
- **FAQ** — 6 preguntas frecuentes con acordeón interactivo
- **CTA Banner** — Llamada a la acción intermedia
- **Contacto** — Formulario completo con guardado en tabla + información de contacto

### Funcionalidades técnicas
- Navbar transparente → sólido al hacer scroll
- Menú hamburguesa responsive para móvil
- Smooth scroll a secciones
- Animaciones AOS (Animate On Scroll)
- Partículas animadas en el hero
- Contador de estadísticas animado
- Acordeón FAQ interactivo
- Formulario con validación y guardado en tabla API
- Enlace activo en navbar según sección visible
- Botón "volver arriba"
- Sticky CTA en móvil

---

## 📁 Estructura de archivos

```
/
├── index.html          — Página principal completa
├── css/
│   └── style.css       — Hoja de estilos premium (paleta verde petróleo)
├── js/
│   └── main.js         — JavaScript: interactividad, formulario, animaciones
└── images/
    └── logo.png        — Logo circular PBP Project (verde petróleo)
```

---

## 🔗 URIs y navegación

| Sección | Ancla |
|---------|-------|
| Inicio / Hero | `#inicio` |
| Servicios | `#servicios` |
| Programas de financiación | `#programas` |
| Cómo trabajamos | `#proceso` |
| Equipo | `#equipo` |
| Contacto | `#contacto` |

---

## 🗄️ Modelo de datos — Tabla `leads`

Los leads del formulario de contacto se guardan en la tabla `leads` de la API REST:

| Campo | Tipo | Descripción |
|-------|------|-------------|
| `nombre` | text | Nombre del contacto |
| `empresa` | text | Nombre de la empresa |
| `email` | text | Email de contacto |
| `telefono` | text | Teléfono (opcional) |
| `sector` | text (enum) | Sector de actividad |
| `ayuda` | text (enum) | Programa de interés |
| `mensaje` | rich_text | Descripción del proyecto |
| `fecha` | datetime | Timestamp de envío |
| `estado` | text (enum) | Estado del lead (nuevo/contactado/propuesta/cliente/descartado) |

**API endpoint**: `tables/leads` (GET, POST, PATCH, DELETE)

---

## 📞 Contactos del equipo

| Persona | Email |
|---------|-------|
| Carlos Ruzafa Silvestre | carlos17rs@gmail.com |
| Víctor M. Serrano Martínez | vitikor97@gmail.com |
| General / Gestión | pbproject.es@gmail.com |

---

## 🎨 Identidad visual

- **Color primario**: Verde petróleo oscuro `#1d4a47` (extraído del logo)
- **Acento**: Teal `#4db6a8`
- **Fondos**: Crema `#f8f5ef` y blanco `#ffffff`
- **Tipografías**: Fraunces (titulares) + Inter (cuerpo)
- **Estilo**: Minimalista, premium, corporativo

---

## 🚀 Próximos pasos recomendados

1. **Dominio propio** — Registrar `pbpconsulting.es` o `pbp-consulting.com`
2. **Foto de perfil real** — Sustituir las iniciales del equipo por fotos reales
3. **Casos de éxito** — Añadir sección con proyectos reales financiados (cuando tengáis clientes)
4. **Blog / Noticias** — Artículos sobre convocatorias abiertas para SEO
5. **Google Analytics** — Seguimiento de conversiones del formulario
6. **Integración de email** — Conectar el formulario a un servicio de email (Mailchimp, Brevo)
7. **Calendario Calendly** — Botón de reserva de reunión directamente en la web
8. **Testimonios** — Añadir reseñas de primeros clientes

---

## 📅 Creado
Marzo 2025 — PBP Consulting
