## ✨ New Features

  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/28c12d2)☢️ Antimatter schematics and QMD config tweaks
    > > Contributed by [evollbrecht](https://github.com/evollbrecht)
    >
    > 1. Add schematics for QMD antimatter synthesis complex, compressed air ->liquid helium process using multiblock distiller + liquefiers, and 7TRF/t mercurial steam turbine  
    > 2. Tweak tube heat transfer rate (NC) and liquefier nozzle speed (QMD) values by factor of 16.6666666667 for parity with generic NC machine buff  
    > 3. Reduce exotic containment chamber explosion size scaling factor (QMD) from 50 -> 1 to make containment failures (which can be triggered on load/unload through no fault of the player) less devastating  
    > 4. Tweak antimatter turbine dynamo coil conductivity multipliers (NTP) by factor of 600 to encourage setting up antimatter production  
    > 5. Remove high pressure mercury reservoirs (Tweaked Petroleum) from Kepler 0119 so it can only be produced via nucleosynthesis
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/dd9e312)✏️`Industrial Foregoing` integration
    > - 📖 Chapter moved up in quest arrangement, change icon  
    > - 📖 ![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/mob_duplicator__0.png "Mob Duplicator") removed from quest and propose RFTools spawner instead  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/iceandfire/dragon_ice_spikes__0.png "Dragon Ice Spikes") now uncraftable in Crafting Table - obtain through ![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/froster__0.png "Froster") instead  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/teslacorelib/speed_tier1__0.png "Speed Upgrade I")![](https://github.com/Krutoy242/mc-icons/raw/master/i/teslacorelib/speed_tier2__0.png "Speed Upgrade II") Now require ![](https://github.com/Krutoy242/mc-icons/raw/master/i/iceandfire/dragon_ice_spikes__0.png "Dragon Ice Spikes")  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/item_extract_speed_upgrade__0.png "Extract Speed Upgrade") replace 2x![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/item_alloy_ingot__0.png "Electrical Steel Ingot") with ![](https://github.com/Krutoy242/mc-icons/raw/master/i/iceandfire/dragon_ice_spikes__0.png "Dragon Ice Spikes")  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/floralchemy/flooded_soil__0.png "Flooded Soil") now only obtainable through ![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/sludge_refiner__0.png "Sludge Refiner")  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/tconevo/metal__15.png "Essence-Infused Ingot") way harder and stronger material (old recipe currently not removed yet)  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/range_addon__8.png "Range Addon") now buyable from villagers  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/sludge_refiner__0.png "Sludge Refiner") clear vanilla item output and add some modded  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/wither_builder__0.png "Wither Builder") now require Protein instead of ![](https://github.com/Krutoy242/mc-icons/raw/master/i/minecraft/nether_star__0.png "Nether Star")  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/villager_trade_exchanger__0.png "Villager Trade Exchanger") harder  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftoolsdim/time_absorber__0.png "Time Absorber")![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftoolsdim/biome_absorber__0.png "Biome Absorber")![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftoolsdim/liquid_absorber__0.png "Liquid Absorber")![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftoolsdim/feature_absorber__0.png "Feature Absorber")![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftoolsdim/terrain_absorber__0.png "Terrain Absorber")![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftoolsdim/material_absorber__0.png "Material Absorber") now require IF materials and harder to craft  
    > - ✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/rftools/spawner__0.png "Spawner") harder
  * <img src="https://i.imgur.com/eNnemGK.png" align=right> [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/cc28e47)🎒Add content preview for ![](https://github.com/Krutoy242/mc-icons/raw/master/i/trinity/medium_container__0.png "Medium-shielded Nuclear Pig")![](https://github.com/Krutoy242/mc-icons/raw/master/i/trinity/heavy_container__0.png "Heavily-shielded Nuclear Pig")![](https://github.com/Krutoy242/mc-icons/raw/master/i/trinity/light_container__0.png "Lightly-shielded Nuclear Pig")
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/c31c39b)📱Make VICE a bauble
    > > Contributed by [TabakaSIM](https://github.com/tabakasim)
    >
    > Now you can place the ![](https://github.com/Krutoy242/mc-icons/raw/master/i/vaultopic/vice__0.png "V.I.C.E. (Vaultopic Item Crafting Entity)") in a **baubles** slot to free up space in your inventory

  #### Build_expansion

  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/aec0d28)🛣️Speed up player steel/alum scaffold blocks
    > List of affected blocks:  
    > - ![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/metal_decoration1__3.png "Steel Scaffolding")![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/metal_decoration1_slab__3.png "Steel Scaffolding Slab")![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/steel_scaffolding_stairs2__0.png "Steel Scaffolding Stairs")![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/metal_decoration1__7.png "Aluminium Scaffolding")![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/aluminum_scaffolding_stairs2__0.png "Aluminium Scaffolding Stairs")![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/metal_decoration1_slab__7.png "Aluminium Scaffolding Slab")

  #### Quest

  * <img src="https://i.imgur.com/5CsrNuC.png" align=right> [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/e1883fb)📖Lootboxes has chance to give box next tier
    > Now "upcraft" is available again 🎉

## 🐛 Fixes

  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/4623bd4)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/chemthrower__0.png "Chemical Thrower") add ![](https://github.com/Krutoy242/mc-icons/raw/master/i/quark/iron_plate__0.png "Iron Plate")➜![](https://github.com/Krutoy242/mc-icons/raw/master/i/quark/iron_plate__1.png "Rusty Iron Plate")
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/ea9a2c2)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/fertilizer__0.png "Fertilizer") rename to "Manure"
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/5df503a)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/twilightforest/magic_beans__0.png "Magic Beans") fix inastantly smelted in Rat's inventory
    > Now it made with Gemcutter instead
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/ee3a013)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/requious/replicator__0.png "Replicator") doesn't save player difficulty on leave
    > Now, Replicator owned by other player will show correct difficulty, even if other player leave server
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/3707705)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/aeadditions/terminal.universal.wireless__0__484a6a92.png "Wireless Universal Terminal - Item") remove since not working
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/759d7ea)🌺Update quest description for [Rokku Eryngium]
    > > Contributed by [TabakaSIM](https://github.com/tabakasim)
    >
    > Update quest description for Rokku Eryngium that it uses redstone
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/52bef0d)💥[Creative harvest] remove effect to prevent crashes with shaders
    > > Contributed by [Maxim](https://github.com/maxim)
    >
    > - removed enchantment effect from creative harvest blocks if shaders is on  
    > - added back crafts from previous versions before creative harvest was removed  
    > - removed ![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/poweroverload__0.png "Power Overload") cuz its useless now
    > 
    > related: 9f2cf8e25ebc9a3b131cb9516c3e264462332aa6
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/122d720)💥Fix crash when depleting Chisel inside ![](https://github.com/Krutoy242/mc-icons/raw/master/i/chisel/auto_chisel__0.png "Auto Chisel")
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/13b75ab)💰Fix cooked meat drop
    > > Contributed by [TabakaSIM](https://github.com/tabakasim)
    >
    > - Fix some entities doesn't drop cooked meat (TF deer)  
    > - Fix Quark's Frog always drop cooked legs
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/fcb2891)🖼️`Icon.png` add to modpack folder
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/6d9736e)🧩Double max amount of chat lines

  #### Balance

  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/2a66473)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/trinity/bomb_antimatter__0.png "Antimatter Bomb") buff explosion radius x10 times
    > Because "antimatter" should sounds cool ('cool' is 2500 blocks radius)
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/f315b8a)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/mekanism/machineblock2__8.png "Chemical Crystallizer") cheaper
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/602d1b5)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/mekanism/energycube__0__633a472e.png "Creative Energy Cube") increase RF output to 250M RF/t
    > To match intended value
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/e8973cf)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/draconicevolution/magnet__0__8dda9da8.png "Item Dislocator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/draconicevolution/magnet__1.png "Awakened Item Dislocator") cheaper
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/93c6f2e)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/mob_duplicator__0.png "Mob Duplicator") harder
    > - Only available in ![](https://github.com/Krutoy242/mc-icons/raw/master/i/extendedcrafting/table_elite__0.png "Elite Crafting Table")  
    > - Require less essence to duplicate mobs  
    > - Change IF chapter icon
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/90a29d1)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/industrialforegoing/protein_reactor__0.png "Protein Reactor") nerf to not overshadow ![](https://github.com/Krutoy242/mc-icons/raw/master/i/gendustry/liquifier__0.png "Protein Liquifier")
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/e87798b)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/rainbowgenerator__0.png "Rainbow Generator!") cheaper
    > Rainbow generator recipe now reset to default one (just two halves). The main challenge is to automate all generators, not to craft the Rainbow one
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/a1c2a6e)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/randomthings/spectrecoil_number__0__91a75d81.png "Spectre Coil Nr. 48") nerf 32➜16 rf/t
    > Because its one of the most popular power source now.
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/b8e8f91)✏️![](https://github.com/Krutoy242/mc-icons/raw/master/i/draconicevolution/draconium_capacitor__0.png "Wyvern Flux Capacitor")![](https://github.com/Krutoy242/mc-icons/raw/master/i/draconicevolution/draconium_capacitor__1.png "Draconic Flux Capacitor") buff capacity x2.5
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/e0d2d06)✏️Buff EnderIO one-block fluid generators
    > - ![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/block_zombie_generator__0.png "Zombie Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/block_franken_zombie_generator__0.png "Frank'n'Zombie Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/block_ender_generator__0.png "Ender Generator") now around 200K - 600K RF/t
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/b4b422d)✏️More ![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/item_material__69.png "Simple Machine Parts") from ![](https://github.com/Krutoy242/mc-icons/raw/master/i/ic2/resource__13.png "Advanced Machine Casing")
    > Now x64
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/396b6ab)✏️Rebalance some EU2 generators
    > - ![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/machine__0__b70ff0c3.png "Explosive Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/machine__0__1c91fbcd.png "Magmatic Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/machine__0__48e64d61.png "Heated Redstone Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/machine__0__23d29ce3.png "Pink Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/machine__0__1615b97.png "Netherstar Generator")![](https://github.com/Krutoy242/mc-icons/raw/master/i/extrautils2/machine__0__fa0d9f51.png "Slimey Generator")
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/50d2399)✏️Reduce efficiency of low-tech ingredients for Gendustry fluid producers
    > Its always easier to spam x20 times more ![](https://github.com/Krutoy242/mc-icons/raw/master/i/ic2/nuclear__0.png "Enriched Uranium Nuclear Fuel") for Mutagen rather than breed isotopes. Now uranium will provide only 1 mutagen (was 20).
    > 
    > Also affected Protein from ![](https://github.com/Krutoy242/mc-icons/raw/master/i/rats/raw_rat__0.png "Raw Rat"), Liquid DNA from Drones.
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/d8deafe)💰![](https://github.com/Krutoy242/mc-icons/raw/master/i/botania/magnetring__0.png "Ring of Magnetization")➜![](https://github.com/Krutoy242/mc-icons/raw/master/i/enderio/item_magnet__0.png "Electromagnet") in Dragon caves
    > Also decrease chance of ![](https://github.com/Krutoy242/mc-icons/raw/master/i/botania/manaring__0__cf0d55ca.png "Band of Mana")![](https://github.com/Krutoy242/mc-icons/raw/master/i/botania/auraring__0.png "Band of Aura")

  #### Quest

  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/ecbde48)📖![](https://github.com/Krutoy242/mc-icons/raw/master/i/excompressum/chicken_stick__0.png "Chicken Stick") add note that unbreakable
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/f741d76)📖![](https://github.com/Krutoy242/mc-icons/raw/master/i/immersiveengineering/coresample__0.png "Core Sample") add note about placement on ground disabled
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/4a5757a)📖`Environmental Tech` change gate task to frame
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/7f70677)📖Add ![](https://github.com/Krutoy242/mc-icons/raw/master/i/engineersdecor/factory_hopper__0.png "Factory Hopper") quest
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/563ae4d)📖Add hint about Katana damage in robot's hands
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/92d8dd8)📖Buff `Rare`+ loot crates
    > Also tierup some loot rewards in quests
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/ba6018e)📖Fix "Infinity decoratives" dank null not working
    > Thx `FleetingDream` for the hint.
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/334aed0)📖Fix `Applied Energetics` typo
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/cf207a0)📖Move "materials" selling to uncommon
  * [🖇](https://github.com/Krutoy242/Enigmatica2Expert-Extended/commit/48d5e3c)📖Rearrange some quest chapters

## Mods changes
### 🟢 Added Mods

Icon | Summary | Reason
----:|:--------|:-------
<img src="https://media.forgecdn.net/avatars/thumbnails/467/621/30/30/637749625001219720.png"            > |                              [**Reach Fix**](https://www.curseforge.com/minecraft/mc-mods/reach-fix)                    <sup><sub>ReachFix-1.12.2-1.1.3.jar                        </sub></sup><br>Fix for vanillas hit detection and the reach attribute not being used for entities. | Recommended by [BareBonesTemplatePack](https://github.com/Invadermonky/BareBonesTemplatePack)
<img src="https://media.forgecdn.net/avatars/thumbnails/846/951/30/30/638246065460259726.png"            > |                           [**Packet Fixer**](https://www.curseforge.com/minecraft/mc-mods/packet-fixer)                 <sup><sub>PacketFixer-forge-2.1.0-1.12.2.jar               </sub></sup><br>A simple mod to solve various problems with packets, NBTs and timeouts. | Recommended by [BareBonesTemplatePack](https://github.com/Invadermonky/BareBonesTemplatePack)
<img src="https://media.forgecdn.net/avatars/thumbnails/870/417/30/30/638286915262284750.png"            > |                    [**Advancement Locator**](https://www.curseforge.com/minecraft/mc-mods/advancement-locator)          <sup><sub>cta-1.12.2-1.2.2.jar                             </sub></sup><br>Got an advancement but have no idea where it is? | Recommended by [BareBonesTemplatePack](https://github.com/Invadermonky/BareBonesTemplatePack)
<img src="https://media.forgecdn.net/avatars/thumbnails/1422/169/30/30/638921443005429425.png"           > |             [**LemonSkin (AppleSkin Fork)**](https://www.curseforge.com/minecraft/mc-mods/lemonskin)                    <sup><sub>lemonskin-4.0.0.jar                              </sub></sup><br>AppleSkin continuation for 1.12.2 | Recommended by [BareBonesTemplatePack](https://github.com/Invadermonky/BareBonesTemplatePack)
-----------


### 🔴 Removed Mods

Icon | Summary | Reason
----:|:--------|:-------
<img src="https://media.forgecdn.net/avatars/thumbnails/47/527/30/30/636066936394500688.png"             > |                              [**AppleSkin**](https://www.curseforge.com/minecraft/mc-mods/appleskin)                    <sup><sub>AppleSkin-mc1.12-1.0.14.jar                      </sub></sup><br>Adds some useful information about food/hunger to the HUD | Replaced by 🍋
<img src="https://media.forgecdn.net/avatars/thumbnails/106/654/30/30/636360849723336023.png"            > |                    [**Better Advancements**](https://www.curseforge.com/minecraft/mc-mods/better-advancements)          <sup><sub>BetterAdvancements-1.12.2-0.1.0.77.jar           </sub></sup><br>Successor to BetterAchievements for the new advancements system in minecraft 1.12+ | Comes out we dont need it 🤷‍♂️
-----------

### 🟡 Updated Mods

Icon | Summary | Old / New
----:|:--------|:---------
<img src="https://media.forgecdn.net/avatars/thumbnails/1041/903/30/30/638568420563290317.png"           > |                    [**Forgelin-Continuous**](https://www.curseforge.com/minecraft/mc-mods/forgelin-continuous)         | <nobr>Forgelin-Continuous-2.2.0.0</nobr><br><nobr>Forgelin-Continuous-2.3.20.0</nobr>
<img src="https://media.forgecdn.net/avatars/thumbnails/468/506/30/30/637752171904887013.jpeg"           > |                       [**Had Enough Items**](https://www.curseforge.com/minecraft/mc-mods/had-enough-items)            | <nobr>HadEnoughItems_1.12.2-4.29.15</nobr><br><nobr>HadEnoughItems_1.12.2-4.30.2</nobr>
<img src="https://media.forgecdn.net/avatars/thumbnails/625/955/30/30/638021348641896375.png"            > |               [**Flare (Spark for 1.12.2)**](https://www.curseforge.com/minecraft/mc-mods/flare)                       | <nobr>flare-0.7.0</nobr><br><nobr>flare-0.8.0</nobr>
<img src="https://media.forgecdn.net/avatars/thumbnails/1001/840/30/30/638521728187451529.jpg"           > |           [**Advanced Rocketry - Reworked**](https://www.curseforge.com/minecraft/mc-mods/advanced-rocketry-2)         | <nobr>advancedrocketry-2.2.4</nobr><br><nobr>advancedrocketry-2.2.5hotfix</nobr>
<img src="null"                                                                                          > |                                  [**ARLib**](https://www.curseforge.com/minecraft/mc-mods/arlib)                       | <nobr>ARLib-17-09-2024</nobr><br><nobr>libvulpes-0.5.1</nobr>
<img src="https://media.forgecdn.net/avatars/thumbnails/1744/676/30/30/639110116041767573.png"           > |                            [**Curvy Pipes**](https://www.curseforge.com/minecraft/mc-mods/curvy-pipes)                 | <nobr>curvy_pipes-1.12.2-1.13.5</nobr><br><nobr>curvy_pipes-1.12.2-1.14.2</nobr>
<img src="https://media.forgecdn.net/avatars/thumbnails/1723/373/30/30/639096406588694749.png"           > |                           [**Armored Arms**](https://www.curseforge.com/minecraft/mc-mods/armored-arms)                | <nobr>ArmoredArms-v1.5.0-1.12.2-betta</nobr><br><nobr>ArmoredArms-v1.5.1-1.12.2-release</nobr>
-----------
