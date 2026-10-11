## CONOCIENDO PROYECTO_VENTAS:
Este proyecto parte de una base de datos de ventas con 12 tipos de producto en más de 180 países, entre enero de 2010 y julio de 2017. 
Con ella armé en PBI Desktop un reporte de 3 lienzos (básico, intermedio y avanzado), con un menú de navegación basado en botones y acciones de página. 
Trabajé con DAX y modelado de datos.

Antes de calcular cualquier margen, quise auditar el dataset y ver cumplían con criterios de validación.

En el lienzo básico respondí qué región vende más y qué país lidera en carne. Europa encabeza las ventas con $3.48B y también la utilidad absoluta, 
aunque no el margen porcentual. Sudán vende más carne, con 56,503 unidades. Sin embargo, la carne tiene el margen más bajo de su portafolio allí (13.6%), 
así que promocionarla no maximiza ganancias. Lo demostré comparando margen porcentual y utilidad por unidad entre productos, con medidas en SUMX, DIVIDE
y formato condicional para destacar posiciones.

En el lienzo intermedio construí un Pareto de margen por región con medidas de acumulado (RANKX, TOPN, CALCULATE y ALL). Resultado: 
hacen falta 5 de las 7 regiones para cubrir el 80% del margen. 
También calculé el tiempo promedio de envío por país. Para el histograma de bins de 1 día tuve que resolver una limitación: 
una medida no se puede agrupar directamente. La solución fue materializar el promedio por país en una tabla y discretizarlo. Eso reveló un empate entre dos rangos.

En el lienzo avanzado calculé el CAGR de ventas 2010-2016, con variables (VAR) y CALCULATE. 
Lo desglosé por tipo de producto para encontrar categorías en contracción. 
Corregí además un eje truncado que exageraba la variación visual, y separé el KPI de la serie temporal para que cada uno comunicara lo suyo. 
Cerré con el análisis de despachos de las órdenes de diciembre de 2015, donde el lunes concentra la mayor cantidad, con 27 envíos.

## 🕵️ HALLAZGOS:

Entre varios, el más revelador fue el CAGR, siendo 1.25% (positivo con tendencia creciente) en ese periodo revela que existen dos categorias en contradiccion pues 
tienen resultados negativos. 

## 🚀 ACCIONABLES:

Priorizar mover volumen en ese product_type especifco con apoyo de marketing, pues muestra buen margen de utilidad. 

