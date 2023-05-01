# Firestore Standup collection data model

```json
{
  "id": "String",          // Unique identifier for the document
  "type": "String",        // Type of the document, e.g., "task progress" or "user progress"
  "userId": "String",      // User ID (applicable for both task progress and user progress)
  "taskId": "String",      // Task ID (applicable for task only)
  "completed": "String",   // Completed portion of the task (applicable for both similar to yesterday or past progress for user)
  "planned": "String",     // Planned portion of the task (applicable for both similar to today or upcoming plan for user)
  "blockers": "String",    // Blockers (applicable for both task and user progress)
  "date": "Timestamp",     // Date of the standup or user progress (applicable for user progress)
  "createdAt": "Timestamp" // Creation timestamp (applicable for both)
}

```

## Example
User Progress Update
```json
{
  "id": "d4606ee112f7892c45a0",
  "type": "task",
  "userId": "f042d216571a40ece689",
  "taskId": "a52c1d09780ee641f462",
  "completed": "Implemented authentication feature",
  "planned": "Refactor code for better performance",
  "blockers": "Waiting for approval from the team",
  "date": 1651224000,
  "createdAt": 1651228230
}
```
Task progress update
```json
{
  "id": "e71c150bebb80e5e1c15",
  "type": "user",
  "userId": "bb1e01bcee87e555011c",
  "completed": "Reviewed code and provided feedback to teammates",
  "planned": "Attend project meeting and work on UI enhancements",
  "blockers": "Awaiting clarification on design requirements",
  "createdAt": 1651224000
}
```