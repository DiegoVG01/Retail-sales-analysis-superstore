## Limpieza de datos - Superstore en EXCEL

- Variable Row ID --> Número
  Se verificó que sea único --> Sin problemas

--Variable Order ID -->  General
  Se verificó consistencia de datos

- Varible Order Date --> Fecha
  Problemas detectado --> Incosistencia del formato. Ejem 11-08-2016 Y 1/16/2016 y se detectó estar en el formato MMDDYYYY con ayuda y analizando   la variable Ship Fecha
  Solución --> Se busco y reemplazó - por / y se estandarizó el formato del dato a DD/MM/YYYY con la herramienta Dato/Texto en columnas

- Variable Ship Date --> Fecha
  Problemas detectado --> Incosistencia del formato. Ejem 12-10-2014 Y 12/13/2016 y se detectó estar en el formato MMDDYYYY con ayuda y   analizando   la variable Order Date
  Solución --> Se busco y reemplazó - por / y se estandarizó el formato del dato a DD/MM/YYYY con la herramienta Dato/Texto en columnas
  Nota: Se detectó que la fecha de despacho puede ser igual a la fecha de orden

- Creación de Varibale Shipping Time derivado de Order Date y Ship Date --> Número
  Se crea esta variable para saber el tiempo de despacho de cada orden

- Variable Ship Mode --> General
  No se detectó anomalías en el texto

- Varible Customer ID --> General
  No se detectó anomalías 

- Varible Segment
  Normal

- Variable Country 
  Validación con una tabla maestra --> Normal

- Variable City
  Validación con una tabla maestra --> Normal

- Varible State
  Validación con una tabla maestra --> Normal

- Varible Region
  Validación con una tabla maestra --> Normal

- Varible Producto ID 
  Normal

- Varibale Category 
  Normal

- Variable Sub-Category
  Normal

- Variable Producto Name
  Normal

- Varibale Sales
  asd

- Varibale Quanty
  asd

- Varibale Discount
  asd

--Varibale Profit
  asd
  


 
