# Análisis de Ventas Retail - Q4 2024 📊

Este proyecto consiste en un análisis detallado del desempeño de ventas de una cadena minorista durante el último trimestre (Q4) de 2024. Incluye el proceso completo de limpieza de datos, extracción de métricas clave y visualización de resultados.

## 📋 Estructura del Proyecto

El archivo Excel está organizado en las siguientes etapas:

1.  **ventas_q4_2024_raw**: Datos originales con inconsistencias de formato y valores faltantes.
2.  **Ventas_Datos_Ajustados**: Datos limpios y normalizados, con nuevas columnas calculadas para el análisis.
3.  **Métricas**: Cálculos consolidados sobre el rendimiento del trimestre.
4.  **Resumen_Ejecutivo**: Hallazgos principales, metodología y recomendaciones.
5.  **Gráficos**: Tablas dinámicas y visualizaciones de ventas por ciudad y mes.

## 🛠️ Proceso de Limpieza y Transformación (ETL)

Para facilitar el análisis, se realizaron las siguientes acciones en la hoja de **Datos Ajustados**:
* **Corrección de Fechas:** Estandarización de formatos (DD/MM/AAAA).
* **Normalización de Texto:** Limpieza de nombres de clientes con caracteres especiales y corrección de nombres de ciudades (ej: "Ciudad de M√xico" a "Ciudad de México").
* **Segmentación de Producto:** Se dividió la columna `Producto` en tres nuevas categorías: `Categoría`, `Desc.1` (Tipo) y `Desc.2` (Capacidad).
* **Tratamiento de Nulos:** Identificación de 12 registros sin *Precio Unitario* y 19 sin *Monto Total*.

## 📈 Hallazgos Principales

### Métricas Clave
* **Ventas Totales (Trimestre):** $3,887,554.77
* **Venta Promedio por Transacción:** $3,891.45
* **Número de Transacciones:** 999
* **Mes con mejor resultado:** Diciembre ($1,318,530.73)

### Rendimiento por Ciudad
La **Ciudad de México** lidera el volumen de ventas, seguida de cerca por Cali y Monterrey.

| Ciudad | Ventas Totales (Q4) |
| :--- | :--- |
| Ciudad de México | $682,952.88 |
| Cali | $670,990.08 |
| Monterrey | $647,212.81 |
| Guadalajara | $632,208.30 |
| Bogotá | $607,996.82 |
| Medellín | $589,769.95 |

### Top 5 Productos más vendidos (Cantidad)
1. Tablet-Mini-4GB
2. Auriculares-Con cable-16GB
3. Tablet-Estándar-4GB
4. Teléfono-Gama alta-8GB
5. Teléfono-Gama alta-4GB

## 💡 Recomendaciones
Basado en el análisis, se sugiere:
* **Estandarización de Captura:** Implementar validación de datos en el origen para evitar inconsistencias en nombres de ciudades y formatos de fecha.
* **Gestión de Inventario:** Reforzar el stock de la línea "Tablet-Mini" y "Auriculares", que muestran el mayor volumen de rotación.
* **Soporte de Precios:** Investigar la causa de los precios unitarios faltantes para asegurar la integridad de los reportes financieros.

## 🖥️ Tecnologías Utilizadas
* **Microsoft Excel:** Limpieza de datos (Power Query / Fórmulas), Tablas Dinámicas y Gráficos.
* **Markdown:** Para la documentación del repositorio.

---
**Autor:** [Juan Pablo Vargas]  
**Fecha:** Octubre 2025
