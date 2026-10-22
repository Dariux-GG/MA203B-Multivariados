# Vegetación y calidad del aire en Monterrey (SIMA)

Reto del curso **Aplicación de métodos multivariados en ciencia de datos** · Tec de Monterrey.

Analizamos cómo la vegetación alrededor de las estaciones del SIMA se relaciona con las concentraciones mensuales de **PM10, PM2.5 y NO2** en el Área Metropolitana de Monterrey (2024–2025).

**Equipo:** Lucero Díaz Ortega · Gema Monserrat Ruiz Güereca · Rafael Sánchez Ramírez · Ángel Darío Marroquín Escobedo

## Datos
- **SIMA:** mediciones horarias de contaminantes y meteorología en 15 estaciones (`2003B_Blank/data/`).
- **NDVI mensual y cobertura verde** (Sentinel-2 / Dynamic World) en radios alrededor de cada estación (`Exploracion_descriptiva/datos/`).

## Contenido
| Archivo | Qué hace |
|---|---|
| `Union_de_bases.ipynb` | Limpieza de los datos del SIMA y agregación mensual |
| `Exploracion_descriptiva/Etapa2_exploracion_descriptiva.ipynb` | Exploración descriptiva; genera la base analítica, tablas y figuras |
| `2003B_Blank/quarto/Etapa3_PCA.qmd` | Análisis de componentes principales (R) |
| `Regresion_logistica/Etapa3_regresion_logistica_v3.ipynb` | Regresión logística múltiple (versión vigente) |

## Cómo correrlo
**Python:**
```bash
pip install pandas numpy scipy statsmodels scikit-learn matplotlib seaborn openpyxl jupyter
```
Antes de correr la regresión logística, ajusta `RUTA` en la primera celda para que apunte a `Exploracion_descriptiva/tablas/base_analitica_mensual.csv`.
