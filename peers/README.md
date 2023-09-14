# Peers

```
{
  'id': string,
  'name': string,
  'joined_events': [
    {
      'event_id':"<event_object_id1>",
      'joined_at': <timestamp>,
      'left_at': <timestamp>,
      'role': <'host' | 'moderator' | 'guest' | 'maven'>,
    },
    {
      'event_id':"<event_object_id2>",
      'joined_at': <timestamp>,
      'left_at': <timestamp>,
      'role': <'host' | 'moderator' | 'guest' | 'maven'>,
    },
    ...
    {
      'event_id':"<event_object_idn>",
      'joined_at': <timestamp>,
      'left_at': <timestamp>,
      'role': <'host' | 'moderator' | 'guest' | 'maven'>,
    }
  ],
  'rds_user': {
    is_rds_user:boolean,
    rds_user_id: "<USER_ID_OF_THE_USER_WHO_JOINED_THE_EVENT>"
  },
}
```
