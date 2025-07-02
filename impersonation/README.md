### Impersonation Request Firestore collection model

```json
{
  "id": "string",
  "createdBy": "string",
  "createdFor": "string",
  "status": "<PENDING | APPROVED | REJECTED>",
  "isImpersonationFinished": "boolean",
  "startedAt": "Timestamp",
  "endedAt": "Timestamp",
  "reason": "string",
  "message": "string",
  "createdAt": "Timestamp",
  "updatedAt": "Timestamp",
  "lastModifiedBy": "string"
}
```

#### Fields

| Field         | Type      | Description                                                        |
| ------------- | --------- | -------------------------------------------------------------------|
| id            | String    | Unique identifier for the document.                                |
| createdBy     | String    | The id of the super-user who created the impersonation request.    |
| createdFor    | String    | The id of the user for the the impersonation request is created.   |
|isImpersonationFinished | Boolean    | The boolean value which determines if a request has already been impersonated              |
| status        | String    | The status of the request like APPROVED, REJECTED, PENDING.        |
| startedAt     | Timestamp | Firebase timestamp for the start time of the impersonation session.|
| endedAt       | Timestamp | Firebase timestamp for the end time of the impersonation session.  |
| message       | String    | The message sent when updating the status of the request.          |
| createdAt     | Timestamp | Firebase timestamp for the creation time of the request.           |
| updatedAt     | Timestamp | Firebase timestamp for the last update time of the request.        |
| lastModifiedBy| String    | The id of the user who last modified the request                   |
| reason        | String    | The reason for the creation of impersonation request.              |

### Example data

#### Example for PENDING state

```json
{
  "id": "qweT1Tlid4Y6Y0d",
  "createdBy": "superUser123",
  "createdFor": "user456",
  "status": "PENDING",
  "reason": "Need to debug an issue in production.",
  "isImpersonationFinished": false,
  "createdAt": 1721233200000,
  "updatedAt": 1721233200000
}
```

#### Example for REJECTED state

```json
{
  "id": "impReq456",
  "createdBy": "superUser123",
  "createdFor": "user789",
  "status": "REJECTED",
  "reason": "Unnecessary access request.",
  "message": "User does not need impersonation.",
  "isImpersonationFinished": false,
  "createdAt": 1722470000000,
  "updatedAt": 1722473600000,
  "lastModifiedBy": "adminReviewer456"
}
```

#### Example for APPROVED state

```json
{
  "id": "impReq456",
  "createdBy": "superUser123",
  "createdFor": "user789",
  "status": "APPROVED",
  "reason": "Debugging an issue reported by the user.",
  "message": "Approved for limited session access.",
  "isImpersonationFinished": false,
  "createdAt": 1722470000000,
  "updatedAt": 1722473600000,
  "lastModifiedBy": "adminReviewer456"
}
```


#### Example for APPROVED state (Session Started)

```json
{
  "id": "abcT1Tlid4Y6Y0d",
  "createdBy": "superUser123",
  "createdFor": "user456",
  "status": "APPROVED",
  "reason": "Debugging user's data issue.",
  "message": "Request approved for investigation.",
  "startedAt": 1721240000000,
  "createdAt": 1721233200000,
  "updatedAt": 1721240000000,
  "lastModifiedBy": "superUser123",
  "isImpersonationFinished": false
}

```

#### Example for Finished state (Session Stopped/Completed)

```json
{
  "id": "defT1Tlid4Y6Y0d",
  "createdBy": "superUser123",
  "createdFor": "user456",
  "status": "APPROVED",
  "reason": "Debugging login issue.",
  "message": "Session completed successfully.",
  "startedAt": 1721240000000,
  "endedAt": 1721240900000,
  "createdAt": 1721233200000,
  "updatedAt": 1721240900000,
  "lastModifiedBy": "superUser123",
  "isImpersonationFinished": true
}
```
