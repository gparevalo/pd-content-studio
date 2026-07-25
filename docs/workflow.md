---
id: DOC-004
title: Workflow Governance
version: 0.2.0
status: Active
owner: PD Agencia
created: 2026-07-23
last_updated: 2026-07-25
author: PD Content Studio
category: Foundation
related:
  - docs/production-pipeline.md
  - docs/architecture.md
  - docs/principles.md
---

# Gobierno del workflow

> Este documento establece las reglas de gobierno del ciclo de producción. No define las etapas operativas.

## Fuente de verdad

`docs/production-pipeline.md` es la única fuente de verdad para las etapas,
entradas, salidas, criterios de avance, aprobaciones y escenarios de
producción. Todo documento, agente o automatización debe referirse a ese
pipeline en lugar de reproducirlo.

## Propósito

Garantizar que el proceso sea consistente, auditable y capaz de incorporar
aprendizajes sin duplicar reglas en distintos documentos.

## Reglas de gobierno

- Toda solicitud debe tener un Workspace identificado antes de producir.
- Las excepciones al pipeline se documentan en el Production Package.
- Ninguna fase que requiera aprobación avanza sin la aprobación indicada.
- Los resultados de medición y revisión generan un aprendizaje o una decisión
  explícita de no actualizar el conocimiento.
- Los cambios permanentes de proceso se registran en `docs/decisions.md` y se
  implementan primero en el pipeline canónico.

## Ciclo de mejora

Después de la entrega, el equipo registra resultados y decide si corresponde:

- actualizar un Framework o patrón reutilizable;
- actualizar el Workspace del cliente;
- crear una decisión arquitectónica; o
- conservar el conocimiento solo en el Production Package, si es específico a
  una entrega.

## Alcance

Este documento no sustituye el brief de una solicitud ni define una plantilla
de entregable. Esas responsabilidades pertenecen, respectivamente, a
`docs/design-brief-specification.md` y al Production Pipeline.
