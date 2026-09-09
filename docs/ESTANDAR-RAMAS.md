# Estandar de Ramas - Git Flow BIT

## Ramas principales (nunca reciben commit directo)

- `master`  -> produccion
- `develop` -> integracion de desarrollo

## Ramas auxiliares

| Tipo | Formato | Ejemplo |
|---|---|---|
| feature | `feature/{{funcionalidad}}` | `feature/catalogo-p004` |
| qa | `qa` / `qa-bit` / `qa-{{ambiente cliente}}` | `qa-bit` |
| bug | `bug/{{id dashboard}}` | `bug/7899` |
| hotfix | `hotfix/{{requerimiento}}-{{id dashboard}}` | `hotfix/precio-1234` |

## Reglas

1. Una rama = una intencion. Si son dos cosas, son dos ramas.
2. Nombres en minuscula, sin espacios, sin acentos, separados por guion.
3. La rama se borra despues del merge. No se acumulan ramas muertas.
4. `feature` y `bug` nacen de `develop`. `hotfix` nace de `master`.
