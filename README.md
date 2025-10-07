# Sprint 6 – Análisis de Retención y Comportamiento del Usuario

## 📄 Descripción
Proyecto desarrollado durante el **Sprint 6 del Bootcamp de Data Analytics (TripleTen)**.  
El objetivo fue analizar **la retención y el comportamiento de los usuarios de una aplicación móvil**, identificando patrones de uso, cohortes con mayor permanencia y variables que afectan la fidelización.

El proyecto combina técnicas de cohort analysis, segmentación temporal y visualización avanzada para apoyar decisiones de producto y marketing.

---

## 🎯 Objetivo
Evaluar la retención de usuarios a lo largo del tiempo, identificar los factores que influyen en su abandono o permanencia, y proponer estrategias para mejorar la lealtad y frecuencia de uso.

---

## 🧩 Contexto del caso
Una app móvil (por ejemplo, de fitness o streaming) busca comprender **cómo varía la retención** según el canal de adquisición, la región y el tipo de dispositivo.  
Los datos abarcan registros de usuarios, eventos de sesión y métricas de interacción diaria durante varios meses.

---

## 🧠 Metodología

1. **Carga y preparación de datos**
   - Archivos: `users.csv`, `events.csv`, `sessions.csv`
   - Conversión de fechas, limpieza de duplicados y construcción de IDs únicos.
   - Cálculo de *user_lifetime_days* y asignación de cohortes por fecha de registro.

2. **Análisis de Retención (Cohort Analysis)**
   - Definición de cohortes mensuales/semanales según `signup_date`.
   - Cálculo del porcentaje de usuarios activos por periodo.
   - Construcción de matriz de retención con visualización de calor (*heatmap*).

3. **Segmentación**
   - Por canal de adquisición, país y tipo de dispositivo.
   - Comparación de curvas de retención entre segmentos.

4. **Visualización**
   - Gráficos de retención acumulada, actividad diaria y evolución del DAU/WAU/MAU.
   - Uso de Matplotlib y Seaborn para visualizaciones comparativas.

---

## 📊 Resultados principales

- La **retención promedio a 30 días** fue del **27.5 %**, con una clara caída entre los días 3 y 7.  
- Los usuarios adquiridos vía **referidos** mostraron la **retención más alta (35 %)**, frente a campañas pagadas (< 20 %).  
- El **canal orgánico móvil (Android)** retuvo mejor que el canal web.  
- Las cohortes de enero y febrero 2025 mantuvieron usuarios activos por más de 8 semanas consecutivas.  
- Se identificaron correlaciones positivas entre número de sesiones y duración de uso diario.

---

## 📈 Conclusiones

El análisis de retención permitió descubrir patrones clave en la permanencia de los usuarios y la efectividad de los canales de adquisición.  
Las cohortes con onboarding más claro y recompensas tempranas mostraron mejor engagement.  
Se recomienda implementar un **sistema de notificaciones personalizadas** y **recompensas por uso recurrente** para fortalecer la lealtad.

---

## 🧰 Herramientas y tecnologías

- **Python:** pandas, numpy, matplotlib, seaborn, datetime  
- **Análisis:** cohort analysis, retención, DAU/WAU/MAU, correlaciones  
- **Visualización:** heatmaps, curvas de retención, histogramas  
- **Control de versiones:** Git · GitHub  
- **Entorno:** Jupyter Notebook / Google Colab

---
