## PRESENTACION DEL ANALISIS
Es un dataset de una tienda del sector retail, cuenta con 21 columnas, casi 10K filas, y registros del año 2014 al 2017. Cada registro representa una 
linea de producto dentro de la orden, no la orden completa. 
El campo Sales representa el total de la linea (precio x cantidad) y ya viene incluido el descuento, o sea, es el ingreso real.
El campo Discount es una tasa de descuento (%), no un monto.
El campo Profit es el total de la linea, representa la utilidad, y puede ser negativa.
Los tres campos estas ligados, si el descuento sube entonces Sales baja, afectando tambien al Profit.

El objetivo de calculo es responder a la pregunta: **Dónde crece el negocio de forma rentable, dónde se pierde dinero.**
---En otras hojas se expande el analisis---
## HALLAZGOS
Estacionalidad: existe una estacionalidad marcada en los ingresos, tienen picos en meses como septiembre y noviembre, y caídas en meses como febrero. Por eso las tarjetas comparan cada mes contra el mismo mes del año anterior, no contra el mes previo. 

Sub Categorias con utilidad negativa: En 2017, Tables, Machines, Supplies y Bookcases cerraron con pérdida (cambia según el año del segmentador).

Más unidades vendidas no significan mayor utilidad: En diciembre de 2017 se vendieron 22 % más unidades que en diciembre de 2016, pero la utilidad cayó 53 %.

## ACCIONABLES
Identificar donde se concentran las concentran las perdidas (en que franja de descuento: 1 al 20% o 20 al 40% etc). ---El accionable cambia cuando se complete el análisis de tramo por descuento---
No promocionar sub categorias que presentaron utilidad negativa hasta corregir su precio o descuento.
