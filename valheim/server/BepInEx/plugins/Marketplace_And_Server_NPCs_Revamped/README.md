﻿![https://i.imgur.com/CkSehPu.png](https://i.imgur.com/CkSehPu.png)
![https://i.imgur.com/dBf99Od.png](https://i.imgur.com/dBf99Od.png)

Like my mods? Support me:
Paypal: war3spells@gmail.com

## Mod adds 7 different NPCs to server so admins can configure them from serverside with no need to restart server for applying settings:

1) Marketplace NPC - allows players to sell/buy items by setting them on marketplace with setting quantity + price. Even if player is offline he still will get gold if someone buys his item. (Player will need to get his gold by clicking "Income" button in right bottom).

2) new Trader NPC - is basically a trader npc that exchanges items that admins set in TraderProfiles.cfg. This file is auto-updated into serverside so that you don't need to restart server for applying new items to a trader.

3) Banker NPC - allows people to store any quantity of items in it

4) ServerInfo NPC -  shows text info from ServerInfoProfiles.cfg file which is also updated in runtime. Rich-text is automaticly applied to text, so you can use <color=red> </color> and other rich text markers. Also I added custom <button>Name, link, width, height<button> mark so you can add dynamic buttons to your server info

5) Teleporter NPC - teleport-hub that allows admins to set up teleport points in any place of map. Can use different profiles as any other NPC in TeleportHubProfiles.cfg

6) Gambler NPC - adds gamble system in game

7) Quests NPC - adds quest system in game that allows admins to create their own quests for players with custom targets/types/rewards/conditions

![https://i.imgur.com/iWZO1dp.png](https://i.imgur.com/iWZO1dp.png)

<details><summary>How to spawn/change NPC:</summary>
<p> 

1) Add yourself as server admin

2) Open console (F5) and write: spawn marketplacenpc

![https://i.imgur.com/gDYUi8R.png](https://i.imgur.com/gDYUi8R.png)

3) To control NPC (change profile, override model, override name, snap to ground and rotate or change NPC type) press Shift + Interact on NPC

