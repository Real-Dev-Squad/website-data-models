### Firestore Collection Model - Request

```json
{
  "typeId": "String",
  "type": "String",
  "state": "<PENDING | APPROVED | REJECTED>",
  "requestedBy": "String",
  "createdAt": "Timestamp",
  "updatedAt": "Timestamp",
  "lastUpdatedBy": "String", // Optional
  "reason": "String", // Optional
  "optionalField": "String" // Optional
}
```

#### Fields

| Field         | Type      | Description                                                                      |
| ------------- | --------- | -------------------------------------------------------------------------------- |
| typeId        | String    | Unique identifier for the document associated with the request.                  |
| type          | String    | A descriptive string representing the type of the request.                       |
| state         | String    | Current state of the request, which can be "PENDING," "APPROVED," or "REJECTED." |
| requestedBy   | String    | Identifier for the user who initiated the request.                               |
| createdAt     | Timestamp | Timestamp indicating when the request was created.                               |
| updatedAt     | Timestamp | Timestamp indicating the last time the request was updated.                      |
| lastUpdatedBy | String    | (Optional) Identifier for the user who last modified the request.                |
| reason        | String    | (Optional) Additional information or justification for the request.              |
| optionalField | String    | (Optional) A field that can be utilized based on specific request types.         |

### Example Data

#### Example 1 - OOO Request (PENDING)

```json
{
  "typeId": "abc123",
  "type": "OOO_REQUEST",
  "state": "PENDING",
  "requestedBy": "user123",
  "createdAt": 1709438900000,
  "updatedAt": 1709438900000
}
```

#### Example 2 - Task Request (APPROVED)

```json
{
  "typeId": "def456",
  "type": "TASK_REQUEST",
  "state": "APPROVED",
  "requestedBy": "user456",
  "createdAt": 1709525400000,
  "updatedAt": 1709827800000,
  "lastUpdatedBy": "admin789",
  "reason": "Task is critical and time-sensitive."
}
```

#### Example 3 - Extension Request (REJECTED)

```json
{
  "typeId": "ghi789",
  "type": "EXTENSION_REQUEST",
  "state": "REJECTED",
  "requestedBy": "user789",
  "createdAt": 1708763200000,
  "updatedAt": 1708841500000,
  "lastUpdatedBy": "admin789",
  "reason": "Cannot extend the deadline due to project constraints."
}
```
