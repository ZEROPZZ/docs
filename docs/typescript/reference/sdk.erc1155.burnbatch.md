---
slug: /reference/sdk.erc1155.burnbatch
title: Erc1155.burnBatch property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Erc1155.burnBatch property

Burn a batch of NFTs

## Example

```javascript
// The token IDs to burn NFTs of
const tokenIds = [0, 1];
// The amounts of each NFT you want to burn
const amounts = [2, 2];

const result = await contract.erc1155.burnBatch(tokenIds, amounts);
```

**Signature:**

```typescript
burnBatch: {
        (tokenIds: BigNumberish[], amounts: BigNumberish[]): Promise<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (tokenIds: BigNumberish[], amounts: BigNumberish[]) => Promise<Transaction<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>>;
    };
```

## Remarks

Burn the batch NFTs from the connected wallet