# Answers

`status` - (can be PENDING, APPROVED,REJECTED) so that HOST | MODERATOR can filter out the answers which has to be shown in word cloud

`reviewed_by` - id can be of HOST | MODERATOR, the one who reviews the answer

`answered_by` - id of the responder(from peers collection)

```
{
   "id": "<STRING>",
    "answer": "<STRING>",
    "status": "<STRING>",
    "reviewed_by": "<RDS_USER_ID> || null", //can be of HOST | MODERATOR
    "question_id": "<STRING>",
    "answered_by": "<STRING>",
    "event_id": "<STRING>",
    "created_at": "TIMESTAMP",
    "updated_at": "TIMESTAMP"
}
```