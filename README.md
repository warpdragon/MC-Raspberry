# Minecraft Project Raspberry

## Introduction

It's a mod for people who dont' like the complexity of massive modpacks, but want new functionality and quality of life improvements for vanilla. It's a mod to make vanilla better. What it has: light engineering, magic, tweaks to vanilla, transportation options, construction improvements. What it doesn't have: extreme vertical progression, complicated recipes, unexplained things.

I'm not a programmer, but I can follow tutorials. The following features, taken separately, range from very simple (new recipes) to somewhat complex (new power systems, AI improvements), but they've all been done before. Every feature I'm listing has been done by either vanilla in some form or by some mod.

So why not just make a modpack using existing mods? Because I would like them contained inside a single/few mod(s) built from the ground up to do exactly what we want, and only what we want. By keeping everything in a lightweight package, we can achieve increased performance over other modpacks which will allow for the use of GL shaders and high-res texture packs.

# Project Outline

## Performance

The project will probably be based on whichever version of Minecraft has the latest Forge (currently 1.11.2). Due to the lightweight nature of the project, higher-end computers should be able to make use of Optifine's GL Shader support as well as Minecraft's high-resolution texture support. For added performance, we will want to stack a few mods on top of the installation:
- Optifine
- Fastcraft
- Foamfix

## Features

### SYSTEMS

#### Villager AI

New features such will require particluar attention to chunk-handling. Villagers and their metadata may have to be handled in new ways to support AI, an example of a mod that features villager AI is "Citizens".

#### Conduits

Currently, Vanilla minecraft has no pipe, wire, or conduit system. The introduction of such a system would require some very high-level logic regarding memory handling. The proposed system would be mechanically identical to Extra Utilities pipes.

Conduits would be easily crafted from iron and glass. Special connectors (referred to as nodes in EU) would give conduits the ability to do the following:
- item connectors - pull from adjacent inventories and search for connected inventories to deposit them into
- liquid connectors - pull liquid from adjacent blocks and search for connected tanks to deposit them into
- power connectors - pull power (watts) from adjacent blocks and search for connected batteries or machines to deposit it into

Other pipes would be sorting conduits and filtering conduits. All of these would be easily craftable on a vanilla crafting table.

#### Power

New generators can be built to create power:
- Windmills (require height and adjacent air blocks)
- Waterwheels (require adjacent water source blocks)
- Engines (require fuel such as coal)
Vanilla machines can be upgraded to accept power as fuel instead of coal. New machines can also be upgraded to accept power as fuel instead of coal. Vehicles can be upgraded to accept batteries (stored power) as fuel instead of coal. Batteries and generators will be easily craftable from basic materials.

#### Enhanced Rail

Currently, rail cars that pass out of player-space have their positions stored in memory and are removed from the game. Enhanced Rail would essentially keep the rail cars in the game while they're active, loading chunks as the car passes through them. Enhanced Rail system would also have powered train engines as well as utilizing the new wrench to connect rail cars.

#### Magic

A new item called the Magic Wand will be craftable from basic materials. It will be craftable in various qualities just like minecraft tools, each higher quality having improved performance over the previouis. The magic wand will have a hotkey-triggered UI wheel where you can select any of your learned spells. Spells require durability to cast. Durability renews passively and can be fully recharged at the Arcane Altar. Magic wands do not break when depleted.

A new block called the Arcane Altar will be craftable from basic materials and is used to craft spells. Spells use special recipes requiring XP to craft.

Spells include teleportation, ranged attack, ranged disable, and ranged heal.

#### Maps

We are replacing the vanilla map with a new one using the same recipe. Maps will not be combineable, as before. Instead, they will update with new information as the player travels. While in the player's inventory, the map will display a minimap on the corner of the screen. If destroyed, the player can create a new map that will have the same information.

#### Redstone Improvements

- New advanced redstone components
- Long range redstone signals
- Custom Command Blocks

#### Roofing

Vanilla minecraft rooves are very frustrating to build. They require tedious placement of stairs and slabs and can result in player death and are an insane investment of materials

Multiblock building components would be a nice solution. 2, 3, 4, 5, and 6 block-long stairs/slabs would make long rooves much easier to build/destroy 

#### Vehicles

Currently, minecarts, mobs, and boats are the only means of transportation aside from walking. We propose the addition of several new forms of transportation. Created in a vanilla crafting bench, these can be placed in the world identically to vanilla boats. They can be mounted identically to vanilla boats. 

A new tool, the wrench, will allow players to interface with all minecraft vehicles in order to add fuel and/or activate them.

Among these new vehicles will be a balloon, specializing in up/down movement, a submarine, capable of going underwater, a powered railcar, a car or bike, a flying machine and/or hangglider. These vehicles will have limited durability and require fuel. They will be repairable on an anvil similarly to tools.

### INVENTORY

#### Inventory Sorting

In vanilla, player inventory is small and unorganized. Two very important improvements offer a simple solution to this. The first is inventory sorting. Inventory sorting would be done with a button, or several buttons, at the top of the player's inventory. It would simply group items by type and line them up.

#### Backpack

Secondly, a new slot in the player's "wearables" bar would allow for crafting and wearing a "backpack". This backpack would simply create new inventory slots for the player. The backpack could be replaced with a more advanced backpack later to create even more slots.

#### Improved Item stacking

Some items (eggs and other things) may only stack up to 16. These should only require a quick update so that they can be stacked up to 64. Some other items, chief among them tools (fishing poles, crafting benches, buckets, swords) cannot be stacked at all. These will likely be trickier to fix, but it would be nice if they were stackable as well.

#### Modified Recipes

Currently, players are forced to travel to other dimensions to craft certain recipes. I propose this not be the case. Additional recipes should be included to offer alternative ways to craft such things.

#### Added recipes

- String - Made from wool
- Horse armor - Made from armor materials

### MISCELLANEOUS

#### BLOCKS

##### Sieve

Enable players to find small items in dirt, sand, or gravel

##### Incinerator

Introducing a new functional block. Rather than introducing a "delete item button" into the UI, I propose a new block called the "incinerator" which requires fuel to burn items.

##### Liquid Tank

Stores one type of liquid.

##### Scaffold

Stackable block that can be climbed like a ladder. The whole stack can be destroyed by breaking the bottom block. The stack can be raised by building on to the bottom block.

#### ITEMS

##### Clock

Clocks will simply display a clock on the user's screen while in their inventory.

##### Hammer

Enable players to break stone into gravel, gravel into sand

##### Diving Helmet

Enable players to breath underwater, durability reduces more the deeper you go.

##### Miscellaneous food

Pork can be broken into bacon. Eggs can be cooked in a furnace. Meat and bread can make a sandich.

### WORLD

#### World-gen

- Taller trees possible
- Increase world height - build higher, dig deeper
- Harvestable water plants

#### Biomes

- Evil biome - spawns mobs during day

- Magic biome - magical plants

- Deserts - more materials available

#### New mobs

Sharks, birds, snakes, etc

#### Seasons

Leaves change color and fall.
