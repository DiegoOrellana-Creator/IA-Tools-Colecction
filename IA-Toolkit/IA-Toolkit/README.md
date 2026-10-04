# IA-Toolkit

Colección personal y reutilizable de **Skills**, **Plugins** y **Prompts** para trabajar con asistentes de IA.
La idea es no empezar de cero en cada proyecto: se eligen aquí los recursos que hagan falta y se llevan al proyecto nuevo.

> Solo se incluyen recursos que existen realmente o que se pudieron identificar de forma verificable.
> Los Skills se conservan **sin modificar**. Cuando algo no se puede exportar como archivo, se documenta, no se simula.

## Estructura

```text
IA-Toolkit/
├── README.md
├── skills/
│   ├── INDEX.md             Registro de origen, licencia y notas de cada Skill
│   ├── skills-lock.json     Registro original del instalador de skills (copia sin cambios)
│   ├── frontend/
│   ├── backend/
│   ├── database/
│   └── general/
├── plugins/
│   ├── README.md            Cómo se documentan los Plugins + registro actual
│   ├── development/
│   ├── database/
│   ├── design/
│   └── productivity/
└── prompts/
    ├── frontend/
    ├── backend/
    ├── database/
    ├── design/
    └── general/
```

Las carpetas sin contenido conservan un `.gitkeep` solo para que Git las mantenga. Se pueden borrar cuando la carpeta tenga archivos.

## Skills

Un Skill es una carpeta con un `SKILL.md` (y, si los tiene, sus archivos de apoyo: referencias, scripts, ejemplos) que un agente de IA carga cuando la tarea lo requiere.

- Se organizan por categoría: `frontend/`, `backend/`, `database/` y `general/`.
- Cada Skill se guarda **completo**, con la estructura de carpetas original y sin editar su contenido.
- El origen, la licencia y las notas de uso de cada uno están en [`skills/INDEX.md`](skills/INDEX.md).

Skills actuales:

| Skill | Categoría | Origen |
|---|---|---|
| `design-taste-frontend` | frontend | github.com/Leonxlnx/taste-skill |
| `web-design-guidelines` | frontend | github.com/vercel-labs/agent-skills |

Para usar uno en otro proyecto, copia su carpeta completa al directorio de skills de tu agente. En el proyecto de origen estaban en `.agents/skills/<nombre>/`.

## Plugins

Un Plugin instalado o conectado en una herramienta de IA normalmente **no es una carpeta que se pueda copiar**: vive en la cuenta o la configuración de la herramienta.
Por eso, en `plugins/` solo se guarda un recurso exportable si existe de verdad. En los demás casos se escribe una ficha de documentación (propósito, uso, requisitos, origen).

El formato de la ficha y el registro actual están en [`plugins/README.md`](plugins/README.md). Las subcarpetas (`development/`, `database/`, `design/`, `productivity/`) son la categoría de cada ficha.

## Prompts

`prompts/` está pensado para prompts reutilizables por tipo de tarea: `frontend/`, `backend/`, `database/`, `design/` y `general/`.
Todavía no contiene prompts.

## Reutilización

Nada aquí es obligatorio ni va en bloque. Para un proyecto nuevo:

1. Revisa `skills/INDEX.md` y `plugins/README.md` para ver qué hay.
2. Copia solo los Skills y prompts que apliquen.
3. Revisa las notas de uso: algunos Skills están pensados para un tipo concreto de interfaz y pueden no encajar en otro.
4. Respeta la licencia y la atribución de cada recurso (ver `skills/INDEX.md`).

## Nota sobre saltos de línea

Los `SKILL.md` copiados usan saltos de línea de Windows (CRLF), igual que en el proyecto de origen. No se convirtieron para mantener la copia idéntica. Si usas Git en Windows, conviene evitar que normalice esos archivos (por ejemplo con un `.gitattributes` que marque `skills/**` como `-text`).
