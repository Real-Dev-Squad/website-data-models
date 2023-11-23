# Task Requests

Firestore Collection name: `taskRequests`

#### Task Request Object:
```
{
    taskId: <string>
    externalIssueId: <string>
    requestType: ASSIGNMENT | CREATION
    users: <Array<users>>
    status: PENDING | APPROVED | DENIED
    taskTitle: <string>
    usersCount: <number>
    createdAt: <epoch>
    createdBy: <string>
    lastModifiedAt: <epoch>
    lastModifiedBy: <string>
}
```
#### Users Object:
```
{
	userId: <string>
	status: APPROVED | PENDING 
	proposedDeadline: <epoch>
	proposedStartDate: <epoch>
  	description: <string>
}
```
