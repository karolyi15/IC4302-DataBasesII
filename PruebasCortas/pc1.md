*** Gunther Karolyi Gutierrez 
2017238873
IC4302 - Bases de Datos 2
Grupo 01 ***

# 1. Explique en que consisten los siguientes conceptos:

## * Data Warehouse

Es un repositorio central de información que viene de diversos sources. Son utilizados para analizar información y toma de decisiones.

## * Data Lake 

Es un repositorio centralizado que permite almacenar datos estructurados y no estructurados a cualquier escala.

## * Data Mart

Son bases de dato que almacenan una cantidad limitada de datos estructurados para algun proposito especifico.

# 2. ¿De que forma se benefician las aplicaciones del uso de Columnar Storage? Explique.

Representa un factor importante de optimización, ya que reduce drásticamente los procesos de lectura y escritura en el disco duro. Esto mediante la conversion a columnar storage de cada una de las columnas, esto permite que cada bloque de datos almacene valores para una sola columna para multiples filas en una tabla de bases de datos relacional.

# 3. ¿En que consiste streaming y batch processing?

## * Streaming

Se refiere al procesamiento de un flujo constante de datos proveniente de alguna fuente.

## * Batch Processing

Se refiere al procesamiento de paquetes de datos que provienen de alguna fuente,

# 4. ¿En que consiste datos estructurados, semi estructurados y no estructurados?

## * Datos estructurados

Se refiere a los datos provenientes de bases de datos realacionales que son faciles de procesar y almacenar en tablas.

## * Datos semi estructurados

No tienen un esquema definido, usualmente se organizan mediante etiquetas que permiten agruparlos. Tambien se les conoce como datos No-SQL.

## * Datos no estructurados

Generalmente son datos binarios que no tienen una estructura interna identificable. Se refiere a un grupo masivo y desorganizado de varios objetos.

# Referencias

* What is a Data Warehouse? | Key Concepts | Amazon Web Services. (s. f.). Amazon Web Services, Inc. Recuperado 26 de agosto de 2022, de https://aws.amazon.com/data-warehouse/
* What is a data lake? (s. f.). Amazon Web Services, Inc. Recuperado 26 de agosto de 2022, de https://aws.amazon.com/big-data/datalakes-and-analytics/what-is-a-data-lake/
* Data Warehouse Vs. Data Lake (Vs. Data Mart): A Full Breakdown. (2021, 21 mayo). CLOUDZERO. Recuperado 26 de agosto de 2022, de https://www.cloudzero.com/blog/data-warehouse-vs-data-lake
* Columnar storage - Amazon Redshift. (s. f.). Amazon. Recuperado 26 de agosto de 2022, de https://docs.aws.amazon.com/redshift/latest/dg/c_columnar_storage_disk_mem_mgmnt.html