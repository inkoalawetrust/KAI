# Koala AI Library
This is an AI library for the [GZDoom](https://github.com/ZDoom/gzdoom) engine that allows for the (Relatively) easy creation of Doom NPCs with sophisticated AI. Mostly meant to be used by me (inkoalawetrust) for interoperability on my own projects.

## Why ?
While GZDoom has the functionality to extend or replace Doom's original stupid AI. There is no simple way to go about it. And every implementation varies from mod to mod. With every modder having to reinvent the wheel for their projects.

The KAI's purpose is to allow for an easier way for modders to make intelligent NPCs in GZDoom. By coming built-in with a variety of virtual and non-virtual functions, mixins, and base NPC classes to inherit new actors from.
Due to its' nature as library. It allows for all the basic AI code to be consolidated in one place. Which also brings additional benefits, like NPCs from 2 different mods to be able to interact with each other without the need for special patches.

## Usage
The recommended way to use this mod/library is as a dependancy for your mods. So it is adviced to NOT SIMPLY COPY THE LIBRARY INTO YOUR MOD. Instead, it should be loaded alongside your mod, and any other mods that use this library for their NPCs.

![](https://cdn.discordapp.com/attachments/762804188807168010/1094310075507691582/Library_Usage.png)

The reason for this is to prevent any potential conflicts between different bespoke versions of the library used by different mods. However you are still free to merge the library to your project if you want, in exchange for having to rename most methods and classes to avoid conflicts, and potentially losing interoperability.

## The present
As of the time of this writing (8/4/2023) the library is incredibly barebones, my current goal is to first import most of the base code from my [Military Vehicles Pack mod](https://github.com/inkoalawetrust/Military-Vehicles-Pack) into the library. To serve as the vehicle base. More base NPC types will be added in the future. The base humanoid/creature NPC will not be added until I begin rewriting [my Smart Marine mod](https://github.com/inkoalawetrust/Smart-Marines).

Still very much a work in progress, so most of what you see is subject to change.
