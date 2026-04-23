## Limpieza de datos - Superstore en EXCEL

- Variable Row ID --> Número  Se verificó que sea único --> Sin problemas

- Variable Order ID -->  General <br>
  Se verificó consistencia de datos

- Varible Order Date --> Fecha <br>
  Problemas detectado --> Incosistencia del formato. Ejem 11-08-2016 Y 1/16/2016 y se detectó estar en el formato MMDDYYYY con ayuda y analizando   la variable Ship Fecha <br>
  Solución --> Se busco y reemplazó - por / y se estandarizó el formato del dato a DD/MM/YYYY con la herramienta Dato/Texto en columnas

- Variable Ship Date --> Fecha <br>
  Problemas detectado --> Incosistencia del formato. Ejem 12-10-2014 Y 12/13/2016 y se detectó estar en el formato MMDDYYYY con ayuda y   analizando   la variable Order Date <br>
  Solución --> Se busco y reemplazó - por / y se estandarizó el formato del dato a DD/MM/YYYY con la herramienta Dato/Texto en columnas
  Nota: Se detectó que la fecha de despacho puede ser igual a la fecha de orden

- Creación de Varibale Shipping Time derivado de Order Date y Ship Date --> Número <br>
  Se crea esta variable para saber el tiempo de despacho de cada orden

- Variable Ship Mode --> General <br>
  No se detectó anomalías en el texto

- Varible Customer ID --> General <br>
  No se detectó anomalías 

- Varible Segment <br>
  Normal

- Variable Country <br>
- Varible Region <br>
- Variable State <br>
- Varible City <br>
  Se validó la jerarquía geográfica (Country → Region → State → City) comparando contra tabla de referencia para detectar asignaciones inconsistentes
- Varible Producto ID <br>
  Se creó una clave compuesta concatenando las columnas "Order ID" y "Product ID", con el objetivo de identificar posibles repeticiones de un mismo producto dentro de una orden. A partir de esta clave, se filtraron los registros repetidos para su análisis.
Dentro de estos casos, se evaluó si las filas correspondían a:
Líneas válidas (mismo producto en una orden pero con diferentes valores de cantidad, ventas o beneficio), o
Duplicados exactos (todas las columnas iguales). <br>

Criterio de eliminación: <br>
Se consideró duplicado exacto cualquier registro en el que todos los campos coinciden.
En dichos casos, se conservó una única fila y se eliminaron las restantes (1 fila #3407).

- Varibale Category --> Texto <br>
  Se revisó consistencia de los datos. No ses encontró errores

- Variable Sub-Category <br>
  Normal
  
- Variable Producto Name <br>
  Normal

- Varibale Sales <br>
  asd por procesar 

- Varibale Quanty <br>
  asd

- Varibale Discount <br>
  asd

- Varibale Profit <br>
  asd
  


 
