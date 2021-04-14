# Contributions

```
{
  prList: [{
    'title': <title of pull request>,
    'url': <url of pull request>,
    'state': <open or closed>,
    'createdAt': <unix_timestamp>,
    'updatedAt': <unix_timestamp>,
    'raisedBy': <username of the assignee>
  }],
  task: {
    'title': <task tile>,
    'purpose': <why this task is needed>,
    'endsOn': <unix_timestamp>,
    'startedOn': <unix_timestamp>,
    'deployedOn': <unix_timestamp>,
    'status': <status of the task>,
    'participants': [
      {
        'firstName': <first name of user>,
        'lastName': <last name of user>,
        'img': <image url of user>,
        'username': <username of the user>
      },
      {
        'firstName': <first name of user>,
        'lastName': <last name of user>,
        'img': <image url of user>,
        'username': <username of the user>
      }
    ],
    'featureUrl': <url of the feature task>,
    'isNoteworthy': true
  }
}
```