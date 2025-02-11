# DH-Desafio 2

**Actualización:  23/9**

- *properatti_geo.csv_V2* no tiene la columna de habitaciones_final, con lo cual volví a poner en el repositorio el *properatti_geo.csv*  

En el notebook **Palermos_1**:

- Lee *properatti_geo.csv*
- Filtrado por barrio de Palermo y eliminadas columnas sin uso o redundantes.  
- Cambie nombre de columnas 'habitaciones_final' por 'ambientes' y 'total' por 'superficie' para hacerlo más claro.  
- Agregado de columna *antiguedad* con 3 valores: *'nuevo', 'usado'* y *'pozo'* para corregir el dataset original.  
- Eliminados los registros sin *ambientes*  
- Guardado nuevo dataframe en *palermo_deptos.csv*  

En el notebook **Palermos_map**:

- Cree el shapefile *palermos_map.zip* que tiene los sub-barrios que componen Palermo
- Devuelve el archivo *palermos_map.csv* con las coordenadas de cada sub-barrio

En el notebook **Palermos_2**:

- Lee *palermo_deptos.csv* y *palermos_map.csv*
- Hace ´sjoin´ para ubicar los deptos en los barrios que componen Palermo.
- Devuelve *palermo_deptos_final.csv* con la nueva columna con el barrio
 
En el notebook **Model_AT**:

- Tomo el csv y arme 2 datasets, uno sin distinción de barrios y el otro con los barrios separados  
- La variable categórica *antiguedad* la discretizé en ambos datasets, eliminando la primera columna  
- En el segundo dataset están discretizados *antiguedad* y *barrio*


**Para pensar:** 

- corr(ambientes, superfie) = 0.78  Evaluar si dejamos *ambientes* como variable o nos quedamos solo con *superficie* (~300 datapoints mas)


**Pendientes:**

- Modelos

