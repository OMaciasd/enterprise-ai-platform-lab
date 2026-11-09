# Enterprise AI Platform Lab

Laboratorio de referencia para el diseño, construcción y operación de una
**plataforma empresarial integral de AI Engineering**.

El objetivo no es acumular demos aisladas, sino demostrar criterio de
arquitectura, gobierno, seguridad y operación sobre un conjunto coherente de
capacidades, con decisiones trazables y artefactos reproducibles.

## Propósito

Este laboratorio integra, de forma incremental y verificable, las siguientes
áreas:

- AI Engineering: datos, features, evaluación, prompting, fine-tuning y
  serving de modelos.
- RAG y Graph RAG: ingestión, indexación, recuperación híbrida, reranking,
  trazabilidad de fuentes y grafos de conocimiento.
- Agentic AI: orquestación de agentes, herramientas, memoria, guardrails y
  evaluación de comportamiento.
- MLOps / LLMOps: versionado, experimentación, despliegue, monitoreo,
  evaluación continua y ciclo de vida de modelos y prompts.
- APIs: contratos, versionado, seguridad, cuotas y observabilidad.
- ERP: integración de procesos empresariales y datos maestros.
- Python, Java y Go: elección de lenguaje según el problema, no por moda.
- Kubernetes: despliegue, escalado, aislamiento y operación de cargas.
- DevSecOps y CI/CD: automatización, análisis de seguridad y entrega
  progresiva.
- Observabilidad: métricas, logs, trazas y correlación extremo a extremo.
- Seguridad: identidad, secretos, aislamiento, cumplimiento y respuesta.
- Gobierno: catálogo, propietarios, políticas, linaje y uso aceptable.
- Recuperación: copias, restauración, continuidad y planes de recuperación.

## Arquitectura híbrida

El laboratorio se apoya en una arquitectura híbrida:

- **Local**: ejecución en el equipo de desarrollo para aprendizaje, pruebas y
  componentes que no requieren infraestructura externa.
- **SaaS gratuito**: servicios gestionados con niveles gratuitos para validar
  integraciones sin coste inicial.
- **Cloud / sandbox**: entornos temporales y de bajo coste para reproducir
  escenarios cercanos a producción.

La elección de cada ubicación se documentará con criterios explícitos de coste,
seguridad, portabilidad, límites de uso y reversibilidad.

## Principio rector: REUSE BEFORE BUILD

Antes de crear cualquier componente, se debe:

1. Inventariar los repositorios, laboratorios y activos existentes.
2. Evaluar su calidad, licencia, mantenimiento, seguridad y encaje.
3. Decidir de forma explícita entre reutilizar, adaptar, integrar o construir.
4. Registrar la decisión y su justificación.

No se crearán componentes duplicados si existe un activo reutilizable que
cubra la necesidad con un coste razonable.

## PoC frente a experiencia profesional

Este repositorio distingue claramente entre:

- **PoC (prueba de concepto)**: validación acotada de una hipótesis, con
  alcance, límites y deuda técnica declarados.
- **Experiencia profesional real**: prácticas, decisiones y operación
  contrastadas en entornos productivos.

Las PoCs de este laboratorio no deben presentarse como experiencia profesional
real. Cada documento indicará su naturaleza, sus límites y lo que no demuestra.

## Estado

Bootstrap del repositorio. La Fase 0 (inventario, evaluación de reutilización,
catálogo de herramientas/licencias/costes, arquitectura, cobertura y backlog)
todavía no se ha ejecutado.

Consulta [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) y
[docs/ROADMAP.md](docs/ROADMAP.md) para más detalle.

## Licencia

El código original de este repositorio se distribuye bajo Apache License 2.0.
Consulta [LICENSE](LICENSE) y [NOTICE](NOTICE). Las licencias de terceros no
quedan sustituidas por esta licencia.
