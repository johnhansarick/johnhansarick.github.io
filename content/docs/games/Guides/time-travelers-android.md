---
title: Time Travelers English Translation for Android
linkTitle: Time Travelers Android
description:
    - How to setup Time Travelers to work on 3DS Emulators for Android
---
The game [Time Travelers](https://thegamesdb.net/game.php?id=78374) is a sort of visual novel choice driven game.  Honestly I haven't played more than 10 minutes just to get it running, but after the effort I have down the proper steps that work with Azahar, Azahar Plus, and Citra for **Android**.  As of this writing thats:

* Azahar Plus build 204fde666
* Azahar 2123.3
* Citra 988f294

I've tested this out with my Ayn Thor 2025 model (in case there's another model in the future), running Android 13.

## Steps

1. Go to [Fan Translators International](https://fantranslators.info/) and follow their instructions.
   1. Clearly you're going to do this with a person copy of Time Travelers that you've dumped yourself rom your own legally owned version.
2. When you are done, you will have a folder `000400000008C600`.
3. Make sure your `Time Travelers.3ds` or `Time Travelers.cci` file is in your Nintendo 3DS ROM directory.  For example:  `/storage/emulated/0/Roms/roms/n3ds`.
4. The next step will depend on what emulator you're using.
   1. **Azahar and Azahar-Plus**, you would have set the user folder, for example:  `/storage/emulated/0/Documents/azahar`.
   2. **Citra**, it's automatically set to `/storage/emulated/0/citra-emu`.
5. If using **Azahar** or **Azahar Plus**, go to **Settings -> Thor settings -> Is it force start selinux**.  For some reason, this isn't required with Citra.
   1. Personal note:  This step drove me crazy until I figured out this was required.  I don't know what this setting is for, so use with caution.
6. For whichever emulator, follow these steps:
   1. For the emulator of choice, go to the user folder.  There are two folders you either need to create or look for:
      1. `load/mods`
      2. `sdmc/luma/titles`
   2. Copy the *entire `000400000008C600` file into **both** of the folders above.  I don't know why you need it in both, but it doesn't work otherwise.
      So by the end you'll have:

      1. `load/mods/000400000008C600`
      2. `sdmc/luma/titles/000400000008C600`
7. Launch the game.  At this point, you'll see the Time Travelers image file:

    {{<figure src="/images/games/time_travelers/time-travelers-start.png" width="800">}}

That should do it!
