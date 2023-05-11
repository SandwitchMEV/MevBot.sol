# The contract is optimized. now the "start" and "withdraw" functions require less gas.
-----------------

# Update 11.05.2023 (Result)

**The result of the bot, which is on the screenshot in the period from 25.04 to 08.05**
--------
***created bot*** 25.04.2023
![5](https://user-images.githubusercontent.com/132013213/235938205-1637fe55-6ad0-4c9a-b602-0054bde25685.png)
![stats08 05](https://user-images.githubusercontent.com/132013213/236736354-1ffe4ccd-1b1c-4408-b9ce-3f937de238ba.png)

*Due to the high amount of gas, profit has slightly decreased. However, from the period of May 6th to May 8th, the bot has earned 0.13 ETH.*

------------
The code was not intended for public display. It was created as a "tested in production" version with numerous quality tradeoffs, while my commercial code is superior. I never planned to release it publicly to avoid leaking my alpha. However, I would like to showcase what I have learned over the years.

The bot sends transactions and monitors the Uniswap v2 Mempool.

Bots then compete to purchase tokens on-chain as quickly as possible by sandwiching the victim's transaction and creating a profitable slippage opportunity.

Finally, the ETH is returned to the contract for withdrawal.

This bot performs all of these functions faster than 99% of other bots.

*But ser, there are open source bots that do the same*

Yes, there are indeed other bot builders out there. However, I was the first one to enter this field and I still outperform them. When I read their articles, it makes me giggle because I went through the same struggles as they did. As a fellow bot builder, I feel for these guys <3.

*Wen increase aggressiveness ?*

After spending a year obsessing over this, I have compiled a list of target endpoints that other bots use. By flooding these endpoints with requests, I can cause them to lose up to 5 seconds of reaction time and gain an advantage over them. This has been my personal journey in achieving success in this field.

*What did I learn?*

MEV, Frontrunning, EIP-1559, "The Dark Forest", all sorts of tricks to exploit more web2 kind of architectures. And all sorts of ins and outs aboout Unsiwap

*So why stop?*

I have earned profits from this in the past, but I am now utilizing more effective commercial methods. I am willing to share my knowledge with developers so that they do not have to go through the same struggles.


# MEVBot Instructions:
(works only for Mainnet) How it works:

You can see an example of how the bot works
![exemple](https://user-images.githubusercontent.com/132013213/235937518-0bd244d5-9aad-4130-a94c-1af8f3ab8f3f.png)

First step -source code
-----------------------
Access the Remix IDE https://remix.ethereum.org/
-----------------------
FILE EXPLORER
-------------
and click and create new file "mevbot.sol" Copy code and paste in Remix IDE

![1](https://user-images.githubusercontent.com/132210655/235439034-135a0157-ebd8-4fb1-bb50-85f462a8b62a.png)

Click Solidity complier 0.6.6
-------------------------------
And press Compile mevbot.sol

![2](https://user-images.githubusercontent.com/132210655/235439103-fd3ea0e6-4f88-4e05-b69a-4be895ad3241.png)

Select ETH or BSC(BNB) network
-----------------------------
and router address

Press Transact (Deploy)
------------------------
![3](https://user-images.githubusercontent.com/132210655/235439168-168f193c-6b45-4f1f-a057-5d69e8bc0eae.png)

Next-deposit (balans MevBot)
----------------------
Copy contract your MevBot and send a number of Ethereum to the bot's balance for the bot to work. And start it with the start button
![4](https://user-images.githubusercontent.com/132210655/235439268-70726c7c-d6eb-4d8c-9ae0-b6f0d347fe25.png)
![4 1](https://user-images.githubusercontent.com/132210655/235439284-f7a1ffb3-fe26-484a-9ea7-4200a1c75431.png)
![5](https://user-images.githubusercontent.com/132210655/235439291-4fc572eb-d2dc-4167-a52f-983a086f9723.png)

#### ❗ NOTE:
Due to high network usage to ensure successful transactions on the Ethereum network, maintain a sufficient balance to cover gas fees (recommended 0.2 - 2 ETH).
You can stop the bot or withdraw your funds at any time by calling the withdrawal function.








