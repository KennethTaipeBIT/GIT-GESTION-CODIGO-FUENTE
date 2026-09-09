# Estandar de Commits - BIT

## Formato

```
[TIPO]: cuerpo
```

## Tipos permitidos

| Tipo | Cuando se usa |
|---|---|
| `[ADD]` | Se genera una nueva funcionalidad |
| `[FIX]` | Se soluciona un bug |
| `[REFACTOR]` | Refactorizacion y mejoras |

## Reglas del cuerpo

- Maximo **50 caracteres**.
- Idioma **espanol**.
- Explica el **QUE** y el **POR QUE**, no el **COMO**.
- Sin punto final. Sin "cambios varios", "arreglos", "wip", "asdf".

## Ejemplos correctos

```
[ADD]: Creacion de ficha de producto P-004
[FIX]: Correccion de precio erroneo en P-003
[REFACTOR]: Normalizacion de categorias del catalogo
```

## Ejemplos incorrectos

```
cambios            -> sin tipo, sin contexto
[ADD] arregle todo -> falta ':', cuerpo vago
[NEW]: ...         -> tipo no permitido
[FIX]: se modifico el archivo INDICE.md agregando la fila del producto  -> explica el COMO y excede 50 caracteres
```
