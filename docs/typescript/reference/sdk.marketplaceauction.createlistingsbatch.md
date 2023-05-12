---
slug: /reference/sdk.marketplaceauction.createlistingsbatch
title: MarketplaceAuction.createListingsBatch property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# MarketplaceAuction.createListingsBatch property

Create a batch of new auctions

## Example

```javascript
const auctions = [...];
const tx = await contract.auction.createListingsBatch(auctions);
```

**Signature:**

```typescript
createListingsBatch: {
        (listings: NewAuctionListing[]): Promise<TransactionResultWithId<never>[]>;
        prepare: (listings: NewAuctionListing[]) => Promise<Transaction<TransactionResultWithId<never>[]>>;
    };
```

## Remarks

Create a batch of new auctions on the marketplace