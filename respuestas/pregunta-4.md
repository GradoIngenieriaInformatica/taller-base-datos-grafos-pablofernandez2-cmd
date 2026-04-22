MATCH (e:Empresa)<-[:TRABAJA_EN]-(p:Persona)
RETURN e.nombre AS Empresa, count(p) AS NumeroEmpleados
