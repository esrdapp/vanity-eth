# Vanity-HPB


Browser-based HPB vanity address generator


## What's a vanity address?

A vanity address is an address which part of it is chosen by yourself, making it look less random. You can use any hexadecimal character/s (abcdef0123456789) to make your wallet address more memorable.

Examples: adding "coffee" `0xc0ffee254729296a45a3885639AC7E10F9d54979`, or adding 999999 `0x999999cf1046e68e36E1aA2E0E07105eDDD1f08E`

## Usage


Enter a short prefix/suffix of your choice at the bottom of the page, and click ‘generate’ to start. Your browser will
generate lots of random addresses until one matches your input.

Once an address is found, you can reveal the private key, or click the 'save' button to download a password-encrypted keystore file.

You can increase the number of working threads to reach higher speeds, or decrease it if you computer struggles.


## Security

As explained above, everything is computed only in your browser. Nothing ever leaves your machine, or even your browser tab.
There is no database, no server-side code. Everything vanishes when you close your tab.

**The website cannot and will never store your private key**, and if you don't trust it, you have 3 ways to ensure your key remains private:

- Once the web page is loaded, you can turn off the internet and continue playing, it will work seamlessly
- You can use it on a completely offline computer
- The code is 100% open source and available on Github. You can review it as much as you want before using it

The keystore file is encrypted with a AES-128-CTR cipher using the BKDF2-SHA256 derivation function with 65536 hashing rounds.


## Performance

Chrome provides the best results.

Using Vanity-HPB on your phone or tablet will work, but don't expect to reach the speed of a good old computer.


## Compatibility

Any address generated with Vanity-HPB is HRC-20 and of course ERC-20 compatible, which means you can use it for an ICO, an airdrop, or just
to withdraw your funds from an exchange.

The keystore file is 100% compatible with MetaMask, geth, etc.


## Build Vanity-HPB from source

The Travis CI bot 🤖 is in charge of building and deploying Vanity-HPB to Github pages, but you can make your own build
from source is you want

```sh
git clone https://github.com/bokub/vanity-eth
cd vanity-eth
npm i
npm run build
```
