# ZALINEL Operation Suite

Herramientas web de registro, control y análisis para la producción de mangas en arena de moldeo.

**Cliente:** Quipasur Ltda · San Bernardo, Chile  
**Máquina:** ZH780L-40 (sand shooting machine)  
**Desarrollado por:** ZALINEL SpA

---

## Herramientas

### ⚙️ Operation Suite `v3.5`
Registro de turno para tablet. Captura:
- Segmentos por tipo de manga (260–460 mm)
- Lotes con KG base, KG resinas y KG mezcla calculado
- Pesos individuales por manga + scrap en grilla
- Panel de eventos con cronómetro en tiempo real (3 categorías: Detiene / En paralelo / Del proceso)
- Historial en localStorage con indicador de uso
- Exporta informes `PROD_fecha_T1_tipo.html` con JSON embebido para el Dashboard

### 📊 Dashboard Producción `v1.1`
Análisis gerencial multi-turno. Carga los informes HTML exportados desde el Operation Suite:
- Resumen ejecutivo con KPIs acumulados
- Producción, Calidad & Pesos, Eficiencia & Merma, Eventos & Paros
- Gráficos de tendencia, distribución y balance de masa
- Filtros por fecha, tipo de manga y turno

---

## Flujo de uso

```
[Tablet en planta]          [PC Gerencia]
Operation Suite   →  HTML  →  Dashboard
  (por turno)    export     (multi-turno)
```

1. El operador registra el turno en el **Operation Suite** (tablet)
2. Al cerrar el turno descarga el informe HTML
3. El informe se arrastra al **Dashboard** para análisis acumulado

---

## URL de acceso

`https://mrkingame.github.io/bitacora-zalinel/`

- Operation Suite: `/operation-suite/`
- Dashboard: `/dashboard/`

---

*ZALINEL SpA · Servicios de Ingeniería de Mantenimiento Industrial*
