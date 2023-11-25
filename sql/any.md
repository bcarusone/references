# Any
Compares a value of the first table with all values of the second table and returns the row if there is a match with any value
```mysql
SELECT *
FROM Teachers
WHERE age = ANY (
	SELECT age
	FROM Students
);
```