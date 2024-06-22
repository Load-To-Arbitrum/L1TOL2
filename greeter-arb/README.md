# Workshop: Getting to grips with the Arbitrum SDK, 23/04/2024

Hey there, fine people. So you wanna learn how to do L1 --> L2 messaging?

Well, you came to the right place.

Let's get started with:

`git clone https://github.com/sashaaldrick/greeter-arb.git`

`cd greeter-arb`

Make sure to copy the `.env.sample` to `.env` and populate the values as required. You'll need a L1 RPC URL for Sepolia, an L2 RPC URL for Arbitrum Sepolia and a private key for the wallet you'll be using. I recommend using [Alchemy](https://alchemy.com) for the RPC URLs. Make sure this private key is funded on both Ethereum/Arbitrum Sepolia.

Then, depending on your JS runtime, you can run the following:

`npm install` or `yarn install` or `bun install` 🥖

After that, you can go ahead and run `exec.js` with:

`npm run greeter` or `yarn run greeter` or `bun run greeter`


You should get something like below if all went well:

```
$ hardhat run scripts/exec.js
WARNING: You are currently using Node.js v21.6.1, which is not supported by Hardhat. This can lead to unexpected behavior. See https://hardhat.org/nodejs-versions


Environmental variables properly set 👍
                            🔵🔵
                           🔵  🔵
                          🔵    🔵
                         🔵      🔵
                        🔵        🔵
                       🔵          🔵
                      🔵            🔵
                     🔵              🔵
                    🔵                🔵
                   🔵                  🔵
                  🔵                    🔵
                 🔵                      🔵
                🔵🔵🔵🔵🔵🔵🔵🔵🔵🔵🔵🔵🔵🔵
               🔵                          🔵
              🔵                            🔵
             🔵                              🔵
            🔵                                🔵
           🔵                                  🔵
          🔵                                    🔵
         🔵                                      🔵
        🔵                                        🔵
       🔵                                          🔵
      🔵                                            🔵
     🔵                                              🔵
    🔵                                                🔵
Arbitrum Demo: Cross-chain Greeter
Lets
Go ➡️
...🚀

Deploying L1 Greeter 👋
deployed to 0x0c4FCc81Cc2D4FA82dE6A59819b35a0829aF292A
Deploying L2 Greeter 👋👋
deployed to 0x8A0759D6A635632ade77B198e28dbF9ef213389c
Counterpart contract addresses set in both greeters 👍
Current L2 greeting: "Hello world in L2"
Updating greeting from L1 to L2:
Current retryable base submission price is: 2321414320000
L2 gas price: 170220000
Sending greeting to L2 with 36004966780000 callValue for L2 fees:
Greeting txn confirmed on L1! 🙌 0xe17e0d96c37c08462d5531b67c0fe2029bb90bd4e9410dbd58501b2ab16b9c60
Waiting for the L2 execution of the transaction. This may take up to 10-15 minutes ⏰
L2 retryable ticket is executed 🥳 0x552edb44db69d3bdad0e9f13ba0ac9c93adc1e62556c5842a535ac6e7e6e2ac3
Updated L2 greeting: "Greeting from far, far away" 🥳
```
