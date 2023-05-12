---
slug: /reference/sdk.erc20.setallowance
title: Erc20.setAllowance property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Erc20.setAllowance property

Set token allowance

## Example

```javascript
// Address of the wallet to allow transfers from
const spenderAddress = "0x...";
// The number of tokens to give as allowance
const amount = 100;
await contract.erc20.setAllowance(spenderAddress, amount);
```

**Signature:**

```typescript
setAllowance: {
        (spender: string, amount: string | number): Promise<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (spender: string, amount: string | number) => Promise<Transaction<Omit<{
            receipt: ethers.providers.TransactionReceipt;
            data: () => Promise<unknown>;
        }, "data">>>;
    };
```

## Remarks

Allows the specified `spender` wallet to transfer the given `amount` of tokens to another wallet