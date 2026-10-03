# DSS para la Mejora de la Productividad de Mano de Obra

## Descripción

Este proyecto desarrolla un Sistema de Soporte a Decisiones (DSS) orientado a apoyar el análisis y la mejora de la productividad de mano de obra en una empresa del sector metalmecánico.

La solución permite procesar información operativa del proceso de fabricación, visualizar indicadores de productividad, identificar pérdidas asociadas a actividades que no agregan valor y apoyar la priorización de acciones de mejora.

El DSS integra tres herramientas principales de Ingeniería Industrial:

- 5S: orientada a reducir desorden y tiempos de búsqueda.
- SLP (Systematic Layout Planning): orientada a reducir recorridos innecesarios y mejorar el flujo.
- TPM (Total Productive Maintenance): orientada a reducir paradas y fallas de los equipos.

---

## Objetivo del DSS

Apoyar la toma de decisiones para mejorar la productividad de mano de obra mediante el análisis de información relacionada con:

- Producción.
- Horas-hombre.
- Horas extra.
- Tiempos de búsqueda.
- Recorridos.
- Paradas de equipos.
- Número de fallas.
- Cumplimiento del Checklist 5S.

---

## Funcionamiento

El flujo general del sistema es:

Datos de entrada  
↓  
Validación de información  
↓  
Cálculo de indicadores  
↓  
Diagnóstico de pérdidas  
↓  
Priorización de oportunidades de mejora  
↓  
Recomendación 5S / SLP / TPM  
↓  
Simulación de escenario propuesto  
↓  
Visualización de resultados

---

## Datos de entrada

El sistema permite cargar archivos Excel (.xlsx) o CSV (.csv).

La base debe contener las siguientes variables:

| Variable | Descripción |
|---|---|
| periodo | Periodo de análisis |
| tipo_tanque | Tipo de tanque fabricado |
| horas_hombre | Horas-hombre utilizadas |
| unidades_producidas | Unidades terminadas |
| horas_extra | Horas extra trabajadas |
| tiempo_busqueda_min | Tiempo destinado a búsqueda de materiales o herramientas |
| recorrido_m | Distancia recorrida durante el proceso |
| paradas_h | Horas de parada de equipos |
| numero_fallas | Número de fallas registradas |
| checklist_5s_pct | Porcentaje de cumplimiento del Checklist 5S |

---

## Indicadores

El dashboard permite visualizar:

- Productividad de mano de obra.
- Horas extra.
- Tiempo de búsqueda.
- Recorridos.
- Horas de parada.
- Número de fallas.
- Cumplimiento del Checklist 5S.

La productividad de mano de obra se calcula mediante:

Productividad = Unidades producidas / Horas-hombre

---

## Dashboard

La interfaz fue desarrollada en Streamlit y presenta gráficos para analizar:

1. Evolución de la productividad.
2. Horas extra por periodo.
3. Recorridos realizados.
4. Tiempo de búsqueda.
5. Horas de parada de equipos.
6. Número de fallas.
7. Cumplimiento del Checklist 5S.
8. Diagnóstico del DSS.
9. Comparación del escenario actual y propuesto.

---

## Simulación de escenarios

El DSS permite modificar parámetros para evaluar posibles escenarios de mejora:

- Reducción del tiempo de búsqueda.
- Reducción de recorridos.
- Reducción de paradas.
- Mejora del cumplimiento 5S.

El sistema recalcula los indicadores y compara:

**Situación actual vs. escenario propuesto**

Los resultados del escenario propuesto corresponden a una simulación para apoyar la toma de decisiones y no representan resultados reales hasta que las mejoras sean implementadas y medidas.

---

## Herramientas utilizadas

- Python
- Streamlit
- Pandas
- NumPy
- OpenPyXL
- Excel / CSV
- GitHub Codespaces

---

## Ejecutar la aplicación

Instalar las dependencias:

```bash
pip install streamlit pandas numpy openpyxl
