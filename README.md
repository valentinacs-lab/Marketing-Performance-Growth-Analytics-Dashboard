# Marketing-Performance-Growth-Analytics-Dashboard
Data-driven analysis of digital channels to optimize sales, engagement and audience growth.

### 1. Marketing Performance & Growth Analytics
**Descripción:**
Análisis del desempeño de canales digitales y comportamiento del usuario para evaluar ventas, engagement y crecimiento de audiencias.

**Objetivos de negocio:**
- Evaluar ventas por canal digital
- Analizar tendencias de crecimiento y engagement
- Identificar patrones de comportamiento del usuario
- Apoyar decisiones de inversión en marketing

**KPIs clave:**
- Ventas totales
- Crecimiento de ventas (%)
- Engagement rate
- Ventas por canal
- Evolución temporal de ventas

**Herramientas:**
Power BI · DAX · Modelado de datos · Visual Analytics

_ _ _ _ _

## Medidas DAX utilizadas
Ventas Totales = SUM ( Marketing[Ventas] )

Interacciones Totales = SUM ( Marketing[Likes] ) + SUM ( Marketing[Comentarios] ) + SUM ( Marketing[Compartidos] )

Engagement % =
DIVIDE ([Interacciones Totales], SUM ( Marketing[Alcance] ))

Ventas Mes Anterior =
CALCULATE ([Ventas Totales], DATEADD ( Dim_Fecha[Date], -1, MONTH ))

Crecimiento Ventas % =
DIVIDE ([Ventas Totales] - [Ventas Mes Anterior],[Ventas Mes Anterior])

