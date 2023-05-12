---
slug: /reference/sdk.contractplatformfee
title: ContractPlatformFee class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# ContractPlatformFee class

Handle platform fees and recipients

## Example

```javascript
const contract = await sdk.getContract("{{contract_address}}");
const feeInfo = await contract.platformFee.get();
await contract.platformFee.set({
  platform_fee_basis_points: 100, // 1% fee
  platform_fee_recipient: "0x...", // the fee recipient
});
```

## Constructors

| Constructor                                                                  | Modifiers | Description                                                             |
| ---------------------------------------------------------------------------- | --------- | ----------------------------------------------------------------------- |
| [(constructor)(contractWrapper)](./sdk.contractplatformfee._constructor_.md) |           | Constructs a new instance of the <code>ContractPlatformFee</code> class |

## Properties

| Property                                                | Modifiers | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Description                                     |
| ------------------------------------------------------- | --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| [featureName](./sdk.contractplatformfee.featurename.md) |           | "PlatformFee"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |                                                 |
| [set](./sdk.contractplatformfee.set.md)                 |           | { (platformFeeInfo: { platform_fee_basis_points?: number &#124; undefined; platform_fee_recipient?: string &#124; undefined; }): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (platformFeeInfo: { platform_fee_basis_points?: number &#124; undefined; platform_fee_recipient?: string &#124; undefined; }) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; } | Set the platform fee recipient and basis points |

## Methods

| Method                                    | Modifiers | Description                                     |
| ----------------------------------------- | --------- | ----------------------------------------------- |
| [get()](./sdk.contractplatformfee.get.md) |           | Get the platform fee recipient and basis points |

**Signature:**

```typescript
export declare class ContractPlatformFee<TContract extends IPlatformFee> implements DetectableFeature
```

**Implements:** DetectableFeature

## Remarks

Configure platform fees for a contract, which can be applied on certain paid transactions