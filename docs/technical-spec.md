# ZED20 Token — Technical Specification

ZED20 is a minimal, secure, and auditable BEP-20 token contract deployed on Binance Smart Chain (BSC). Designed for DeFi interoperability and cross-chain utility, it features no admin functions, no minting/burning, and full transparency.

---

## 📄 Contract Details

| Property              | Value                                                                                                                |
|-----------------------|-------------------------------------------|
| **Contract Address**  | [`0x12c860695289e06b390e008ed0871172a24f5008`](https://bscscan.com/token/0x12c860695289e06b390e008ed0871172a24f5008) |
| **Name**              | ZED20 Token                                                                                                          |
| **Symbol**            | ZED20                                                                                                                |
| **Decimals**          | 8                                                                                                                    |
| **Total Supply**      | 200,000,000 ZED20                                                                                                    |
| **Blockchain**        | Binance Smart Chain (BSC)                                                                                            |
| **Standard**          | BEP-20                                                                                                               |
| **Compiler**          | Solidity v0.6.12+commit.27d51765                                                                                     |
| **Optimization**      | Enabled (200 runs)                                                                                                   |
| **License**           | MIT                                                                                                                  |
| **Ownership**         | Not renounced, but no admin functions exist post-deployment                                                          |

---

## ⚙️ Core Functions

The contract implements the standard BEP-20 interface:

- `transfer(address to, uint256 amount)`
- `balanceOf(address account)`
- `approve(address spender, uint256 amount)`
- `allowance(address owner, address spender)`
- `transferFrom(address sender, address recipient, uint256 amount)`
- `increaseAllowance(address spender, uint256 addedValue)`
- `decreaseAllowance(address spender, uint256 subtractedValue)`

> ✅ No additional functions (mint, burn, pause, blacklist) exist.

---

## 🔐 Security Features

- **Immutable**: Contract cannot be upgraded or modified after deployment.
- **No Admin**: No privileged addresses can alter token behavior.
- **No Mint/Burn**: Total supply is fixed at 200,000,000.
- **No Freeze/Pause**: All transfers are always enabled.
- **Gas Optimized**: Efficient transfers and approvals using SafeMath.

---

## 🧪 Verification

- **Verified on BscScan**: [View Contract](https://bscscan.com/token/0x12c860695289e06b390e008ed0871172a24f5008)
- **Source Code**: [Public on GitHub](https://github.com/Maxrighttalent/zed20-official)

---

## 📌 How to Add to Your Wallet

1. Open MetaMask, Trust Wallet, or any BSC-compatible wallet.
2. Go to “Add Token” → “Custom Token”
3. Enter:
   - **Token Contract Address**: `0x12c860695289e06b390e008ed0871172a24f5008`
   - **Token Symbol**: `ZED20`
   - **Decimals**: `8`
4. Click “Add Token”

---

## 🛡️ Disclaimer

This token is **not a stablecoin** and has **no affiliation with Tether Limited, USDT, or any USD-pegged asset**. Use at your own risk.