![https://i.imgur.com/lQ5SPQf.png](https://i.imgur.com/lQ5SPQf.png)

Menu:

![https://i.imgur.com/5A9Fgx4.png](https://i.imgur.com/5A9Fgx4.png)

Change NPC Type => Changes NPC type to chosen one

Change NPC Profile => Changes NPC profile string so Seller/Buyer/Info/Teleporter can change its values from config

Override NPC Name => Overrides NPC name to any string. Can apply rich text to it (font size, font color) with <color> and e.t.c

Override NPC Model => Overrides NPC model to your chosen Creature Prefab from Valheim (you can also use modded creatures)

Apply => Apply options

</p>
</details>
<details><summary>Main Options Config:</summary>
<p> 
All main options are located in BepInEx/MarketplaceKG/MarketPlace.cfg

![https://i.imgur.com/O1wcMwZ.png](https://i.imgur.com/O1wcMwZ.png)

OnlyEpicLootItems => If true, then players will be able to sell ONLY ITEMS WITH EPICLOOT EFFECTS in marketplace

ItemMarketLimit => limit of max slots that player can place in marketplace (I recommend to leave it on 15)﻿

MarketTaxes => This % of gold will be reduced for seller to get after his item is sold

VIPplayerTaxes => **## This taxes will be applied instead of usual one if player is in VIP list

BlockedPlayers => steam ids (write each after , ) that can't use marketplace

VIPplayersList => steam ids (write each after , ) that have different taxes value

CanTeleportWithOre => can player use teleport hub (teleporte npc) with ore in their inventory

BlockedPrefabs => prefab on each line is prohibited to sell in marketplace

</p>
</details>

<details><summary>Marketplace NPC:</summary>
<p> 

![https://i.imgur.com/qKLkeIu.png](https://i.imgur.com/qKLkeIu.png)

Marketplace allows player to add item in market slot and for other player to buy it. After your item slot bought, you get gold in "Income" tab. Player will get gold in "Income" even if seller is offline. ﻿

In order for seller to get his gold you need to click INCOME button.

Players can cancel their own lots after pressing on it and clicking "CANCEL"

![https://i.imgur.com/QQNDo5f.png](https://i.imgur.com/QQNDo5f.png)

Marketplace 100% supports EpicLoot mod with all its MagicItemEffects and extentions:

![https://i.imgur.com/xL8JFFK.png](https://i.imgur.com/xL8JFFK.png)

"My Sales" button allows you to see only YOUR sales so you can cancel them

</p>
</details>

<details><summary>Seller NPC:</summary>
<p> 

1) In order for admin to change Seller NPC data you need to go BepInEx/config/MarketplaceKG/SellerProfiles.cfg

![https://i.imgur.com/q5s4Nxi.png](https://i.imgur.com/q5s4Nxi.png)

![https://i.imgur.com/e0xAQR6.png](https://i.imgur.com/e0xAQR6.png)

In Order to add items to seller you need to add each item in new line with template: ItemPrefab , Count , Price
All items will automatically be added into [default] profile. 

If you want to add items in specific profile you need to write [profilename] and then start adding items with new line each

Example:

![https://i.imgur.com/PnEl06g.png](https://i.imgur.com/PnEl06g.png)

﻿Here I added two profiles Profile1 and Profile2 with items in each.
Then You should apply profile to Seller NPC inside game with NPC UI :

![https://i.imgur.com/qJtJjua.png](https://i.imgur.com/qJtJjua.png)

Result:

![https://i.imgur.com/CJCwWct.png](https://i.imgur.com/CJCwWct.png)

If you assign Profile2 it will have different items﻿﻿
</p>
</details>

<details><summary>Buyer NPC:</summary>
<p> 
It does SAME as Seller NPC but instead of Selling N Items for X gold it BUYS N items for X gold.

All Buyer Data is inside BepInEx/config/BuyerProfiles.cfg. 
Data has same structure as Seller NPC:

![https://i.imgur.com/dOkBoHO.png](https://i.imgur.com/dOkBoHO.png)

Result:

![https://i.imgur.com/7SDTOnb.png](https://i.imgur.com/7SDTOnb.png)﻿

</p>
</details>

<details><summary>Info NPC:</summary>
<p> 

NPC will read info from ServerInfo.cfg and display that on GUI.
Rich text markers can be applied to text you write. [Guide](https://docs.unity3d.com/Packages/com.unity.ugui@1.0/manual/StyledText.html) 
Also if you want to add button in your GUI (that will open any link), you can use <button>Name of button, link to site, width, height<button>

ServerInfo npc uses "default" profile by default. But you can add as many info profiles you want (same as Trader NPC profiles). Example below:

![https://i.imgur.com/sD7wex8.png](https://i.imgur.com/sD7wex8.png)

Non-profiled text will be applied to every new Info NPC with "default" profile. But if you want to add your own you need to add new line with [ProfileName] and then in new line write your text you want
</p>
</details>

<details><summary>Teleporter NPC:</summary>
<p> 

NPC acts as teleport-hub but all in one. Its profile/data controlled by BepInEx/MarketplaceKG/TeleportHubProfiles.cfg

![https://i.imgur.com/RY551NN.png](https://i.imgur.com/RY551NN.png)

To Add new teleport spots you need to add them new line each with structure: Spot Name, X coord, Y coord, Z coord, Icon name

You can add Icons in BepInEx/config/MarketplaceKG/MapPinsIcons folder

![https://i.imgur.com/yZVRMLF.png](https://i.imgur.com/yZVRMLF.png)

I recommend you to use 32x32 icons. 
Also you can write ItemPrefab name instead of icon in order to use its icon as map pin
When you click Interact on Teleporter NPC with profile you will open map and it will show pins to you. After Left Mouse click on icon you will teleport to XYZ coords of spot.

![https://i.imgur.com/Hoy6Gg1.png](https://i.imgur.com/Hoy6Gg1.png)

XYZ COORDS SHOULD BE INTEGERS VALUE ONLY (5.6 <= WRONG, 5 <= good)﻿
</p>
</details>

## ALL OPTIONS / PROFILES / NPCs DATA ARE AUTO-RELOADED IN SERVER RUNTIME WITHOUT RESTART

## ![https://i.imgur.com/5ZHfxlo.png](https://i.imgur.com/5ZHfxlo.png)

## To install mod place MarketPlaceRevamped.dll into Client Plugins folder AND Server Plugins Folder


![https://i.imgur.com/gTTJ9HJ.png](https://i.imgur.com/gTTJ9HJ.png)

﻿For Questions or Comments, find ## KG![https://i.imgur.com/CPYNjXV.png](https://i.imgur.com/CPYNjXV.png)﻿ in the Odin Plus Team Discord:
[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/5gXNxNkUBt)