
!!! note "This is a inventory script"
---
## Setup

You must change this  ==value==:

```lua
Config.MaxDropViewDistance
```

Value must be `max 20`:

```lua
Config.MaxDropViewDistance = 12
```

```lua title="config.lua" linenums="1" hl_lines="2-4"
Config.MaxInventoryWeight = 150000 -- Max weight a player can carry (default 250kg, written in grams)
Config.MaxBackpackWeight = 250000 -- Max weight a player can carry (default 250kg, written in grams)
Config.MaxBodyWeight = 125000 -- Max weight a player can carry (default 250kg, written in grams)
Config.MaxInventorySlots = 15 -- Max inventory slots for a player
Config.MaxBackpackSlots = 40 -- Max inventory slots for a player
Config.CleanupDropTime = 15 * 60 -- How many seconds it takes for drops to be untouched before being deleted
Config.MaxDropViewDistance = 12.5 -- The distance in GTA Units that a drop can be seen
Config.UseItemDrop = true -- This will enable item object to spawn on drops instead of markers
Config.ItemDropObject = `prop_nigel_bag_pickup` -- if Config.UseItemDrop is true, this will be the prop that spawns for the item

Config.ItemLoadMs = 6    --İtem load time ((item.weight * item.amount) / Config.ItemLoadMs)  higher == lower loading time
Config.MaxDistance = 5.0 -- determines how far you can place the item from the player

Config.DefaultHatItem = "hat" 
Config.DefaultMaskItem= "mask"
Config.DefaultGlassesItem= "glasses"
Config.hatitems = {"hat","hat_blue"}
Config.maskitems = {"mask","mask_blue"}
Config.glassesitems = {"glasses","glassess_2"}
Config.armoritems = {"armor"}
Config.clotheitems = {"mask","glasses","hat"}
Config.walletitems = {"wallet","id_card"}
Config.phoneitems = {"phone","phone_blue"}
Config.keyitems = {"key","key_blue"}
Config.carditems = {"card","mastercard","visa"}

Config.backpackitems = {"backpack","moneybag"}
```