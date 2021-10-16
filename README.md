# lotto-lottery
Tezos lottery smart-contract
Made for Tezos SmartPy Developer Course

## Instructions
Write a lottery smart contract
The way this simple lotto works is as follows.

- A ticket costs 0.01 xtz
- After 5 tickets are sold, a winning ticket is randomly chosen.
- The purchaser of that ticket is randomly selected and gets all the funds (0.05) collected by the lotto.
- Lotto restarts

Notes:
- Keep a map that maps ticket numbers (keys) to addresses (values).
- Use 'now' timestamp to get a random value (note this is not truly random and can be gamed in a true lottery). Use that value to select winner.
- Someone can send more than 0.01 to buy multiple tickets at once. I.e. sending 0.04 will give them 4 tickets.
- If someone sends more money than number of tickets available, you can either send them back the extra money, or just enter them into the next lottery.
- You can reject payments that aren't a perfect multiple of the number of tickets.

Modifications - further exercises:
- Allow the number of tickets for the lottery to be modified, within some range, before any tickets are sold.
- Allow the ticket price to be modified, within some range (before any tickets are sold).

