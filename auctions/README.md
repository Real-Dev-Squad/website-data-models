# Auctions

## Firestore collections:

- auctions
- biddingLog

## Auctions
```
{
  'id': <auction-id>,
  'seller': <userId>,
  'item_type': <example: neelam>,
  'quantity': <number>,
  'highest_bidder': <userId>,
  'highest_bid': <example: 200 dinero | default: initial_price>,
  'start_time': <unix-timestamp>,
  'end_time': <unix-timestamp>,
  'bidders': [<userId>, <userId>]
}
```

## biddingLog
```
{
  'id': <auction-id>,
  'seller': <userId>,
  'item_type': <currency: neelam>,
  'quantity': <number: 10>,
  'initial_price': <example: 100 dinero>,
  'highest_bidder': <userId>,
  'highest_bid': <example: 200 dinero | default: initial_price>,
  'start_time': <unix-timestamp>,
  'end_time': <unix-timestamp>,
  'bidders_and_bids': [
    {
      'bidder': <userId>,
      'bid': <number>,
      'timestamp': <unix-timestamp>
    }
  ],
}
```