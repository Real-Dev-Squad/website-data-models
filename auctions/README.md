# Auctions

## Firestore collections:

- auctions
- bids

## Auctions
```
{
  'end_time': <unix-timestamp>,
  'highest_bid': <example: 200 dinero | default: initial_price>,
  'highest_bidder': <userId>,
  'item': <example: neelam>,
  'quantity': <number>,
  'seller': <userId>,
  'start_time': <unix-timestamp>
}
```

## Bids
```
{
  'auction_id': <auction-id>,
  'bid': <number: 10>,
  'bidder': <userId>,
  'timestamp': <unix-timestamp>
}
```