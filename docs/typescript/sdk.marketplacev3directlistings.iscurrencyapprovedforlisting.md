---
slug: /sdk.marketplacev3directlistings.iscurrencyapprovedforlisting
title: MarketplaceV3DirectListings.isCurrencyApprovedForListing() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# MarketplaceV3DirectListings.isCurrencyApprovedForListing() method

Check if a currency is approved for a specific direct listing

## Example

```javascript
const listingId = 0;
const currencyContractAddress = "0x1234";
const isApproved = await contract.directListings.isCurrencyApprovedForListing(
  listingId,
  currencyContractAddress,
);
```

**Signature:**

```typescript
isCurrencyApprovedForListing(listingId: BigNumberish, currency: string): Promise<boolean>;
```

## Parameters

| Parameter | Type         | Description      |
| --------- | ------------ | ---------------- |
| listingId | BigNumberish | the listing id   |
| currency  | string       | currency address |

**Returns:**

Promise&lt;boolean&gt;