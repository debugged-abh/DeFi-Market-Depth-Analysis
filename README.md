Market Depth Analysis:
The ultimate goal is to calculate market depth for the Ekubo Protocol for STRK/ETH, STRK/USDC, ETH/USDC, USDC/USDT pools. We will do that in a series of steps.
Step 1
Calculate and report the current price ratio for each pool in the dataset. Note that there are multiple pools for a given pair.
Step 2
Create a data structure to store all current liquidity in each pool according to their tick deltas
A tick delta is the net amount of all liquidity starting/ending in a given price tick. Tick deltas are positive when liquidity starts in a given tick and negative when it ends there (on net). The sum of all tick deltas in a pool must be zero, as all liquidity has a lower bound where it starts and an upper bound where it ends.
Step 3
Create a function that takes a set of tick deltas, the current price, and a price range and outputs the number of token0 and/or token1 in that price range
Step 4
Report the 1%, 5%, and 10% market depths for STRK/ETH, STRK/USDC, ETH/USDC, USDC/USDT using your function above. You can report them denominated in amounts of both tokens rather than USD. (NB: You will have to calculate market depths for each pool and then sum over them to get the market depth for a pair, as there are multiple pools for a given pair)
