### OOO Status request Firestore collection model

```json
{
  "id": "String",
  "userId": "String",
  "state": "<PENDING | APPROVED | REJECTED>",
  "from": "Timestamp",
  "until": "Timestamp",
  "message": "String",
  "createdAt": "Timestamp",
  "updatedAt": "Timestamp",
  "lastUpdatedBy": "String",
  "reason": "String"
}
```

#### Fields

| Field         | Type      | Description                                                |
| ------------- | --------- | ---------------------------------------------------------- |
| id            | String    | Unique identifier for the document.                        |
| userId        | String    | The id of the user who created the request.                |
| state         | String    | The state of the request like APPROVED, REJECTED, PENDING. |
| from          | Timestamp | Unix timestamp for the start date of the OOO request.      |
| until         | Timestamp | Unix timestamp for the end date of the OOO request.        |
| message       | String    | The message for the request.                               |
| createdAt     | Timestamp | Unix timestamp for the creation time of the request.       |
| updatedAt     | Timestamp | Unix timestamp for the last update time of the request.    |
| lastUpdatedBy | String    | The id of the superuser who processed the request          |
| reason        | String    | The reason for the APPROVED or REJECTED.                   |

### Example data

#### Example for PENDING state

```json
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
```

#### Example for APPROVED state

```json
{
  "id": "MpykhM8sT1Tlid4Y6Y0d",
  "userId": "dfdsd5T1Tlid4Y6Y0d",
  "state": "APPROVED",
  "from": 1709525300000,
  "until": 1709870800000,
  "message": "Attending a work conference.",
  "createdAt": 1709525400000,
  "updatedAt": 1709827800000,
  "lastUpdatedBy": "Sedv5T1Tlid4Y6Y0d",
  "reason": "Nice to have you back."
}
```

#### Example for REJECTED state

```json
{
  "id": "Me8sT1Tlid4Y6Y0d",
  "userId": "dfdsd5T1Tlid4Y6Y0d",
  "state": "REJECTED",
  "from": 1709603700000,
  "until": 1709785600000,
  "message": "Out of office for personal reasons.",
  "createdAt": 1708763200000,
  "updatedAt": 1708841500000,
  "lastUpdatedBy": "Sedv5T1Tlid4Y6Y0d",
  "reason": "Not enough vacation days."
}
```
