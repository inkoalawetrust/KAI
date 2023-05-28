# Koala AI Library
This is an AI library for the [GZDoom](https://github.com/ZDoom/gzdoom) engine that allows for the (Relatively) easy creation of Doom NPCs with sophisticated AI. The library serves both the purpose of making my mods compatible with each other, and also for other modders to use. It is vaguely modelled after GMod's [VJ Base](https://github.com/DrVrej/VJ-Base) addon, e.g how it includes multiple base NPC types.

## Why ?
While GZDoom has the functionality to extend or replace Doom's original stupid AI, there is no simple way to go about it. And every implementation varies from mod to mod. With every modder having to reinvent the wheel for their projects.

The KAI's purpose is to allow for an easier way for modders to make intelligent NPCs in GZDoom. By coming built-in with a variety of virtual and non-virtual functions, mixins, and base NPC classes to inherit new actors from.
Due to its' nature as library. It allows for all the basic AI code to be consolidated in one place. Which also brings additional benefits, like NPCs from 2 different mods to be able to interact with each other without the need for special patches.
Even mods that do not have the KAI as a dependancy can have some level of compatibility with the mod, without the mod NEEDING to be loaded alongside the library.

## Documentation
The wiki for the library can be found [here](https://github.com/inkoalawetrust/KAI/wiki/), containing information on classes, functions, variables, and other code structures, along with guides in the future.

## Usage
For the time being, you can check for info on how to use the library [here](https://github.com/inkoalawetrust/KAI/wiki/Mod-interoperability), as I have not yet begun writing guides for it.

But generally, I'd recommend using the latest stock version (This repositories' master branch) like I do for my own mods that use it, for maximum compatibility with other KAI-based mods. However, you can still make your own version of the library and directly merge it to your project, like how most GZDoom libraries are used for some reason.

## The present
Currently, the library is still in very early alpha, and is still massively biased towards just containing code for vehicle NPCs, since it's based on the codebase of my [Military Vehicles Pack mod](https://github.com/inkoalawetrust/Military-Vehicles-Pack), which as of the time of this writing (28/5/2023) is still the mod I'm focusing development on.

More base NPC types will be added in the future. The base humanoid/creature NPC in particular will not be added until I begin rewriting [my Smart Marine mod](https://github.com/inkoalawetrust/Smart-Marines).

Still very much a work in progress, so most of what you see is subject to change.
