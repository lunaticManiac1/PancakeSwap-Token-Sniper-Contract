# PancakeSwap-Token-Sniper

## How to use it:
1. Deploy contract using http://remix.ethereum.org/ on Binance Smart Chain
2. Send at least 1 bnb to contract for tokens to buy
3. Call function 'Action' to start sniping

## How it works:
By default contract is looking for 'pair created' event which is when new LP is created to new tokens.
Contract then proceed to buy tokens for 0.002 bnb , approve it to sell and try to sell 1% of tokens in one transaction. If it fails to sell or approve then whole transaction is reverted. That way it avoids honeypots.
Later it waits until price of 20% tokens is worth more then 0.012. When price reach that limit contract sells tokens and send bnb to your wallet.

## Youtube tutorial if you are not sure how to deploy it
https://www.youtube.com/watch?v=YwezjkHEHz8
