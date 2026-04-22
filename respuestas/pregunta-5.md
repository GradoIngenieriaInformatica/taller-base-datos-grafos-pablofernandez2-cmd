MATCH (a:Persona)-[:AMIGO_DE]-(b:Persona)-[:AMIGO_DE]-(c:Persona)
WHERE a <> c 
  AND NOT (a)-[:AMIGO_DE]-(c)
RETURN DISTINCT b.nombre AS PersonaPuente
