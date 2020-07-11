# dca
Dollar Cost Averaging
Credit goes to Brianddk. Found this DCA script via his reddit post here: https://old.reddit.com/r/BitcoinBeginners/comments/gy5qe2/dollar_cost_averaging/

1. Determine annual investment goal then divide by 365 (daily=goal/365)
2. Every day ACH daily amount into Gemini (or CB Pro)
3. If I buy anything with BTC via FOLD or whatever, add that to my daily deposit
4. Cancel the previous days limit orders if any exist (see below)
5. Every day split my available USD balance in to 20 pieces (piece=usd_bal/20)
6. Buy one piece as market order at spot
7. Spread the other 19 as downward limit orders
8. Set the limit orders at spot minus 0.5%, 1.0%, 1.5%, 2.0%, ... 10.0%


This does a couple of things. It "buys extra" on dips, it ensures you "buy some" every day, it fulfills "buy and replace" to support BTC merchants, and it allows you to tolerate one or two days of downtime.

It can all be done in 5 minutes over morning coffee, though I went ahead and wrote a python script to do it for me.
