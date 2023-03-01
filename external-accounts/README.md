# External Accounts

## Firestore collection:

```
{
  "type": string,
  "token": string,
  "createdOn": timestamp,
  "attributes" : object
}
```

- Optional fields for `attributes`:
    - `expiry` - timestamp
    - `discordId` - number
    - `username` - string
    - `picture` - string 

### Example
- For Discord Accounts
```
{
  "type": string,
  "token": string,
  "createdOn": timestamp,
  "attributes" : {
    "discordId": number,
    "username": string,
    "picture": string,
    "expiry": timestamp,
  }
}
```
