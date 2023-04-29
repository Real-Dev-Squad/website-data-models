# Firestore Standup collection Streaks model

```json
{
  "userId": "String",
  "currentStreak": "Number",
  "longestStreak": "Number",
  "lastEntryDate": "Timestamp",
  "missedDays": {
    "YYYY-MM": {
      "count": "Number",          // Missed days count for the month
      "days": ["YYYY-MM-DD", ...] // Array of specific days missed
    }
  },
  "attendedDays": {
    "YYYY-MM": {
      "count": "Number",          // Attended days count for the month
      "days": ["YYYY-MM-DD", ...] // Array of specific days attended
    }
  }
}


```

## Example
User Streak
```json
{
  "userId": "f042d216571a40ece689",
  "currentStreak": 7,
  "longestStreak": 10,
  "lastEntryDate": 1651224000,
  "missedDays": {
    "2023-04": {
      "count": 2,
      "days": ["2023-04-02", "2023-04-16"]
    }
  },
  "attendedDays": {
    "2023-04": {
      "count": 25,
      "days": [
        "2023-04-01",
        "2023-04-03",
        "2023-04-04",
        "2023-04-05",
        "2023-04-06",
        "2023-04-07",
        "2023-04-09",
        "2023-04-10",
        "2023-04-11",
        "2023-04-12",
        "2023-04-13",
        "2023-04-14",
        "2023-04-17",
        "2023-04-18",
        "2023-04-19",
        "2023-04-20",
        "2023-04-21",
        "2023-04-23",
        "2023-04-24",
        "2023-04-25",
        "2023-04-26",
        "2023-04-27",
        "2023-04-28",
        "2023-04-30"
      ]
    }
  }
}

```