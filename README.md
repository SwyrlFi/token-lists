# Swyrl Finance Official Token List 🌀

Welcome to Swyrl Finance's canonical token list repository!

This repo tracks every asset that can be listed through Swyrl's concentrated-liquidity DEX and ve(3,3)–governed ecosystem on Monad.


## Contributing to the Token List

Thank you for contributing to the Swyrl Finance token list! Follow these guidelines to submit your token.

### Submission Rules

1. Token must be deployed on Monad Testnet (chainId: 10143)
2. Token icon URL is required
3. Token address must be unique
4. All token information must be accurate

### How to Submit Your Token

**Recommended workflow:**

1. Fork this repository
2. Create a new branch
3. Edit `lists/tokenlists.json` to add your token
4. Submit a pull request

### Token Format

Add your token to the `tokens` array in `lists/tokenlists.json`:

```json
{
  "symbol": "YOUR_SYMBOL",
  "name": "Your Token Name",
  "address": "0x...",
  "logo": "https://your-token-icon-url.png",
  "chainId": 10143,
  "decimals": 18
}
```

### Field Requirements

- **symbol**: Token symbol (required)
- **name**: Full token name (required)
- **address**: Token contract address (required, must be checksummed)
- **logo**: Direct URL to token icon (required)
- **chainId**: Must be 10143 for Monad (required)
- **decimals**: Token decimals (required)

### Logo Guidelines

- Use the same icon URL submitted to [Monad Explorer](https://testnet.monadexplorer.com/listing?type=Token)
- Format: PNG/JPG
- Aspect ratio: 1:1 (square)
- Maximum size: 10MB
- Must be a direct link to the image file

### Example Submission

```json
{
  "symbol": "ANGLER",
  "name": "ANGLER Token",
  "address": "0xfE5bC01Ff7631D495630331E02B4aEAA0BF9840D",
  "logo": "https://swyrl.finance/assets/tokens/angler.png",
  "chainId": 10143,
  "decimals": 18
}
```
