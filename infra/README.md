# Infraestructura

Directorio reservado para la definición de infraestructura como código y
artefactos de despliegue (Kubernetes, contenedores, red, almacenamiento,
observabilidad y seguridad).

## Estado

Bootstrap. No contiene infraestructura desplegable. La Fase 0 definirá el
inventario, las herramientas, las licencias, los costes y la arquitectura antes
de crear componentes.

## Reglas

- No incluir secretos, credenciales ni datos personales.
- Documentar licencias y costes de las herramientas utilizadas.
- Priorizar reutilización antes de crear nuevos componentes.
- Mantener cada cambio pequeño, verificable y reversible.
