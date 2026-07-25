---
id: DOC-011
title: Production Pipeline
version: 1.1.0
status: Active
owner: PD Agencia
created: 2026-07-24
last_updated: 2026-07-25
author: PD Content Studio
category: Core
related:
  - docs/workflow.md
  - docs/design-brief-specification.md
  - docs/reference-analysis.md
  - docs/architecture.md
  - team/sofi.md
---

# Production Pipeline

> Proceso operativo canónico de PD Content Studio.

## Autoridad y propósito

Este documento es la única fuente de verdad para producir contenido. Define las
etapas, sus entradas y salidas, los puntos de aprobación y los escenarios de
inicio. Los demás documentos pueden aportar contexto, pero no redefinir este
flujo.

Su propósito es transformar una necesidad de comunicación en un Production
Package y convertir los aprendizajes relevantes en conocimiento reutilizable.

## Entradas mínimas

- Workspace del cliente identificado.
- Objetivo de comunicación.
- Formato o canal solicitado.

Cuando existan, también se reciben pilar, tema, copy aprobado, indicaciones,
recursos, PDF o referencias. Si falta una entrada mínima, se solicita antes de
iniciar la fase que la necesita.

## Flujo canónico

| Etapa | Objetivo | Salida | Gate |
| --- | --- | --- | --- |
| 1. Solicitud y brief | Registrar necesidad, restricciones y responsable. | Brief verificable. | Brief completo. |
| 2. Workspace | Cargar contexto, identidad, pilares y recursos. | Contexto aplicable. | Cliente identificado. |
| 3. Objetivo | Definir resultado, audiencia y CTA esperado. | Objetivo validado. | Aprobación estratégica cuando aplique. |
| 4. Investigación | Reunir información confiable y aprobada. | Hallazgos validados. | Datos aptos para uso. |
| 5. Referencias y patrones | Analizar sin copiar. | Principios reutilizables. | Sin replicación literal. |
| 6. Framework | Seleccionar la estructura adecuada. | Framework justificado. | Alineación con objetivo. |
| 7. Ideación | Proponer enfoques, hooks o ideas. | Idea aprobada. | Aprobación de idea. |
| 8. Producción | Desarrollar copy, guion, slides, caption y CTA. | Contenido aprobado. | Aprobación de contenido. |
| 9. Diseño | Definir dirección visual y producir los recursos requeridos. | Pieza lista para QA. | Respeto al Workspace. |
| 10. Control de calidad | Validar exactitud, marca, legibilidad y formato. | QA aprobado o ajustes. | Aprobación final. |
| 11. Entrega | Preparar el paquete acordado para cliente o publicación. | Production Package. | Entrega registrada. |
| 12. Medición | Registrar resultados disponibles. | Métricas o ausencia justificada. | Información documentada. |
| 13. Aprendizaje | Actualizar el sistema cuando el hallazgo sea reutilizable. | Cambio, decisión o nota de no acción. | Conocimiento trazable. |

## Escenarios de inicio

- **Ideas desde cero:** iniciar en etapas 1–7 y esperar aprobación de idea.
- **Copy aprobado:** verificar Workspace y objetivo; iniciar en etapa 9, salvo
  que el copy requiera correcciones autorizadas.
- **PDF:** iniciar en investigación para extraer, validar y adaptar el material.
- **Referencia visual:** iniciar en referencias y patrones; nunca reproducirla.
- **Solo diseño:** verificar que copy, formato y recursos estén aprobados antes
  de iniciar diseño.

## Reglas de avance

- No se avanza desde ideación, producción o QA sin el gate correspondiente.
- La IA no inventa información, cambia estrategia ni modifica mensajes
  aprobados sin autorización.
- Las referencias generan aprendizajes, no copias.
- Las afirmaciones de salud requieren información aprobada por el cliente o
  responsable designado; si no existe, se detiene y se solicita validación.

## Production Package

El paquete reúne únicamente los componentes aplicables: brief, copy, guion o
slides, caption, CTA, dirección visual, recursos, prompts, archivo editable,
resultado de QA, aprobaciones y aprendizaje. Debe permitir reconstruir la
decisión sin depender de una conversación previa.
