# WoM rewards for GSC

From the 9th GSC, [Minesweeper Online](https://minesweeper.online/) resources are added to the pool to bring more motivation and attract international players. Anyone can sponsor GSC by donating resources to an [official account](https://minesweeper.online/player/5619613). Any kind of resources are accepted while different resources apply different allocating rules. All resources fall into one of the following categories:
- Currency: coins and gems. The prices of gems are relatively stable so we can do conversions. Currently, 1 gem = 395 coins.
- Floating-value items: tickets and equips.

The allocation start from the top players (in terms of T.37). Every player can pick either currency or **one** floating-value item. The amount of currency the player can get is calculated as follows:

- The 1st can get the maximum between 200k or 5% of total currency pool. We calculate the ratio `p` by `p = (top prize)/pool`. For example, if the pool is 2M, then p=10%. If the pool is 5M, then the top prize is 250k and p=5%.
- The following players can get up to `p*(remaining pool)`, rounded up. For example, if the pool is 2M and the first player takes 200k, then the second player can take up to 1.8M\*10%=180k. If the first player takes an equipment instead, then the second player can take up to 200k. Taking less than what you can get or taking a floating-value item will affect everyone downstream.

The official account will contact the player in turn via Minesweeper Online. The player needs to send an exchange to the official account to claim their rewards. If a player doesn't do this in 24 hours, they will be "hanged up". When they return later by replying to the official account, their status will become "back" and will be called after a reward is successfully allocated. For example, suppose the queue is `A->B->C`. The official account contacts A first but A doesn't respond in 24 hours, then the official account turns to B. Suppose that A comes back when B is pending. If B takes their rewards, A will be the next to pick rewards. If B also doesn't respond in time and is hanged up, A will need to wait for C's decision, etc.

If two players are both back after being hanged up, they will be called in the order of their ranking. After we reach the end of ranking, we start to call those who are back. Then all hanged-up players have 1 chance in 1 week to get an equip or a ticket by sending an exchange to the official account. The exchanges will be accepted by the order of their indices. For example, if two players hit the same single item, only the exchange with smaller index will pass while the other will be discarded, meaning that one player will get nothing. After the week, the allocation is over and the pool is open for donation.
