# ZALINEL Production Suite

Suite de herramientas web para trazabilidad operativa, control de proceso y análisis de producción en fabricación de mangas de fundición por disparo de arena.

## Propósito

Este repositorio reúne las herramientas de trabajo usadas en computador para registrar el proceso productivo y analizar sus resultados de forma estructurada.

La suite está pensada para acompañar la operación real de planta y transformar la información del turno en datos útiles para control, seguimiento y toma de decisiones.

## Componentes

### Operation Suite
Herramienta principal de captura estructurada del proceso productivo.

Uso principal:
- Registro de turno
- Captura de lotes
- Registro de producción por manga
- Control de scrap
- Registro de eventos con tiempo
- Control de merma
- Registro de pallets
- Generación de informe HTML del turno

Ubicación:
`/apps/operation-suite/`

### Dashboard
Herramienta de análisis y visualización de resultados.

Uso principal:
- Lectura de informes exportados desde Operation Suite
- Consolidación de registros
- Visualización de KPIs
- Balance de masa
- Análisis de scrap, merma y eficiencia
- Revisión de tendencias y oportunidades de mejora

Ubicación:
`/apps/dashboard/`

## Flujo de trabajo

1. El turno se registra en `Operation Suite`.
2. Se genera un informe HTML del turno.
3. El informe se carga en `Dashboard`.
4. Se analizan resultados, tendencias y oportunidades de mejora.

## Estructura del repositorio

```text
apps/
  operation-suite/
    index.html
  dashboard/
    index.html
docs/
  historial-de-cambios.md
index.html
README.md
