---
id: DOC-003
title: Architecture
version: 1.0.0
status: Active
owner: PD Agencia
created: 2026-07-23
last_updated: 2026-07-24
author: PD Content Studio
category: Foundation
tags:
  - architecture
  - system
  - production
related:
  - README.md
  - docs/principles.md
  - docs/production-pipeline.md
  - docs/glossary.md
---

# Arquitectura de PD Content Studio

> **La arquitectura define cómo se organiza el conocimiento de PD Content Studio y cómo se transforma una necesidad de comunicación en un contenido listo para publicar.**

---

# Propósito

Este documento describe la arquitectura conceptual de PD Content Studio.

Su objetivo es garantizar que cualquier integrante del equipo comprenda cómo funciona el sistema, cuáles son sus componentes y cómo interactúan entre sí.

La arquitectura es independiente de la herramienta utilizada para ejecutar el proceso.

---

# Principio fundamental

PD Content Studio es un **motor de producción de contenido impulsado por conocimiento**.

Su función es transformar una necesidad de comunicación en una pieza lista para publicar.

Para lograrlo combina tres elementos:

- El conocimiento permanente de PD Content Studio.
- La identidad del cliente (Workspace).
- La solicitud realizada por la ejecutiva.

El resultado es un **Production Package** listo para producción.

---

# Arquitectura General

```text
                 PD Content Studio

      ┌────────────────────────────┐
      │   Knowledge Base (Core)    │
      │ Frameworks · Diseño · IA   │
      └──────────────┬─────────────┘
                     │
                     │
      ┌──────────────▼─────────────┐
      │ Workspace del Cliente      │
      │ Contexto · Marca · Pilares │
      └──────────────┬─────────────┘
                     │
                     ▼
          Production Pipeline
      ┌────────────────────────────┐
      │ 1. Ideación                │
      │ 2. Producción              │
      │ 3. Diseño                  │
      └──────────────┬─────────────┘
                     │
                     ▼
            Production Package
```

La arquitectura se basa en una separación clara de responsabilidades.

El conocimiento pertenece al sistema.

La identidad pertenece al cliente.

La producción es el proceso que conecta ambos mundos.

---

# Componentes del sistema

PD Content Studio está compuesto por cuatro componentes principales.

## 1. Knowledge Base (Core)

Es el cerebro de PD Content Studio.

Contiene todo el conocimiento reutilizable que puede aplicarse a cualquier cliente.

Ejemplos:

- Frameworks de contenido
- Copywriting
- Storytelling
- Psicología de marketing
- Buenas prácticas de redes sociales
- Diseño visual
- Patrones virales
- Prompts
- Agentes
- Plantillas
- Checklists

Su propósito es responder:

> ¿Cómo producimos contenido de alta calidad?

El Core evoluciona continuamente y nunca depende de un cliente específico.

---

## 2. Workspace

Cada cliente dispone de un Workspace propio.

Su función es almacenar únicamente la información permanente que define la identidad de la marca.

Ejemplo:

```text
clients/

└── restrepo_optica/

    client-context.md

    brand/
        visual-style.md

    content/
        pillars.md

    assets/

    references/
```

El Workspace contiene:

- Contexto del cliente
- Identidad visual
- Pilares de contenido
- Activos gráficos
- Referencias visuales
- Publicaciones anteriores

El Workspace **no almacena metodologías de producción**.

Toda la estrategia reutilizable pertenece al Core.

---

## 3. Production Pipeline

Es el proceso oficial utilizado para producir cualquier contenido.

Siempre sigue las mismas tres fases.

### Fase 1 — Ideación

Transforma una necesidad en propuestas de contenido.

Entradas:

- Workspace
- Objetivo
- Pilar
- Formato
- Indicaciones
- Referencias

Salida:

- Ideas de publicaciones

---

### Fase 2 — Producción

Desarrolla la idea aprobada.

Genera:

- Copy
- Slides
- Caption
- CTA
- Estructura del contenido

---

### Fase 3 — Diseño

Transforma el contenido aprobado en una pieza visual.

Genera:

- Dirección visual
- Recursos gráficos
- Prompts para imágenes
- Presentación PPTX editable
- Material listo para Canva

---

## 4. Production Package

Es el resultado final generado por el sistema.

Dependiendo del formato puede incluir:

- Copy
- Slides
- Caption
- Dirección visual
- Recursos gráficos
- Prompts
- PPTX editable
- Checklist

El Production Package representa la entrega oficial del sistema.

---

# Flujo de Producción

Toda producción sigue el mismo recorrido.

```text
Solicitud de la Ejecutiva
            │
            ▼
Carga del Workspace
            │
            ▼
Consulta del Knowledge Base
            │
            ▼
Production Pipeline

      Fase 1
      Ideación

            ▼

      Aprobación

            ▼

      Fase 2
      Producción

            ▼

      Aprobación

            ▼

      Fase 3
      Diseño

            ▼

Production Package

            ▼

Entrega

            ▼

Aprendizaje

            ▼

Actualización del Knowledge Base
```

La producción termina con una entrega.

El sistema termina cuando ese aprendizaje se convierte en conocimiento reutilizable.

---

# Responsabilidad de cada componente

## Knowledge Base

Responsable de:

- Frameworks
- Copywriting
- Storytelling
- Diseño
- Psicología
- Tendencias
- Patrones
- Agentes
- Prompts
- Metodologías

---

## Workspace

Responsable de:

- Contexto del cliente
- Identidad visual
- Pilares
- Activos
- Referencias
- Publicaciones anteriores

---

## Production Pipeline

Responsable de ejecutar el proceso de producción utilizando el conocimiento del Core y la identidad del Workspace.

---

## Production Package

Responsable de entregar todos los recursos necesarios para publicar el contenido.

---

# Principios Arquitectónicos

Toda mejora realizada en PD Content Studio debe cumplir los siguientes principios.

- El conocimiento debe ser reutilizable.
- La identidad pertenece al Workspace.
- La metodología pertenece al Core.
- Toda producción sigue el mismo Pipeline.
- El sistema debe adaptarse al proceso de PD Agencia, no al contrario.
- La automatización nunca reemplaza la estrategia.

---

# Evolución del sistema

PD Content Studio está diseñado para crecer de forma modular.

Las herramientas pueden cambiar.

Los modelos de IA pueden cambiar.

Las automatizaciones pueden cambiar.

La arquitectura debe permanecer estable.

Toda nueva funcionalidad debe cumplir al menos una de las siguientes condiciones:

- Reduce trabajo manual.
- Incrementa la reutilización.
- Mejora la calidad del contenido.
- Facilita la automatización.
- Simplifica la operación diaria.

Si una mejora no aporta alguno de estos beneficios, probablemente no deba incorporarse al sistema.

---

# Documentos relacionados

- README.md
- principles.md
- production-pipeline.md
- glossary.md