# Firestore collection (trackedProgresses) Data Model

```json
{
  "id": "Unique identifier for the document. (String)",
  "type": "Type of the document, i.e task or user. (String)",
  "userId": "The id of the user, will be applicable only for user. (String)",
  "taskId": "The id of the task, will be applicable only for task. (String)",
  "frequency": "The frequency at which the item is being tracked, expressed as a positive integer. For example, a frequency of 1 represents daily tracking, a frequency of 7 represents weekly tracking, and so on. If not specified, a default value of 1 will be used for tasks. For Users it will always be 1. (Number)",
  "createdAt": "The timestamp indicating the creation time of the trackedProgresses document. (ISO 8601 format)",
  "updatedAt": "The timestamp indicating the last update time of the trackedProgresses document. (ISO 8601 format)"
}
```

## Example

User trackedProgresses Document

```json
{
  "id": "eBe01VS3oYI2HJuWdRuG",
  "type": "user",
  "userId": "abc123",
  "frequency": 1,
  "createdAt": "2023-05-16T14:35:00Z",
  "updatedAt": "2023-05-16T14:35:00Z"
}
```

Task trackedProgresses Document

```json
{
  "id": "en7nlNnpfqoqodcmtMeZ",
  "type": "task",
  "taskId": "abc123",
  "frequency": 4,
  "createdAt": "2023-05-16T14:35:00Z",
  "updatedAt": "2023-05-16T14:35:00Z"
}
```
