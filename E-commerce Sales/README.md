# 📊 E-commerce Sales | Análisis en Power BI
Análisis de ventas y cartera de clientes de una tienda en línea.

**Negocio:** vi que son muchas transacciones pequeñas y pocos clientes de alto valor; 
con eso sé de qué país y productos vienen, si dejan de comprar y cómo se comportan en el tiempo.

**Datos y modelo:** limpié filas inválidas y validé el dataset antes de analizar.

🏢 Lienzo Directorio
Pulso del negocio: venta, pedidos, ticket promedio, evolución mensual, analisis de inteligencia de tiempo, con la aplicación de segmentadores y haciendo uso de DAX
`SUMX` `DIVIDE` `CALCULATE` `DATEADD` `DATESMTD` `DATESBETWEEN` `SWITCH` `SELECTEDVALUE`

🎯 Lienzo Comercial
Cartera de clientes por valor, recencia, frecuencia y estado (activo o en riesgo). Haciendo uso de funciones DAX
(`IF` `SWITCH` `DATEDIFF` `COUNTROWS` `CALCULATETABLE` `INTERSECT`)

## 🚨 Hallazgo
Cerca del **9%** de la venta de clientes identificados está en clientes relevantes **en fuga**, 
y una quinta parte de eso se concentra en solo tres cuentas.

## ✅ Acción
Campaña de reactivación priorizando a los de mayor valor.
