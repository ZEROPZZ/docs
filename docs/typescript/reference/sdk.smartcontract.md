---
slug: /reference/sdk.smartcontract
title: SmartContract class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# SmartContract class

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.

Custom contract dynamic class with feature detection

## Example

```javascript
import { ThirdwebSDK } from "@thirdweb-dev/sdk";

const sdk = new ThirdwebSDK(provider);
const contract = await sdk.getContract("{{contract_address}}");

// call any function in your contract
await contract.call("myCustomFunction", param1, param2);

// if your contract follows the ERC721 standard, contract.nft will be present
const allNFTs = await contract.erc721.query.all();

// if your contract extends IMintableERC721, contract.nft.mint() will be available
const tx = await contract.erc721.mint({
  name: "Cool NFT",
  image: readFileSync("some_image.png"),
});
```

## Constructors

| Constructor                                                                                                              | Modifiers | Description                                                                    |
| ------------------------------------------------------------------------------------------------------------------------ | --------- | ------------------------------------------------------------------------------ |
| [(constructor)(network, address, abi, storage, options, chainId, contractWrapper)](./sdk.smartcontract._constructor_.md) |           | **_(BETA)_** Constructs a new instance of the <code>SmartContract</code> class |

## Properties

| Property                                                      | Modifiers             | Type                                                                                              | Description                                           |
| ------------------------------------------------------------- | --------------------- | ------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| [abi](./sdk.smartcontract.abi.md)                             |                       | [Abi](./sdk.abi.md)                                                                               | **_(BETA)_**                                          |
| [app](./sdk.smartcontract.app.md)                             | <code>readonly</code> | [ContractAppURI](./sdk.contractappuri.md)&lt;IAppURI &#124; IContractMetadata&gt;                 | **_(BETA)_** Auto-detects AppURI standard functions.  |
| [chainId](./sdk.smartcontract.chainid.md)                     | <code>readonly</code> | number                                                                                            | **_(BETA)_**                                          |
| [directListings](./sdk.smartcontract.directlistings.md)       | <code>readonly</code> | [MarketplaceV3DirectListings](./sdk.marketplacev3directlistings.md)&lt;DirectListingsLogic&gt;    | **_(BETA)_** Direct listings                          |
| [encoder](./sdk.smartcontract.encoder.md)                     |                       | [ContractEncoder](./sdk.contractencoder.md)&lt;TContract&gt;                                      | **_(BETA)_**                                          |
| [englishAuctions](./sdk.smartcontract.englishauctions.md)     | <code>readonly</code> | [MarketplaceV3EnglishAuctions](./sdk.marketplacev3englishauctions.md)&lt;EnglishAuctionsLogic&gt; | **_(BETA)_** Auctions                                 |
| [erc1155](./sdk.smartcontract.erc1155.md)                     | <code>readonly</code> | [Erc1155](./sdk.erc1155.md)                                                                       | **_(BETA)_** Auto-detects ERC1155 standard functions. |
| [erc20](./sdk.smartcontract.erc20.md)                         | <code>readonly</code> | [Erc20](./sdk.erc20.md)                                                                           | **_(BETA)_** Auto-detects ERC20 standard functions.   |
| [erc721](./sdk.smartcontract.erc721.md)                       | <code>readonly</code> | [Erc721](./sdk.erc721.md)                                                                         | **_(BETA)_** Auto-detects ERC721 standard functions.  |
| [estimator](./sdk.smartcontract.estimator.md)                 |                       | [GasCostEstimator](./sdk.gascostestimator.md)&lt;TContract&gt;                                    | **_(BETA)_**                                          |
| [events](./sdk.smartcontract.events.md)                       |                       | [ContractEvents](./sdk.contractevents.md)&lt;TContract&gt;                                        | **_(BETA)_**                                          |
| [interceptor](./sdk.smartcontract.interceptor.md)             |                       | [ContractInterceptor](./sdk.contractinterceptor.md)&lt;TContract&gt;                              | **_(BETA)_**                                          |
| [metadata](./sdk.smartcontract.metadata.md)                   |                       | [ContractMetadata](./sdk.contractmetadata.md)&lt;BaseContract, any&gt;                            | **_(BETA)_**                                          |
| [offers](./sdk.smartcontract.offers.md)                       | <code>readonly</code> | [MarketplaceV3Offers](./sdk.marketplacev3offers.md)&lt;OffersLogic&gt;                            | **_(BETA)_** Offers                                   |
| [owner](./sdk.smartcontract.owner.md)                         | <code>readonly</code> | [ContractOwner](./sdk.contractowner.md)&lt;Ownable&gt;                                            | **_(BETA)_** Set and get the owner of the contract    |
| [platformFees](./sdk.smartcontract.platformfees.md)           | <code>readonly</code> | [ContractPlatformFee](./sdk.contractplatformfee.md)&lt;IPlatformFee&gt;                           | **_(BETA)_** Handle platform fees                     |
| [publishedMetadata](./sdk.smartcontract.publishedmetadata.md) |                       | ContractPublishedMetadata&lt;TContract&gt;                                                        | **_(BETA)_**                                          |
| [roles](./sdk.smartcontract.roles.md)                         | <code>readonly</code> | [ContractRoles](./sdk.contractroles.md)&lt;IPermissions, any&gt;                                  | **_(BETA)_** Handle permissions                       |
| [royalties](./sdk.smartcontract.royalties.md)                 | <code>readonly</code> | [ContractRoyalty](./sdk.contractroyalty.md)&lt;IRoyalty, any&gt;                                  | **_(BETA)_** Handle royalties                         |
| [sales](./sdk.smartcontract.sales.md)                         | <code>readonly</code> | [ContractPrimarySale](./sdk.contractprimarysale.md)&lt;IPrimarySale&gt;                           | **_(BETA)_** Handle primary sales                     |

## Methods

| Method                                                               | Modifiers | Description                                     |
| -------------------------------------------------------------------- | --------- | ----------------------------------------------- |
| [call(functionName, args, overrides)](./sdk.smartcontract.call.md)   |           | **_(BETA)_** Call any function on this contract |
| [getAddress()](./sdk.smartcontract.getaddress.md)                    |           | **_(BETA)_**                                    |
| [onNetworkUpdated(network)](./sdk.smartcontract.onnetworkupdated.md) |           | **_(BETA)_**                                    |
| [prepare(method, args, overrides)](./sdk.smartcontract.prepare.md)   |           | **_(BETA)_** Prepare a transaction for sending  |

**Signature:**

```typescript
export declare class SmartContract<TContract extends BaseContractInterface = BaseContract> implements UpdateableNetwork
```

**Implements:** UpdateableNetwork