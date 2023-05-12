---
slug: /reference/sdk.marketplacedirect.acceptoffer
title: MarketplaceDirect.acceptOffer property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# MarketplaceDirect.acceptOffer property

Accept an offer on a direct listing

## Example

```javascript
// The listing ID of the asset you want to bid on
const listingId = 0;
// The price you are willing to bid for a single token of the listing
const offeror = "0x...";

await contract.direct.acceptOffer(listingId, offeror);
```

**Signature:**

```typescript
acceptOffer: {
        (listingId: BigNumberish, addressOfOfferor: string): Promise<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (listingId: BigNumberish, addressOfOfferor: string) => Promise<Transaction<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>>;
    };
```

## Remarks

Accept an offer on a direct listing