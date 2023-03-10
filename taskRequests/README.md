# Task Request

Firestore Task Requests collection data model

```
{
  approvedTo?: string,
  id: string,
  isNoteworthy: boolean,
  priority: "LOW" | "Normal" | "HIGH",
  purpose: string,
  requestedBy: string[],
  status: "APPROVED" | "WAITING",
  title: string,
  type: "feature" | "bug",
}
```
