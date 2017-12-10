To work on this repo, always make a branch with a description of your task and group. When finished, make a pull request into 'master'


First task:

"Hi Cody

This library can be one of the starting points, althouth you may find
better ones.
https://github.com/alecalve/python-bitcoin-blockchain-parser


Here are some tasks

1. For example this tweet summarizes some ideas

https://twitter.com/VinnyLingham/status/939554077817503744

Can you quantify those into Python pandas format.

Each hour will have last value occurred during that hour.

For example
                              mempool size        miner profitability
       block times
12/9/2017 18:00     10020012               2020                             900
12/9/2017 19:00     10050052               2010                             920
...

Times should be in UTC.

..."

Please read through the Twitter comments, a few of them have value to what we're doing. Mostly the man who is pinging links to his site:

https://jochen-hoenicke.de/queue/#30d

https://jochen-hoenicke.de/queue/#2h

He is nice enough to give this away for free (at bottom of that site):

https://github.com/jhoenicke/mempool

His mempool system can be used to get the "mempool size"

So for now we just need "mempool size" and "miner profitability" of the bitcoin blockchain on an hourly basis.

I would start by:

1. Reading his mempool package

2. Google "bitcoin blockchain parser python" 
I found https://github.com/toidi/pyblockchain
A few more come up

We need to:

Write a client that grabs "mempool size" and "miner profitability" once per hour and writes to a DB
