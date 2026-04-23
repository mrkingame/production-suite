# Contrato De Datos ZALINEL Suite

Este documento define el mínimo común para que los módulos conversen entre sí.

## Regla Principal

Cada dato relevante debe mantener:

- `id`
- `timestamp`
- `fecha`
- `origen`
- `tipo`
- `categoria`
- `descripcion`

## Objetivo

Permitir que producción, eventos, bitácora, procedimientos y RCM puedan conectarse sin depender de una base de datos compleja.

## Flujo Inicial

- Operation Suite escribe producción y eventos.
- Bitácora escribe observaciones crudas e incidentes.
- Proceditor escribe procedimientos versionados.
- Dashboard lee producción, eventos y futuras fuentes locales.

## Nota

Esta es la versión inicial del contrato. No debe romper compatibilidad con datos ya generados.
