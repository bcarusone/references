# Join across intermediate table
In the following example `Patient` is the intermediate table
```python
query = self.session.query(Users
	).join(
		Patient, 
		Patient.user_id == Users.user_id
	).join(
		Policy, 
		Policy.patient_id == Patient.id
	).filter(base_filters)
```