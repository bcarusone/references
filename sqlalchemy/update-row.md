# Update row
```python
def update_row(new_name):
	session = Session()
	
	new_row = Row(
		id=old_row.id,
		name=new_name 
	)
	
	session.merge(new_row)
	session.commit()
```