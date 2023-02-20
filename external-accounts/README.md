# External Accounts

## Firestore collection:

- external-accounts

```
{
  "type": string,
  "token": string,
  "createdOn": timestamp,
  "attributes" : object
}
```

### Example
- For Discord Accounts
```
{
  "type": string,
  "token": string,
  "createdOn": timestamp,
  "attributes" : {
    "discordId": string,
    "expiry": timestamp,
  }
}
```
