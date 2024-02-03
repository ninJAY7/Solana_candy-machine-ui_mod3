

# Candy Machine UI Setup Guide

This guide provides step-by-step instructions to set up the user interface (UI) for your Candy Machine, enabling users to mint NFTs using the SPL token you've created. The UI will leverage the SPL token as the payment method, allowing users to mint NFTs by connecting their Phantom wallet.

## Prerequisites

Before initiating the setup, ensure you have the following:

- A Candy Machine configured with details in its `config.json` file.
- A Phantom wallet to act as the minting wallet.

### Candy Machine Configuration Details

Your Candy Machine's `config.json` file should contain the following details:

- `price: 0.01`
- `number: 10`
- `symbol: "NB"`
- `sellerFeeBasisPoints: 500`
- `splTokenAccount: "GfNrcaNWK73ZWJfp4YQ1a2SUvACRPoaoHXEeedDXCWzT"`
- `splToken: "FoBG9XY7s1GyRhxpGkANcbuYorV5sHHnWVXbauiygGYV"`
- `goLiveDate: "2022-07-24T00:00:00Z"`
- `creators: an array with creator details`

## Steps

1. **Set Up the SPL Token**
   - Create the SPL token as per the guidelines provided in Lesson Three and note down its address.

2. **Update Candy Machine Config**
   - Open the `config.json` file and update the following fields:
     - `splTokenAccount` with the created SPL token account address.
     - `splToken` with the SPL token address.

3. **Set Up the UI**
   - Refer to the "Quick Node: Set Up a Minting Site" tutorial to create a user interface for your Candy Machine. This UI enables users to connect their Phantom wallets and mint NFTs using the SPL token as payment.

4. **Modify Minting Logic**
   - Adjust the minting logic of your SPL project to mint NFTs to the Phantom wallet address or modify the transfer function to send the minted NFTs to your Phantom wallet.

5. **Testing**
   - Conduct thorough testing by transferring or minting your SPL token to a Phantom account. Use the created UI to ensure users can successfully mint NFTs by paying in the configured SPL token.

## Additional Tips

- Refer to the complete Candy Machine logic, including minting functionality and token configuration, in the Candy Machine Repository.
- For creating SPL tokens, consult the SPL Token Program by MetaCrafters.
- Ensure all addresses and token details in `config.json` align with the created addresses and tokens.
- Provide clear instructions in your UI for users to connect their Phantom wallets and mint NFTs.
- Customize your UI further based on your design preferences.

## Conclusion

Following these steps will help you establish a Candy Machine UI, allowing users to mint NFTs using the configured SPL token. Users can connect their Phantom wallets and utilize the SPL token as payment to mint NFTs from your Candy Machine. Prioritize thorough testing before deploying for public use.

---
