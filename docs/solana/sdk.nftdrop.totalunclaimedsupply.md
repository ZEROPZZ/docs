---
slug: /sdk.nftdrop.totalunclaimedsupply
title: NFTDrop.totalUnclaimedSupply() method
hide_title: true
displayed_sidebar: solana
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## NFTDrop.totalUnclaimedSupply() method

Get the total unclaimed supply of this drop

**Signature:**

```typescript
totalUnclaimedSupply(): Promise<number>;
```

**Returns:**

Promise&lt;number&gt;

the total supply

## Example

```jsx
// Get the total number of lazy minted NFTs that aren't yet claimed
const supply = await program.totalUnclaimedSupply();
```