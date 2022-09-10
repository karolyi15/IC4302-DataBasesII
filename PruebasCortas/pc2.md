***Gunther Karolyi Gutierrez 
2017238873
IC4302 - Bases de Datos 2
Grupo 01***

# 1. Explique el concepto de shard, replica y partition.

## Shard

Un shard es una replica que contiene un subconjunto de datos pertenecientes a un cluster.

## Replica

Es una copia exacta de los datos en varios servidores de base de datos.

## Partition

Partitioning consiste en dividir las tablas en un conjunto de sub-tablas más pequeñas con el objetivo de incrementar el performance. A este sub set de datos se le llama partition.

# 2. Explique la diferencia entre Strong Consistency y Eventual Consistency.

El eventual consistency tiene un retraso de un tiempo S para que una base de datos transfiera los datos a una segunda base de datos. Por lo que por este tiempo S, los datos accedidos son inconsistentes. Mientras que el strong consistency requiere que los datos sean consistentes todo el tiempo, por lo que se pone un lock en los nodos mientras que se actualizan y se debe esperar a que todos los nodos sean consistentes.

# 3. ¿En que consiste warm replicas y hot replicas?

## Warm Replicas

Son replicas que no contienen la ultima version de datos, usualmente se actualizan 1 vez a la semana, esto depende del necesidad del cliente. Con normalidad, este tipo de replicas tienen bajos requerimientos de CPU y memoria pero altos requerimeintos de capacidad de disco.

## Hot Replicas

Son replicas que se actulizan en tiempo real. Tienen altos requerimientos de CPU, memoria y disco.

# 4. ¿En que consiste consiste switch over y fail over?

## Switch Over

Consiste en intercambiar la base de datos principal por alguna de las secundarias. Basicamente, se transiciona la base de datos principal a un estado *standby* o secundario y de forma inversa la base de datos secundaria transiciona al papel principal. El switch over garantiza que no hay perdida de datos y usualmente es utilizado en mantenimientos programados.

## Fail Over

Ocurre cuando la base de datos principal falla por alguna razón y alguna de las base de datos secundarias toma el papel de principal. Es utilizado unicamente en caso de catastrofe, donde no sea posible recuperar la base de datos principal en el tiempo requerido.

# Referencias

* MongoDB. (s. f.). MongoDB Sharding. Recuperado 9 de septiembre de 2022, de https://www.mongodb.com/basics/sharding
* Wickramasinghe, S. (s. f.). MongoDB Replication: A Complete Introduction. BMC Blogs. Recuperado 9 de septiembre de 2022, de https://www.bmc.com/blogs/mongodb-replication/
* protostechnologies. (s. f.). Standby Latency & The Difference Between Hot, Warm, and Cold Recovery Sites  |. Recuperado 9 de septiembre de 2022, de https://protostechnologies.com/blog/disaster-recovery/recovery-site-hot-warm-or-cold/
* Oracle. (s. f.). Switchover and Failover Operations. Recuperado 9 de septiembre de 2022, de https://docs.oracle.com/cd/B19306_01/server.102/b14230/sofo.htm
* GeeksforGeeks. (2022, 13 junio). Eventual vs Strong Consistency in Distributed Databases. Recuperado 9 de septiembre de 2022, de https://www.geeksforgeeks.org/eventual-vs-strong-consistency-in-distributed-databases/