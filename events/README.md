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
    "<peer_id>",
    "<peer_id>",
    "<peer_id>"
   ]
  'created_by': {
    ref: 'User',
  },
  'questions': [
    "<question_id>",
    "<question_id>",
    "<question_id>"
  ],
  'comments: [
    "<comment_id>",
    "<comment_id>",
    "<comment_id>",
  ],
  'status': <'active' | 'inactive'>,
  'timestamp': {
    'created_at': timestamp,
    'updated_at': timestamp,
  }
}
```
