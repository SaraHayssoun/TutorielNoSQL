## Bases de Données Orientées Graphes


### Structure:

La base de données orientée graphes est structurés sous forme noeuds-arcs.
chaque noeud représente une donnée ayant une étiquette ainsi que les arcs représentent les relations entre les données (noeuds).

![structure(Ref: https://docs.microsoft.com/en-us/sql/relational-databases/graphs/sql-graph-sample?view=sql-server-2017)](images/relation-graph-example.png)

### Langage:

Les bases de données orientées graphes ont différentes manières pour manipuler les données. Plusieurs BD, comme Neo4j,
supporte : 
* Le langage de requête RDF SPARQL 
* Le langage impératif (Lamgage des requêtes basées sur le chemin) Gemlin 
* Le langage déclaratif Cypher.

### Exemple de requêtes utilisant CYPHER

	(emil:Person {name:'Emil'})<-[:KNOWS]-(jim:Person {name:'Jim'})
 	-[:KNOWS]->(ian:Person {name:'Ian'})
 	-[:KNOWS]->(emil)
