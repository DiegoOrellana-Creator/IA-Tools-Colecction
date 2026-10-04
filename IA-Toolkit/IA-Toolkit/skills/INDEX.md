# Índice de Skills

Los Skills de esta carpeta son copias **íntegras y sin modificar** de los que estaban en `.agents/skills/` del proyecto *Electrónica Central AZ* (frontend React + TypeScript + Vite + Tailwind).
El archivo `skills-lock.json` de esta carpeta es la copia sin cambios del registro de instalación de ese proyecto.

Fecha de incorporación a IA-Toolkit: 2026-10-03.

---

## frontend/design-taste-frontend

| Campo | Valor |
|---|---|
| Ruta | `skills/frontend/design-taste-frontend/` |
| Archivos | `SKILL.md` (1206 líneas). No hay archivos adicionales en el original. |
| Descripción (del propio Skill) | Skill "anti-slop" de frontend para landing pages, portfolios y rediseños: infiere la dirección de diseño del brief y evita interfaces con aspecto genérico. |
| Fuente | `Leonxlnx/taste-skill` (GitHub), ruta `skills/taste-skill/SKILL.md`. Según `skills-lock.json`. |
| Proyecto donde se utilizó | Presente en *Electrónica Central AZ*. Instalado el 2026-09-30 según la fecha de los archivos. |
| Licencia | MIT, © 2026 Leonxlnx. Verificada en el README del repositorio de origen. El `SKILL.md` no incluye texto de licencia. |
| Hash del lock | `899b84384f74f540ea5284d9b2e9234e050998b42eacc805410b518d4226c0b3` |

Notas de uso (tomadas del propio Skill): su encabezado indica que es para "landing pages, portfolios y rediseños. No dashboards, no tablas de datos, no UI de producto de varios pasos". Un panel administrativo como *Electrónica Central AZ* queda fuera de ese alcance declarado.
El repositorio de origen identifica la versión actual de este Skill como v2 (experimental), con la v1 disponible por separado como `design-taste-frontend-v1`. No se comprobó cuál de las dos corresponde exactamente a esta copia.

## frontend/web-design-guidelines

| Campo | Valor |
|---|---|
| Ruta | `skills/frontend/web-design-guidelines/` |
| Archivos | `SKILL.md` (1270 bytes). No hay archivos adicionales en el original. |
| Descripción (del propio Skill) | Revisa código de interfaz según las Web Interface Guidelines (accesibilidad, UX, buenas prácticas). |
| Fuente | `vercel-labs/agent-skills` (GitHub), ruta `skills/web-design-guidelines/SKILL.md`. Según `skills-lock.json`. Metadatos del Skill: autor `vercel`, versión `1.0.0`. |
| Proyecto donde se utilizó | Presente en *Electrónica Central AZ*. Instalado el 2026-09-30 según la fecha de los archivos. |
| Licencia | **No verificada de primera mano.** Una fuente de terceros indica MIT "según el README, sin archivo LICENSE". Confírmala en el repositorio antes de redistribuir. |
| Hash del lock | `d8e7d3afe37dcc8a97b99ffb5afdb4d0919ae0092ea8b68f44eb201f035e33ac` |

Dependencia externa: este Skill no contiene las reglas. Indica que se descarguen en cada revisión desde
`https://raw.githubusercontent.com/vercel-labs/web-interface-guidelines/main/command.md`,
por lo que necesita acceso a internet y a una herramienta de descarga web. Las reglas pueden cambiar con el tiempo.

---

## Limitaciones conocidas

- Se verificó que los Skills están presentes en el proyecto y registrados en `skills-lock.json`. **No se pudo verificar en qué tareas concretas se aplicaron.**
- El hash `computedHash` del lock no coincide con el SHA-256 del `SKILL.md` copiado. El algoritmo que usa el instalador no está documentado en los archivos, así que no se puede confirmar la integridad frente al original. Los SHA-256 de los archivos copiados son:
  - `design-taste-frontend/SKILL.md`: `2e064e92aca020b2e0bad69326fe7ea55d59005ed53d1a8cbce1bd135d44b8b3`
  - `web-design-guidelines/SKILL.md`: `17e48da905f83a19c174079b50760a98c069527ba50079239b3c187236627c29`
- Ambos archivos usan saltos de línea CRLF; pueden diferir del original solo en eso. No se modificaron.
