# Plugins

Aquí se documentan los plugins (de asistentes de IA) usados o relevantes en tus proyectos.

**Regla:** un plugin instalado o conectado normalmente no es una carpeta copiable. Solo se guarda un archivo exportable si existe de verdad; si no, se escribe una ficha. No se simulan copias.

## Dónde va cada ficha

`development/`, `database/`, `design/` o `productivity/`, según su categoría. Un archivo `.md` por plugin, con:

- Nombre
- Propósito
- Tipo de proyecto para el que sirve
- Cómo se usa (solo si se conoce)
- Requisitos o dependencias conocidas
- Fuente u origen
- Tipo de recurso: **exportable** (archivo guardado aquí) o **solo documentado**

No incluyas credenciales, tokens, claves API ni datos privados.

## Registro actual

**Ningún plugin de IA identificado.**

Se revisó el proyecto *Electrónica Central AZ* y no hay evidencia verificable de plugins, conectores o servidores MCP:

- No existe ningún archivo de configuración de plugins o MCP (`.mcp.json`, `plugin.json`, `marketplace.json`, `.claude/`, `.cursor/` u otros).
- No aparece ninguno en `skills-lock.json` (solo registra los dos Skills de `skills/frontend/`).

Por eso las carpetas de `plugins/` están vacías (solo `.gitkeep`).

### Aclaración: plugins de herramientas de build

El proyecto sí usa plugins de **herramientas de desarrollo**, que no son plugins de IA y por eso no se catalogan aquí. Quedan solo como referencia, tal como figuran en `package.json` y `vite.config.ts`:

- Vite: `@vitejs/plugin-react` y `@tailwindcss/vite`.
- ESLint: `eslint-plugin-react-hooks` y `eslint-plugin-react-refresh`.

Se recuperan con `npm install` desde el `package.json` del proyecto; no hay nada que copiar.
