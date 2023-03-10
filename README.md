# Dex Arbitrage Using Flash-Loan

In this tutorial we will create an artificial arbitrage opportunity between two dummy decentralised exchanges.

Then we will create a trade where we buy Dai low from a cheaper dex and sell it high on a costlier dex using USDC.

We will use Aave's flash loan as a leverage to obtain USDC to perform this arbitrage.
To do this we will create a smart contract that does the following in one transaction:

1. Take a flash loan of 1000 USDC
2. Exchange it for Dai from Exchange A where Dai is cheaper
3. Sell the Dai for USDC on Exchange B where it is costlier
4. Pay off the flash loan + fee in USDC
5. Keep the profit
