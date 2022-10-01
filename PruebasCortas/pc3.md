***Gunther Karolyi Gutierrez 
2017238873
IC4302 - Bases de Datos 2
Grupo 01***

# 1. Explique el concepto de Write Concern en MongoDB. (10 pts)

Write concern describe el nivel de reconocimiento solicitado desde MongoDB para operaciones de escritura en un mongod o bien, en un set de replicas o sharded clusters.

# 2. Explique diferencias entre bases de datos NoSQL y SQL, tome como ejemplo las bases de datos estudiadas en clase y utilizadas en proyectos y tareas: (40 pts)
## a. MongoDB
## b. Elasticsearch
## c. SQL Server
## d. MySQL
## e. PostgreSQL

Una de las principales diferencias es que las bases de datos relacionales (SQL) tales como SQL Server y MySQL utlizan datos estructurados mientras que por el contrario, bases de datos No-SQL como MongoBD y Elasticsearch utilizan esquemas dinamicos para datos no estructurados (JSON). Por otra parte las bases de datos sql son escalables verticalmente, mientras que las no-sql son escalables horizontalmente. Una diferencia adicional es que tal como dice el nombre las bases de datos relacionales se basan en relaciones de tablas, mientras que las las no-sql en pares de llave y valor.

# 3. Desde un punto de vista de una base de datos de series de tiempo, ¿Porqué la localidad de datos es relevante para la escogencia del hardware a utilizar?, puede justificar su respuesta utilizando los data tiers de algún motor de bases de datos como Elasticsearch. (40 pts)

Tal como se menciona los requerimientos de hardware difieren segun el data tier donde se encuentre los datos. Para un data tier hot, donde es necesario acceder a los datos en tiempo real se requiere gran cantidad de memoria, cpu y capacidad de disco. Esto debido a que la disponibilidad y la velocidad deben de ser una prioridad. Mientras que para un data tier cold, por el contrario, son datos que se no es necesario que esten actualizados o bien se acceden cada cierto periodo de tiempo. Por temas de costo y necesidad, se puede utilizar un hardware con menor capacidad tanto en disco, como en memoria y cpu. 

# 4. Explique el concepto de Federated Queries y el impacto que tienen estas en el rendimiento de bases de datos. (10 pts)

Un federed query consiste en enviar una consulta a una base de datos externa (Union de Tablas de diferentes datasets) y obtener el resultado como una tabla temporal. Afecta directamente el rendimiento ya que es probable que las consultas no sean tan rapidas ya que se debe esperar a que la base de datos de origen ejecute la consulta externa y mueva de forma temporal los datos.

# Referencias

* Write Concern — MongoDB Manual. (s. f.). Recuperado 30 de septiembre de 2022, de https://www.mongodb.com/docs/manual/reference/write-concern/
* Consultas federadas  |  BigQuery  |. (s. f.). Google Cloud. Recuperado 30 de septiembre de 2022, de https://cloud.google.com/bigquery/docs/federated-queries-intro?hl=es-419
* GeeksforGeeks. (2022a, junio 6). Difference between SQL and NoSQL. Recuperado 30 de septiembre de 2022, de https://www.geeksforgeeks.org/difference-between-sql-and-nosql/