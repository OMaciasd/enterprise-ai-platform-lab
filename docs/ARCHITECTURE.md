# Architecture

## Objetivo

Definir una plataforma empresarial integral de AI Engineering que sea
comprensible, verificable, segura y reversible. La arquitectura se documenta
antes de construir para evitar duplicación y decisiones implícitas.

Este documento describe la arquitectura objetivo a alto nivel. La evaluación
detallada de componentes, licencias, costes y reutilización se realizará en la
Fase 0.

## Principios

1. **REUSE BEFORE BUILD**: inventariar y evaluar activos existentes antes de
   crear componentes nuevos.
2. **Reversibilidad**: cada fase debe poder revertirse sin dejar estado
   irrecuperable.
3. **Seguridad por defecto**: mínimo privilegio, secretos fuera del repositorio,
   aislamiento y trazabilidad.
4. **Portabilidad**: evitar dependencias innecesarias de un proveedor concreto.
5. **Observabilidad**: toda capacidad debe poder medirse y diagnosticarse.
6. **Gobierno**: propietarios, políticas, linaje, licencias y uso aceptable.
7. **Documentación de límites**: diferenciar PoC de experiencia profesional
   real.

## Capas

| Capa | Responsabilidad | Ejemplos |
| --- | --- | --- |
| Experiencia | Interfaces de usuario y APIs de negocio | Portales, asistentes, APIs |
| Orquestación | Coordinación de agentes, flujos y herramientas | Agentic AI, workflows |
| Conocimiento | Recuperación y contexto | RAG, Graph RAG, grafos |
| Modelos | Entrenamiento, ajuste y serving | Modelos abiertos, SaaS |
| Datos | Ingestión, calidad, linaje y almacenamiento | Pipelines, catálogos |
| Plataforma | Ejecución y operación | Kubernetes, colas, almacenamiento |
| Seguridad y gobierno | Identidad, secretos, políticas y auditoría | IAM, policy as code |
| Entrega | CI/CD y DevSecOps | Pipelines, escaneos, artefactos |
| Observabilidad | Métricas, logs, trazas y alertas | OpenTelemetry, dashboards |
| Recuperación | Copias, restauración y continuidad | Backups, DR, runbooks |

## Despliegue híbrido

La plataforma se compone de tres entornos con criterios explícitos:

- **Local**: desarrollo, pruebas unitarias, componentes sin dependencia de
  servicios externos y aprendizaje.
- **SaaS gratuito**: validación de integraciones con niveles gratuitos,
  asumiendo límites de uso, privacidad y disponibilidad.
- **Cloud / sandbox**: reproducción de escenarios cercanos a producción con
  coste controlado y destrucción planificada.

Cada componente deberá declarar:

- Entorno recomendado y alternativas.
- Requisitos de datos y tratamiento de información sensible.
- Coste esperado y mecanismo de control.
- Dependencias externas y límites conocidos.
- Estrategia de salida o reemplazo.

## Dominios cubiertos

- AI Engineering
- RAG y Graph RAG
- Agentic AI
- MLOps y LLMOps
- APIs
- ERP
- Python, Java y Go
- Kubernetes
- DevSecOps y CI/CD
- Observabilidad
- Seguridad
- Gobierno
- Recuperación

## Flujo de decisión

1. Identificar la necesidad y su alcance.
2. Buscar activos existentes y evaluar reutilización.
3. Registrar la decisión: reutilizar, adaptar, integrar o construir.
4. Definir criterios de aceptación, seguridad y reversión.
5. Implementar en una fase pequeña.
6. Verificar, documentar y decidir el siguiente paso.

## Límites

- Este repositorio es un laboratorio, no un producto ni un servicio.
- Las PoCs no equivalen a experiencia profesional real.
- Las licencias de terceros se respetan y se documentan por separado.
- No se almacenan secretos, credenciales ni datos personales.
