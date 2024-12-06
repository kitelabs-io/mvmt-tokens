# Mosaic: The Leading DEX Aggregator on Movement


# Movement Token List:
Mosaic's Movement Token List is the go-to categorized catalog for both legacy coins and Fungible Assets tradeable on the Movement chain. You can JSON file in github to fetch the [Movement Token List](https://raw.githubusercontent.com/kitelabs-io/mvmt-tokens/main/token-list-testnet.json). 

# Projects - How to Add Your Token to the Mosaic Token List:

To add your token to the Movement Token List, follow these steps:

## 1. Add Token Icon

Add the token_symbol.svg file for the token in the [logos_testnet](https://github.com/kitelabs-io/mvmt-tokens/tree/main/logos_testnet) folder. Ensure it's no larger than 250x250 pixels, < 1MB, and has a unique symbol not used by any existing token. 

Provide the following details:


Example:

```typescript
    {
      "faAddress": "0xe161897670a0ee5a0e3c79c3b894a0c46e4ba54c6d2ca32e285ab4b01eb74b66",
      "coinType": "0x275f508689de8756169d1ee02d889c777de1cebda3a7bbcce63ba8a27c563c6f::tokens::USDT",
      "type": "coin",
      "symbol": "USDT",
      "name": "Tether USD",
      "decimals": 6,
      "logoUrl": "https://raw.githubusercontent.com/kitelabs-io/mvmt-tokens/main/logos_testnet/USDT.png"
  }
```


## 2. Commit Changes

Commit your changes with a descriptive message explaining the modifications made.

## 3. Make a Pull Request

Open a pull request to the main branch, and submit it for review. 


`Reminder`: Tokens are always available for trading by pasting the complete token address into our token picker, regardless of their validation status.


# Movement Token List Response

Movement Token List Response object consists of the following fields:

- `faAddress`: The fungible asset address of the token
- `coinType`: The complete address of the token as per the Aptos Coin Standard (Legacy) (optional)
- `type`: 'coin' | 'fungibleAsset'
- `name`: The on-chain registered name of the token
- `symbol`: The on-chain registered symbol of the token
- `decimals`: The number of decimal places of the token
- `logoUrl`: The URL for the token’s logo


Example:

```typescript
    {
      "faAddress": "0xe161897670a0ee5a0e3c79c3b894a0c46e4ba54c6d2ca32e285ab4b01eb74b66",
      "coinType": "0x275f508689de8756169d1ee02d889c777de1cebda3a7bbcce63ba8a27c563c6f::tokens::USDT",
      "type": "coin",
      "symbol": "USDT",
      "name": "Tether USD",
      "decimals": 6,
      "logoUrl": "https://raw.githubusercontent.com/kitelabs-io/mvmt-tokens/main/logos_testnet/USDT.png"
  }
```
