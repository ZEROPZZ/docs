---
slug: /reference/sdk.marketplacev3offers.acceptoffer
title: MarketplaceV3Offers.acceptOffer property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# MarketplaceV3Offers.acceptOffer property

Accept an offer

## Example

```javascript
// The ID of the offer you want to accept
const offerId = 0;

await contract.offers.acceptOffer(offerId);
```

**Signature:**

```typescript
acceptOffer: {
        (offerId: BigNumberish): Promise<Omit<{
            receipt: import("@ethersproject/abstract-provider").TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (offerId: BigNumberish) => Promise<Transaction<Omit<{
            receipt: import("@ethersproject/abstract-provider").TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>>;
    };
```