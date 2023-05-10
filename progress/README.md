# Firestore Standup collection data model

```json
{
  "id": "Unique identifier for the document. (String)",
  "type": "Type of the document, i.e task or user. (String)", 
  "userId": "The id of the user (String)",
  "taskId": "The id of the task ,will be applicable only for task. (String)",
  "completed": "The work accomplished after the previous progress update. (String)",
  "planned": "The planned work to be accomplished before the next update. (String)",
  "blockers": "Issues or obstacles that are preventing progress .(String)",
  "date": "The date for which the progress document pertains to. (Unix Timestamp)",
  "createdAt": "The timestamp indicating the creation time of the progress document. (Unix Timestamp)" 
}

```

## Example
User Progress Document
```json
{
  "id": "d4606ee112f7892c45a0",
  "type": "user",
  "userId": "f042d216571a40ece689",
  "completed": "Implemented authentication feature",
  "planned": "Refactor code for better performance",
  "blockers": "Waiting for approval from the team",
  "date": 1683676800000,
  "createdAt": 1683681079838
}
```

Task progress Document
```json
{
  "id": "e71c150bebb80e5e1c15",
  "type": "task",
  "taskId": "4ERr8WrizICemnQnMF0U",
  "userId": "bb1e01bcee87e555011c",
  "completed": "Reviewed code and provided feedback to teammates",
  "planned": "Attend project meeting and work on UI enhancements",
  "blockers": "Awaiting clarification on design requirements",
  "date": 1683676800000,
  "createdAt": 1683681079838
}
```