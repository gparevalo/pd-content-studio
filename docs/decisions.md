---
id: DOC-007
title: Decisions
version: 0.1.0
status: Active
owner: PD Agencia
created: 2026-07-23
last_updated: 2026-07-23
author: PD Content Studio
category: Foundation
tags:
  - decisions
  - adr
  - architecture
related:
  - README.md
  - docs/principles.md
  - docs/architecture.md
  - docs/roadmap.md
---

# Registro de Decisiones

> **Este documento registra las decisiones arquitectónicas más importantes de PD Content Studio.**

Su objetivo es preservar el contexto detrás de cada decisión para evitar que el conocimiento dependa de la memoria de las personas.

---

# ¿Qué es una decisión?

Una decisión es una elección estratégica que afecta el diseño, funcionamiento o evolución de PD Content Studio.

No se registran decisiones operativas o temporales.

Solo aquellas que impactan el sistema a largo plazo.

---

# Formato

Cada decisión debe incluir:

- Contexto
- Decisión
- Justificación
- Consecuencias

---

# ADR-001

## Título

PD Content Studio se construye como un sistema y no como una colección de prompts.

### Contexto

El objetivo del proyecto es crear un activo permanente para PD Agencia.

Depender únicamente de prompts dificulta la reutilización y el crecimiento del conocimiento.

### Decisión

Toda la información relevante será documentada como parte del sistema.

Los prompts serán únicamente una herramienta de ejecución.

### Consecuencias

Positivas

- Mayor reutilización.
- Independencia de la IA utilizada.
- Escalabilidad.

Negativas

- Mayor inversión inicial en documentación.

---

# ADR-002

## Título

La estrategia pertenece a las personas.

### Contexto

La inteligencia artificial puede generar contenido, pero no debe definir el posicionamiento de una marca.

### Decisión

Las decisiones estratégicas serán responsabilidad del equipo de PD Agencia.

La IA ejecutará sobre una estrategia previamente definida.

### Consecuencias

Positivas

- Mayor coherencia.
- Mayor control de calidad.
- Protección del conocimiento estratégico.

---

# ADR-003

## Título

Arquitectura modular.

### Contexto

Mezclar branding, copywriting, diseño y automatización en un mismo documento dificulta el mantenimiento.

### Decisión

Cada documento tendrá una única responsabilidad.

### Consecuencias

Positivas

- Mayor claridad.
- Mejor reutilización.
- Documentación más simple.

---

# ADR-004

## Título

Congelamiento de arquitectura durante un Sprint.

### Contexto

Durante la construcción surgieron múltiples oportunidades de mejora que amenazaban con cambiar constantemente el rumbo del proyecto.

### Decisión

Una vez iniciado un Sprint, la arquitectura queda congelada.

Las nuevas ideas se registran en el backlog y se evalúan al finalizar la versión.

### Consecuencias

Positivas

- Mayor foco.
- Entregas más rápidas.
- Reducción del retrabajo.

Negativas

- Algunas mejoras deberán esperar al siguiente Sprint.

---

# ADR-005

## Título

PD Content Studio será un motor de conocimiento.

### Contexto

El sistema debe servir para múltiples clientes, marcas y canales.

### Decisión

El objetivo principal es construir conocimiento reutilizable.

El contenido será una consecuencia del sistema y no su finalidad.

### Consecuencias

Positivas

- Escalabilidad.
- Reutilización.
- Adaptabilidad a nuevos formatos.

---

# ADR-006

## Título

`production-pipeline.md` es la fuente única de verdad del proceso operativo.

### Contexto

El repositorio mantenía una descripción completa de etapas tanto en Workflow
como en Production Pipeline, con diferente nivel de detalle. Esa duplicación
podía producir instrucciones contradictorias para el equipo y los agentes.

### Decisión

Production Pipeline define etapas, entradas, salidas, aprobaciones y
escenarios. Workflow conserva solo las reglas de gobierno y mejora continua.

### Consecuencias

Positivas

- Un único lugar para actualizar el proceso.
- Menor ambigüedad para Sofi y futuras automatizaciones.
- Mejor trazabilidad de excepciones y aprobaciones.

Negativas

- Todo cambio de proceso requiere actualizar primero el pipeline canónico.

---

# Próximas decisiones

Las siguientes decisiones deberán registrarse conforme evolucione el sistema.

Ejemplos:

- Gestión de Workspaces.
- Biblioteca de activos.
- Automatización.
- Integración con Canva.
- Integración con n8n.
- Agentes especializados.

---

# Historial

| ADR     | Estado |
| ------- | ------ |
| ADR-001 | Activa |
| ADR-002 | Activa |
| ADR-003 | Activa |
| ADR-004 | Activa |
| ADR-005 | Activa |
| ADR-006 | Activa |
