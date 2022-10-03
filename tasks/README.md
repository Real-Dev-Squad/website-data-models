# Tasks
Firestore Tasks collection data model

```
{
  taskId: <id>,
  title: string,
  purpose: string,
  featureUrl: string,
  type: string,
  links: [string],
  endsOn: string,
  startedOn: string,
  status: string,
  dependsOn: [string],
  completionAward: {
    neelam: number,
    dinero: number
  },
  lossRate: {
    neelam: number,
    dinero: number
  },
  isNoteworthy: boolean,
  createdBy: string,
  assignee: string,
  participants: [userId, userId]
  percentCompleted : number
}
   
```
