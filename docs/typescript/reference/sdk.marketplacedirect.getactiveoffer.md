---
slug: /reference/sdk.marketplacedirect.getactiveoffer
title: MarketplaceDirect.getActiveOffer() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# MarketplaceDirect.getActiveOffer() method

Get the active offer on a listing

**Signature:**

```typescript
getActiveOffer(listingId: BigNumberish, address: AddressOrEns): Promise<Offer | undefined>;
```

## Parameters

| Parameter | Type                                  | Description                     |
| --------- | ------------------------------------- | ------------------------------- |
| listingId | BigNumberish                          | the listing id                  |
| address   | [AddressOrEns](./sdk.addressorens.md) | the address that made the offer |

**Returns:**

Promise&lt;[Offer](./sdk.offer.md) \| undefined&gt;