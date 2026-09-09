# Catalogo de Productos - Repositorio de Practica

Repositorio semilla del **Taller de Gestion de Codigo Fuente (SCM)** - BIT, Desarrollo de Software.

## Que es esto

Un catalogo de productos representado en archivos de texto/Markdown.
No hay lenguaje de programacion, ni dependencias, ni compilacion: **el foco es 100% Git**.
Nadie se traba instalando nada.

## Estructura

```
catalogo/
  INDICE.md          <- indice maestro del catalogo (archivo compartido: aqui aparecen los conflictos)
  P-000-plantilla.md <- plantilla de ficha de producto
  P-0XX-*.md         <- una ficha por equipo (archivo propio: aqui NO hay conflictos)
docs/
  ESTANDAR-COMMITS.md
  ESTANDAR-RAMAS.md
  VERSIONES.md       <- historial de versiones (se actualiza en cada release)
.gitignore
README.md
```

## Ramas

| Rama | Rol |
|---|---|
| `master` | Produccion. Solo recibe codigo via `qa` o `hotfix`. Nunca commit directo. |
| `develop` | Integracion de desarrollo. Recibe `feature`, `bug`. Nunca commit directo. |
| `qa` | Candidata a release, ya certificada por el equipo. |
| `feature/*` | Nueva funcionalidad o historia de usuario. |
| `bug/*` | Error reportado por el equipo de pruebas. |
| `hotfix/*` | Defecto critico detectado en produccion. |

## Reglas del taller

1. **Prohibido** hacer commit directo a `master`, `develop` o `qa`.
2. Todo cambio entra por Pull Request.
3. Todo commit cumple el estandar: `[TIPO]: cuerpo` (ver `docs/ESTANDAR-COMMITS.md`).
4. Cada equipo trabaja SOLO en su archivo `catalogo/P-0XX-*.md`, salvo cuando la fase indique lo contrario.

## Requerimiento funcional (ficticio)

> **RF-001 - Catalogo de Productos**
> El area comercial necesita publicar un catalogo unico de productos. Cada producto debe
> tener codigo, nombre, categoria, precio, stock y estado. El catalogo debe contar con un
> indice maestro que liste todos los productos publicados y su version vigente.

## Como empezar

Ver la guia completa: `GUIA-EJERCICIO.md` (entregada por el facilitador).
