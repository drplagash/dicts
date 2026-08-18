<p align="center">
  <img src="docs/portada.svg" alt="Credential Dictionaries" width="100%">
</p>

# dicts

Diccionarios privados de Oráculo SOC.

Este repo es para uso interno. Acá no quiero una vidriera llena de carpetas raras: quiero abrir, encontrar las claves, encontrar los pares usuario/password y seguir trabajando como una persona normal, no como un arqueólogo de YAML.

## Acceso rápido

| Quiero ver | Archivo |
|---|---|
| Listado actualizado de claves/passwords | [`raw/passwords.txt`](raw/passwords.txt) |
| Pares usuario/password observados | [`raw/userpass.observed.tsv`](raw/userpass.observed.tsv) |

Esos son los dos archivos principales. La rutina debería mantenerlos actualizados.

## Para análisis interno

- `raw/passwords.txt`: lista directa de claves observadas.
- `raw/userpass.observed.tsv`: pares usuario/password observados, con contexto de aparición cuando aplique.

No usar la vista con `***` para análisis interno. Los archivos masked existen solo para exportar o mostrar sin exponer valores completos. Para mí, en privado, se usa la vista legible.

## Hashes

Los hashes se dejan en `derived/` para control, comparación y export seguro. No son el camino principal para revisar el repo.

## Qué no mirar primero

- `derived/`: transformaciones, hashes y versiones masked.
- `metadata/`: manifiestos y contexto técnico.
- `docs/`: assets y documentación auxiliar.

Sirven, pero no son la entrada humana principal.

## Regla simple

Para trabajar:

```text
raw/passwords.txt
raw/userpass.observed.tsv
```

Para exportar o mostrar algo sin valores completos:

```text
derived/
```

## Nota

Este repo debe seguir privado. El material público va en `payloads`. Los diccionarios son material operativo interno.
