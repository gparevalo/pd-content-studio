---
id: DOC-012
title: Ejemplos de Solicitudes
version: 0.1.0
status: Active
owner: PD Agencia
created: 2026-07-25
last_updated: 2026-07-25
author: PD Content Studio
category: Operation
related:
  - docs/production-pipeline.md
  - docs/design-brief-specification.md
  - docs/reference-analysis.md
  - docs/AI_CONTEXT.md
---

# Ejemplos de solicitudes para PD Content Studio

> Usa estos mensajes como punto de partida. Completa solo la información que ya esté aprobada; no es necesario repetir el contexto que ya vive en el Workspace del cliente.

## 1. Crear un nuevo cliente

Adjunta el manual de marca, los logos y cualquier recurso disponible junto con este mensaje:

```text
Sofi, crea el Workspace para este nuevo cliente.

Nombre de marca: [nombre]
Industria: [industria]
Ubicación: [ciudad/país, si aplica]
Descripción del negocio: [descripción aprobada]
Propuesta de valor: [propuesta aprobada]
Productos o servicios: [lista]
Audiencia principal: [audiencia]
Objetivo de comunicación: [objetivo]
Tono de marca: [tono]
Restricciones: [legales, médicas, comerciales o de lenguaje]

Adjunto: manual de marca, logos, tipografías, fotografías, plantillas y referencias disponibles.

No inventes información que no esté en los adjuntos. Indica qué campos quedan pendientes antes de activar el Workspace.
```

**Resultado esperado:** un Workspace con `client-context.md`, `brand/visual-style.md`, `content/pillars.md`, y las carpetas de activos y referencias. Si falta información, el Workspace queda en estado `Draft`.

## 2. Solicitar un carrusel o post fijo

El sistema carga automáticamente el contexto del cliente. Indica el objetivo y el tema, sin repetir el manual de marca.

```text
Sofi, necesito un [carrusel / post fijo] para [cliente].

Objetivo: [educar / generar confianza / informar / convertir]
Tema: [tema específico]
Audiencia: [audiencia, si cambia de la habitual]
Pilar: [pilar del cliente, si lo conoces]
Formato: [carrusel de X slides 4:5 / post fijo 4:5 / otra medida]
CTA: [acción esperada]
Información aprobada que debe incluir: [texto, datos o mensajes]
Restricciones: [lo que no debe decir o mostrar]

Primero propón [número] ideas con hook y enfoque. Espera mi aprobación antes de desarrollar el copy y el diseño.
```

### Si ya tienes el copy aprobado

```text
Sofi, necesito diseñar un [carrusel / post fijo] para [cliente].

El copy adjunto está aprobado. No modifiques su mensaje sin consultarme.
Formato: [medida y número de slides, si aplica]
CTA: [CTA aprobado]
Recursos que deben usarse: [logos, fotos, productos o enlaces]

Carga el Workspace del cliente y propón la dirección visual antes de generar los entregables.
```

**Resultado esperado:** idea aprobada, copy o estructura, dirección visual y el Production Package aplicable al formato solicitado.

## 3. Enviar referencias para adaptar al manual de marca

Adjunta las imágenes, enlaces, PDF o capturas de las referencias y usa este mensaje:

```text
Sofi, adjunto [cantidad] referencias para una pieza de [cliente].

Objetivo de la nueva pieza: [objetivo]
Formato: [carrusel / post fijo / reel / otro]
Tema o mensaje: [tema]

Analiza las referencias usando el manual de marca ya cargado en el Workspace de [cliente].

De cada referencia necesito que identifiques:
- qué funciona en el hook, la estructura y la composición;
- qué patrones visuales o narrativos podemos adaptar;
- qué no debemos replicar;
- cómo se traducirá al estilo, colores, tipografías y restricciones de la marca.

No copies la referencia. Primero entrega el análisis y una propuesta original de dirección visual para mi aprobación.
```

### Qué conviene adjuntar

- La referencia original, no solo una descripción.
- El enlace de origen cuando esté disponible.
- Una nota breve sobre qué te interesa de ella: por ejemplo, *“me gusta la jerarquía del titular”* o *“quiero una sensación de calma similar”*.
- Fotografías o productos obligatorios, si deben aparecer.

**Resultado esperado:** análisis de principios reutilizables, propuesta visual adaptada al cliente y una ejecución original. Las referencias inspiran; nunca se reproducen literalmente.
