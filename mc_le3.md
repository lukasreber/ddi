Neo4J

Graph Database

- Open-Source
- NoSQL
- Since 2007
- ACID Compliant
- Cluster support
- Runtime failover

What makes it different

You dont relate Tables and Columsn, you relate data. Therefore it is less structured

Nodes
Relationships
Properties

No ForeignKey

The relationsship is stored in the data, its not an abstract model, like a key
A Relationship can have a property

## Key Argument against SQL
Joins are expensive and confusing

Query Language called Cypher

SQL Example

SELECT name FROM Person
LEFT JOIN Person_Department
ON Person.ID = Person_Department.PersonID
LEFT JOIN Department
ON Department.ID = Person_Department.DepartmentID
WHERE Department.name = "IT Department"

MATCH (p:Person)-[:WORKS_AT]->(d:Dept)
WHERE d.name = "IT Department"
RETURN p.name
