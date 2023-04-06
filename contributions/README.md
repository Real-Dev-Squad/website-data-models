# Contributions

```
{
  noteworthy: {
    task: {
      title: string,
      purpose: string<why task is needed>,
      featureUrl: string,
      endsOn: timestamp,
      startedOn: timestamp,
      deployedOn: timestamp,
      status: string,
      dependsOn: [string],
      participants: [{
        firstName: string,
        lastName: string,
        img: string,
        username: string
      }],
      isNoteworthy: boolean,
      isCollapsed: boolean
    },
    prList: [{
      title: string,
      url: string,
      state: string<open|closed>,
      createdAt: timestamp,
      updatedAt: timestamp,
      raisedBy: string<username>
    }]
  },
  all: {
    task: {
      title: string,
      purpose: string<why task is needed>,
      featureUrl: string,
      endsOn: timestamp,
      startedOn: timestamp,
      deployedOn: timestamp,
      status: string,
      dependsOn: [string],
      participants: [{
        firstName: string,
        lastName: string,
        img: string,
        username: string
      }],
      isNoteworthy: boolean,
      isCollapsed: boolean
    },
    prList: [{
      title: string,
      url: string,
      state: string<open|closed>,
      createdAt: timestamp,
      updatedAt: timestamp,
      raisedBy: string<username>
    }]
  }
}

```