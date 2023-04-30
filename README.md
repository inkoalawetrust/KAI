# Koala AI Library
This is an AI library for the [GZDoom](https://github.com/ZDoom/gzdoom) engine that allows for the (Relatively) easy creation of Doom NPCs with sophisticated AI. The library serves both the purpose of making my mods compatible with each other, and also for other modders to use. It is vaguely modelled after GMod's [VJ Base](https://github.com/DrVrej/VJ-Base) addon, e.g how it includes multiple base NPC types.

## Why ?
While GZDoom has the functionality to extend or replace Doom's original stupid AI, there is no simple way to go about it. And every implementation varies from mod to mod. With every modder having to reinvent the wheel for their projects.

The KAI's purpose is to allow for an easier way for modders to make intelligent NPCs in GZDoom. By coming built-in with a variety of virtual and non-virtual functions, mixins, and base NPC classes to inherit new actors from.
Due to its' nature as library. It allows for all the basic AI code to be consolidated in one place. Which also brings additional benefits, like NPCs from 2 different mods to be able to interact with each other without the need for special patches.
Even mods that do not have the KAI as a dependancy can have some level of compatibility with the mod, without the mod NEEDING to be loaded alongside the library.

## Usage
The recommended way to use this mod/library is as a dependancy for your mods. NOT SIMPLY COPY THE LIBRARY INTO YOUR MOD. Instead, it should be loaded alongside your mod, and any other mods that use this library for their NPCs.

![](https://cdn.discordapp.com/attachments/762804188807168010/1094310075507691582/Library_Usage.png)

The reason for this is to prevent any potential conflicts between different bespoke versions of the library used by different mods.
That being said, you can still merge the library into your project like most GZDoom libraries if you really want, even if it may break compatibility with other mods. Such as if you are making a total conversion, full mapset, or a full game.

## The present
As of the time of this writing (25/4/2023) the library is effectively in pre-alpha, it still mostly consists of code I imported from my [Military Vehicles Pack mod](https://github.com/inkoalawetrust/Military-Vehicles-Pack), and is riddled with debug messages and actors.
A lot of that code serves as the vehicle base (Of course). But a good chunk of the former MVP code (Functions, virtuals, variables etc) has been backported to KAI_Actor as generic actor code, along with addition of some new features like new generic checks, and a generic threat level system. I have not even decided on a license yet.

More base NPC types will be added in the future. The base humanoid/creature NPC will not be added until I begin rewriting [my Smart Marine mod](https://github.com/inkoalawetrust/Smart-Marines). As of right now it'

The code is currently undocumented outside of comments in the code itself, at some point hopefully soon, I will write a GitHub wiki with proper documentation for classes, functions, variables, and guides on those code structures, along with examples. First however, I need to figure out how to write a GitHub wiki.

Still very much a work in progress, so most of what you see is subject to change.
