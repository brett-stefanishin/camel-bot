# Camel Bot

Camel Bot is a trading strategy that determines instances which it is profitible to enter or exit a trade.

### Established rules of strategy
__1.__ We assume that the price of Bitcoin will be worth (p)r more than it is today, where r is the discount rate and p is the price per 1 bitcoin. We cam express this as a geometric sequence.
__(p)r + (p)r^2 + (p)r^3 + . . . + (p)r^n__ 

__2.__ Trading in a volitile market shall lock the strategy. For the time being, a 5% change in p would lock the bot. 

__3.__ The bot will be strictly limited to 2 trades per 24 hour period, with one buy execution and one sell execute, respectivley. Note that the amount of orders can be unlimited, but once an order is executed upon, all other orders are cleared.
