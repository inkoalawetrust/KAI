# Koala AI Library
This is an AI library for the [UZDoom](https://github.com/UZDoom/UZDoom) engine that allows for the (Relatively) easy creation of Doom NPCs with sophisticated AI. The library serves both the purpose of making my mods and future projects compatible with each other, and also for other modders to use. It is vaguely modelled after GMod's [VJ Base](https://github.com/DrVrej/VJ-Base) addon, e.g how it includes multiple base NPC types, the purpose of the library existing.

## Why ?
While UZDoom has the functionality to extend or replace Doom's original stupid AI, there is no simple way to go about it. And every implementation varies from mod to mod. With every modder having to reinvent the wheel for their projects.

The KAI's purpose is to allow for an easier way for modders to make intelligent NPCs in UZDoom. By coming built-in with a ton of virtual and non-virtual functions, mixins, base NPC classes to inherit new actors from, features, etc; KAI is basically a toolkit for making smarter and more competent NPCs.

Due to its' nature as library, it allows for all the basic AI code to be consolidated in one place, which also brings additional benefits, like NPCs from 2 different mods to be able to interact with each other without the need for special patches (As long as they use a single identical or at least similar enough copy of the mod).
Even mods that do not have the KAI as a dependancy can have some level of compatibility with the mod, without the mod NEEDING to be loaded alongside the library.

## FAQ
### How do I download it?
There's two ways to download the library, the first and easiest one is to download one of the [releases](https://github.com/inkoalawetrust/KAI/releases) of the library, which are stable and generally what you'd likely want to use, especially if you intend for your monsters to still be usable with other people's KAI mods. It's easier to keep track of numbered releases than individual commits after all.

The second way is to get one of the latest commit versions, which you can do by clicking on the green "<> Code" button, selecting the Local tab, and clicking Download ZIP, and unpacking and using that. If you plan to merge the non-release codebase to your mod, just keep in mind to remove any unnecessary cruft like the Git directory and files, and the GitHub wiki file directory. Also, since this is obviously a dev commit build in this case, keep in mind that there might be unfinished, half baked code, or debug console messages and objects appearing that need manual removing.
### I've downloaded the mod but all the monsters are still stupid, what do I do?
KAI is a library for other modders to use in order to make custom monsters, it's not a gameplay mod that does anything on its' own.

## Documentation
The wiki for the library can be found [here](https://github.com/inkoalawetrust/KAI/wiki/), containing information on classes, functions, variables, and other code structures, along with guides in the future.

## Usage
For the time being, you can check for info on how to use the library [here](https://github.com/inkoalawetrust/KAI/wiki/Mod-interoperability), as I have not yet begun writing guides for it.

But generally, I'd recommend using the latest stock version (This repositories' master branch) like I do for my own mods that use it, for maximum compatibility with other KAI-based mods. However, you can still make your own version of the library and directly merge it to your project, like how most UZDoom libraries are used for some reason.

## The present
Currently, the library is still in early alpha, so a lot of it is subject to change as I add new features, remove unnecessary/bad code, and just generally update the codebase over time. A lot of features that I'll probably add in the future are still missing, such as optional momentum-based movement for ground NPCs, a passenger system for vehicle NPCs, locational damage, [general integration of UZDoom's behavior system once that makes it into a release build](https://zdoom.org/w/index.php?title=Classes:Behavior), and so on.