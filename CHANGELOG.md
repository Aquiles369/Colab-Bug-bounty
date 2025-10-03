# Changelog

Todas las modificaciones notables en este proyecto se listan por versión.

## [Unreleased]
- Preparando v0.2: mejoras en UI, optimización de export/import y tests automáticos.
- Añadir opción de cifrado local para campos sensibles (plan).
- Mejoras en accesibilidad y mobile UX.

## v0.1 - 2025-10-03
### Added
- Panel web local (.html/.js) para gestión colaborativa de reports de bug bounty.
- Búsqueda rápida por **ID de informe**.
- CRUD completo: añadir/editar/borrar filas y columnas (incluye "eliminar última fila").
- Selección múltiple con casillas para editar/borrar en lote.
- Export / Import en **JSON** y **CSV** para compartir con colegas.
- Persistencia en **localStorage** (offline, sin dependencias externas).
- Indicador visual en **Notas** (círculo rojo cuando hay contenido).
- Estados coloreados para **Severidad** (Crítica/Alta/Media/Baja/Info) y **Triage** (triage/resolver/dupe/auto-close/pendiente/pelear).
- Tabla principal con 10 columnas predeterminadas:
  - Título del reporte
  - ID de informe
  - Fecha de reporte
  - Encontrado por
  - Reportado por
  - Severidad / Estado
  - Triage / Estado de gestión
  - Bounty — quien cobró
  - Bounty — mi parte / total pagado
  - Notas (texto largo; indicador visual si no vacío)
- Demo GIF + walkthrough (ver carpeta `assets` / README).
- Quickstart documentado (abrir localmente o via simple server).

### Changed
- Estructura del proyecto organizada: `web/`, `assets/`, `docs/`, `CHANGELOG.md`.

### Fixed
- Correcciones menores de estilo y compatibilidad en tablas.
- Ajustes en la detección del indicador de notas (bugs UI corregidos).

### Security
- Herramienta marcada **lab-only**: no ejecutar contra sistemas sin permiso.
- Recomendación explícita: evitar guardar datos sensibles en repos públicos.
- Política: PoC y ejemplos sanitizados para demos.

## v0.0 - 2025-09-28
- Versión inicial: prototipo funcional con almacenamiento local y operaciones básicas CRUD.
