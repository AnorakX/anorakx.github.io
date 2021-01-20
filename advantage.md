---
layout: post
title: Advantage
---
> Advantage is a custom economy/leveling/server management bot with dynamic inventories, balances, and shops.

## the idea
Tired of the restrictions of many "custom economy/leveling" bots, I decided to use my knowledge of MongoDB and Python that I gained from 
[Dropship](https://anorakx.github.io/dropship) to create an economy and leveling systemfor my server, 
([The Grand Order](https://discord.gg/FQ6wwRe)).
## the inspirations
I have used many custom bots to improve my server. These are some of the bots that most heavily influenced Advantage:
- [Dank Memer](https://top.gg/bot/memes)
- [ActivityRank](https://top.gg/bot/534589798267224065)
- [Color-Chan](https://top.gg/bot/436515089441488907)
## the features
In the end, Advantage contained:
- Individual inventory, balances, bank and trinkets
- Trinket spawns
- Bank upgrades
- Different sectors (I'll explain these later)
- Individual command cooldowns
- A `work` command with different tasks based on sectors
- A `beg` command with different tasks based on sectors
- A `daily` command 
- A `rob` command
- Automatic rewards for voting for the server on top.gg
- A shop with gems, crates, and trinkets
- Rewards for boosting the server
## the components
### balances, bank, and trinkets
This was the most basic part. The idea was that your <i>card</i> could be robbed by others using the `rob` command, but your <i>bank</i> couldn't. However, your bank had to be upgraded using money. This was an idea I got primarily from Dank Memer. 
Trinkets were something I thought of myself. They were collectible items that could be received from <i>Trinket Bags</i> (a random lootbox) or randomly spawned when you ran commands. Each had a name, description, and rarity that connected in some way to the server's history or members.
### work, beg, daily, and rob
These were perhaps the most challenging and time-consuming commands to code. Each command yielded a random amount of currency (called <i>credits</i>) based on its cooldown. 
### leveling
One of the most effective ways to make a server active is a good leveling system. I also wanted the leveling system and economy system to work closely together (you'll see this in the next section with gems, medals and crates). Some of the features of leveling were:
- Auto-roles (roles would automatically be added/removed based on level)
- `daily` and `vote` earnings scale with level
- Some items in the shop (such as colors) can only be bought when levels are reached
### gems, medals, and crates
Gems were currency multipliers and medals were leveling multipliers. Both could be bought with credits. The idea was to incentivize activity during periods when people had multipliers on. 
Crates were random lootboxes with specified chances that gave out gems, medals, and trinkets alike.
### colors
Many servers use colors to incentivize economy, and I thought that was a good idea. 
### sectors
Halfway along, I thought of different <i>sectors</i>. These were different "locations" that the user could move to by spending a certain amount of credits and `work`, `beg`, and `rob` would have different chances or earnings, but I only ever coded 2 sectors.
## conclusion 
<u>If I were given the chance to re-do, I would:</u>
- My biggest do-over would be dynamic cooldowns. I used Discord.py's built-in cooldowns, which caused a lot of problems. I couldn't reset cooldowns or alter them, which I would've liked, and if someone used a bugged command it was always in a cooldown. Whenever I restarted the program, cooldowns also restarted.
- Fix bugs. Advantage was pretty buggy at the beginning, and I wish I'd known better.
- A gambling module. A lot of bots have this, and I'm working on it for my next economy bot. 

<b>Advantage was a project where I learned to do a lot. It was an ambitious project that enhanced my Discord.py and propelled me into really making Discord bots.</b>
