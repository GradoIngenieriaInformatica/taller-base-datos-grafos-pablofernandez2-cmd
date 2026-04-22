MATCH (p:Persona)-[:PARTICIPA_EN]->(pr:Proyecto) 
RETURN pr.nombre, count(DISTINCT p)
