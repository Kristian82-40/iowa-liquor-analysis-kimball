# Iowa Liquor Sales Analysis - Kimball Data Warehouse

**Proyecto:** Análisis de ventas de licor en Iowa usando metodología Kimball  
**Analista:** Data Analyst Junior  
**Fecha:** 27/12/2025  
**Herramientas:** Google BigQuery, SQL, Metodología Kimball

---

## 📊 Resumen Ejecutivo

Este proyecto demuestra el análisis de datos de ventas de licor en Iowa siguiendo la **metodología Kimball de data warehouse**, integrando análisis de negocio con diseño dimensional profesional.

**Objetivo:** Responder 4 preguntas clave de negocio y diseñar una fact table Kimball para análisis futuro.

---

## 🎯 Preguntas de Negocio Respondidas

### **Q1: ¿Cuál es el ingreso total por categoría de licor?**
- **Consulta:** `Iowa_Liquor_Q1_Ingresos_por_Categoria`
- **Métrica clave:** SUM(sale_dollars) agrupado por category
- **Resultado:** TOP 5 categorías por ingresos identificadas
- **Utilidad para negocio:** Priorizar inventario y marketing

### **Q2: ¿Cuál es la tendencia de ventas por mes?**
- **Consulta:** `Iowa_Liquor_Q2_Tendencia_por_Mes`
- **Métrica clave:** SUM(sale_dollars) agrupado por mes-año
- **Resultado:** Patrón de crecimiento/caída de ventas
- **Utilidad para negocio:** Planeación estacional y presupuesto

### **Q3: ¿Hay ciudades que se comportan diferente a otras?**
- **Consulta:** `Iowa_Liquor_Q3_Ventas_por_Ciudad`
- **Métrica clave:** SUM(sale_dollars) agrupado por city
- **Resultado:** TOP 10 ciudades (DES MOINES lidera)
- **Utilidad para negocio:** Estrategia regional

### **Q4: ¿Cuál es el ticket promedio y su distribución?**
- **Consulta:** `Iowa_Liquor_Q4_Ticket_Promedio`
- **Métrica clave:** AVG, MIN, MAX, COUNT de sale_dollars
- **Resultado:** Ticket promedio ~$148
- **Utilidad para negocio:** Análisis de rentabilidad

---

## 📐 Diseño Kimball

**Fact Table:** Centraliza métricas (sale_dollars, quantity)  
**Dimensiones:** fecha, ciudad, categoría  
**Limpieza:** COALESCE y CAST para NULLs y tipos

---

## 💾 Estructura de Datos

- Dataset: `bigquery-public-data.iowa_liquor_sales.sales`
- Registros: 33M+ transacciones
- Período: 2012-2024

---

## 🚀 Metodología Kimball

1. Identificar hechos (métricas numéricas)
2. Identificar dimensiones (atributos descriptivos)
3. Limpiar datos (COALESCE, CAST)
4. Documentar profesionalmente
5. Diseño dimensional

---

## 🔧 Roadmap

- ✅ Q1-Q4 completadas
- ✅ Fact table diseñada
- ⏳ Crear dimensiones
- ⏳ dbt para automatizar
- ⏳ Airflow para pipelines
- ⏳ Dashboards Looker

---

## 📞 Contacto

**Analista:** Data Analyst Junior  
**Email:** contacto@email.com  
**GitHub:** github.com/tu-usuario

---

## 📄 Práctica educativa para Kimball
