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
    "discordId": string,
    "timestamp": timestamp,
    "expiry": timestamp,
  }
}
```
