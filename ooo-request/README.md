### OOO Status request Firestore collection model

```json
{
  "id": "String",
  "userId": "String",
  "state": "PENDING",
  "from": "Timestamp",
  "until": "Timestamp",
  "message": "String",
  "createdAt": "Timestamp",
  "updatedAt": "Timestamp",
  // after approval
  "state": "APPROVED",
  "approvedAt": "Timestamp",
  "approvedBy": "String",
  // after rejection
  "state": "REJECTED",
  "rejectedAt": "Timestamp",
  "rejectedBy": "String",
  "rejectedReason": "String"
}
```

#### Fields

| Field          | Type      | Description                                             |
| -------------- | --------- | ------------------------------------------------------- |
| id             | String    | Unique identifier for the document.                     |
| userId         | String    | The id of the user.                                     |
| state          | String    | The state of the request.                               |
| from           | Timestamp | Unix timestamp for the start date of the request.       |
| until          | Timestamp | Unix timestamp for the end date of the request.         |
| message        | String    | The message for the request.                            |
| createdAt      | Timestamp | Unix timestamp for the creation time of the request.    |
| updatedAt      | Timestamp | Unix timestamp for the last update time of the request. |
| approvedAt     | Timestamp | Unix timestamp for the approval time of the request.    |
| approvedBy     | String    | The id of the user who approved the request.            |
| rejectedAt     | Timestamp | Unix timestamp for the rejection time of the request.   |
| rejectedBy     | String    | The id of the user who rejected the request.            |
| rejectedReason | String    | The reason for the rejection of the request.            |

### Example data

```json
// Example for PENDING state
{
  "id": "OfsT1Tlid4Y6Y0d",
  "userId": "dfdsd5T1Tlid4Y6Y0d",
  "state": "PENDING",
  "from": 1709438800000,
  "until": 1709870800000,
  "message": "Out of office for personal reasons.",
  "createdAt": 1709438900000,
  "updatedAt": 1709438900000
}

// Example for APPROVED state
{
  "id": "MpykhM8sT1Tlid4Y6Y0d",
  "userId": "dfdsd5T1Tlid4Y6Y0d",
  "state": "APPROVED",
  "from": 1709525300000,
  "until": 1709870800000,
  "message": "Attending a work conference.",
  "createdAt": 1709525400000,
  "updatedAt": 1709827800000,
  "approvedAt": 1709827800000,
  "approvedBy": "Sedv5T1Tlid4Y6Y0d"
}

// Example for REJECTED state
{
  "id": "Me8sT1Tlid4Y6Y0d",
  "userId": "dfdsd5T1Tlid4Y6Y0d",
  "state": "REJECTED",
  "from": 1709603700000,
  "until": 1709785600000,
  "message": "Out of office for personal reasons.",
  "createdAt": 1708763200000,
  "updatedAt": 1708841500000,
  "rejectedAt": 1708841500000,
  "rejectedBy": "Sedv5T1Tlid4Y6Y0d",
  "rejectedReason": "Not enough notice."
}

```
