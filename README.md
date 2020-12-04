# Apuntes y scripts de Bases de Datos - UF2
Repositorio de la asignatura de Bases de Datos (Unidad Formativa 2)

## Diferencias entre OR, AND e IN
Ejemplo:

```sql
SELECT characters.id_character,characters.name
FROM `characters`
WHERE
	characters.id_character IN (1,3)
ORDER BY id_character DESC;


SELECT characters.id_character,characters.name
FROM `characters`
WHERE
	characters.id_character=1 OR characters.id_character=3
ORDER BY id_character DESC;

SELECT characters.id_character,characters.name
FROM `characters`
WHERE
	characters.id_character=1 AND characters.id_character=3
ORDER BY id_character DESC
```