# Use a Subquery
```python
# Write subquery as regular query and call subquery() at the end
subquery = session.query(Claim.id).filter(
	or_(
		Claim.reimbursement.isnot(None),
		and_(
			Claim.created_at.isnot(None),
			Claim.reimbursed_at.isnot(None)
		)
	)
).subquery()

# Use subquery in main query
claims = session.query(Submissions)
	.filter(Submissions.id.in_(subquery))
	.filter(
		Submissions.status == Status.APPROVED,
		Submissions.is_estimate.is_(False)
	).all()
```