# External Accounts

## Firestore collection:

- external-accounts

```
{
  "type": string,
  "attributes" : object
}
```

### Example
- For Discord Accounts
```
{
  "type": string,
  "attributes" : {
    "token": string,
    "accountId": string,
    "timestamp": timestamp,
    "expiry": timestamp,
  }
}
```
