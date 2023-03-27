# Events

```
{
  'name': string,
  'description': string,
  'room_id':string,
  'template_id': string,
  'enabled': boolean,
  'lock': boolean,
  'region': <'in' | 'us' | 'eu' | 'auto'>,
  'peers': [
    "peer_id": string,
    "peer_id": string,
    "peer_id": string
   ]
  'createdBy': {
    ref: 'User',
  },
  questions: [
     "question_id": string,
     "question_id": string,
     "question_id": string
  ],
  comments: [
    "comment_id": string,
    "comment_id": string,
    "comment_id": string
  ],
  status: <'active' | 'inactive'>,
  'timestamp': {
    'createdAt': new Date(),
    'updatedAt': new Date(),
  }
}
```
