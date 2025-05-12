## Dimensions:
### Vanilla
- Overworld
- The Nether
- The End
### Modded
- The Bumblezone
- Deeper & Darker
- Eternal Starlight
- The Twilight Forest
### Special Purpose
- AE2 Spatial Storage
- Compact Machines
- Void Dimension (Search `@JAVD`)
- Mining Dimensions (Search `@JAMD`)

<hr/>

To craft the **Celestigem/Eclipse Alloy Paxel** from the mod *Just Dire Things* you need to place all three of the main celestigem/eclipse alloy tools (pickaxe, axe, shovel) into the smithing table to combine them.

The reason the recipe doesn't show is due to EMI being unable to translate the recipe from JEI![.](https://innx.dev/images/paxel.webp)

<hr/>

Pressing `u` toggles your FTB Team chat. If all you see is the following, you must have accidentally pressed it and can press it again to bring you back to global chat![.](https://innx.dev/images/team.png)

<hr/>

## Logs, please?
_Your log file can be very helpful in diagnosing what’s gone wrong._
### Where are my logs, you ask? Well..

__Go to your modpack's folder__. There should be an `Open Folder` button, or similar, in your launcher.

1. Look for:
  - an `hs_err_pid-----.log`, _or_…
  - the newest file in the `crash-reports` folder, _and/or_…
  - `logs/latest.log`.

2. Please upload it (or them) to [MC Logs](https://mclo.gs/).
3. Copy the link (or links) to the report(s) and paste here.

<hr/>

## Trying to Verify?
First, read [#whitelisting](https://discord.com/channels/570630340075454474/726536593136943204) in it's entirety. By whitelisting yourself to one of our servers, you agree to the rules.
Next, head over to one of the server channels. ([#craftoria-eu](https://discord.com/channels/570630340075454474/1254490870808318087), [#craftoria-eu2](https://discord.com/channels/570630340075454474/1292199371848552548), [#craftoria-na](https://discord.com/channels/570630340075454474/1282263854922862632))
Lastly, use the command `/verify` followed by the code you obtain when attempting to join the server for the first time.

*If* you verify yourself, yet you are still unable to join the server, use the command `/unverify`, then retry the verification.
*If* Discord is not recognizing your `/verify` command, try **disabling** this setting in Discord:
`Settings` -> `Accessability` -> __`Use the legacy chat input.`__

For the non-Craftoria servers, simply use what is stated in [#whitelisting](https://discord.com/channels/570630340075454474/726536593136943204).

<hr/>

## Verify Failing?

Try un-verifying and re-verifying again. Sometimes the bot can fail to properly verify your code.
Use `/unverify` before doing your verification process over again, just as you did the first time.

*If* Discord is not recognizing your `/verify` command, try **disabling** this setting in Discord:
`Settings` -> `Accessability` -> __`Use the legacy chat input.`__

The website `craftoria.net` is **not** owned or run by us and we do not affiliate with it. It was created by an unknown entity without permission and contains a *lot* of false information about the modpack.

<hr/>

The *direct* power conversion rate between all the different types is the following:

1 E/t  : 1 LF/t :  1 FE/t : 1🗲/t : 1 EU/t : 2 AE/t : 2.5 J/t

Specifically for the pack **Craftoria**, using the *Flux Transformer* you can convert EU to FE in the conversion 1 EU/t : 50 FE/t one way. Connecting the EU Cable *directly* into anything run by FE will be a 1 EU/t : 10 FE/t.

<hr/>

The Essential Mod is known to cause incompatibilities with mods in the pack (possibly due to the requirement of Sinytra Connector) and is full of bloat and microtransactions. The mod is also closed source, so no one exactly knows what's going on under the hood.

Our recommended mod for self hosting servers *without* the need for port forwarding is [e4mc](<https://modrinth.com/mod/e4mc>). With this mod, your "Open to Lan" button becomes a "Start Server" button and is only needed to be installed on the side that becomes the host. It's simple, safe, and performant.

<hr/>

## Adoptium (AdoptOpenJDK)
For Craftoria and AOF7:
[Java 21](https://adoptium.net/?variant=openjdk21&jvmVariant=hotspott) for Minecraft 1.20.5 and later

For AOF7, AOF6, AOF5:
[Java 17](https://adoptium.net/?variant=openjdk17&jvmVariant=hotspot) for Minecraft 1.17 to 1.20.4

<hr/>

# High-Pressure Steam Loop![:](https://innx.dev/images/HP_steam_setup.png)

<hr/>

To host your own server locally, proceed to the [Craftoria Curseforge](<https://www.curseforge.com/minecraft/modpacks/craftoria/files/all?page=1&pageSize=20&version=1.21.1&gameVersionTypeId=6>) page and look for the latest version in the files. Press *Additional Files* to find the **Server Files**.

Press download and you should obtain a `.zip` file, also known as an "archive." Extract this into the folder you would like to host your server from. This `.zip` file does *not* have the mods included in it from the get go, this is to cut down on unnecessary direct file sizes.

Next, ensure you have [Java 21](<https://adoptium.net/?variant=openjdk21&jvmVariant=hotspott>) installed, as you'll need it to run servers (and clients) from Minecraft version 1.20.5 and up.

Then, navigate back to the folder you extracted the files to and run the `startserver.bat` if you are on windows, or `startserver.sh` if you are on Linux or Mac (both are Unix based). This will begin to download all the required mods, config, and everything else required. After, you'll be prompted to accept the EULA, which you can do right in the terminal by following the instructions it provides. After which you have accepted, the world will begin to load up and generate (this may take a considerable amount of time, depending on your hardware).

<hr/>

Ensure you're using optimal Java arguments depending on how much RAM you allocate.

If you're allocating 6GB or more, use `-XX:+UseZGC -XX:+ZGenerational`
If you're allocating less than 6GB, use `-XX:+UseG1GC`

<hr/>

The *Apotheosis* mod has a mechanic called "World Tiers." Using the default keybind (**Ctrl+T**) you can access the GUI which shows the tiers and what each entails on top of a pretty background.

Check the advancement (default keybind: **L**) tab labeled "Apothic World Tiers" to find out what you need to do to unlock the next world tier.

Each world tier unlocks the ability for higher tier mob bosses to spawn and thus unlocks the ability to obtain higher tier apothic gear traits.

<hr/>

To find the items in the blacklist for both the Replicator Mk1 and the Replicator, search the following for the two blacklists in EMI respectively:

- #replicator_blacklist for Replicator
- #replicator_1_blacklist for Mk1 Replicator

<hr/>

Run a Spark client profiler for 30 seconds while doing the action that causes the lowered client performance. Use the following command (with or without OP)

`/sparkc profiler start --timeout 30`

Send the resulting URL it gives you once it finishes.

<hr/>

## Want to learn about EMI?
**EMI**, or as we like to call it, your *Evolving Manufacturing Index*, is a browser that contains every single material, tool, block, resource, and fluid in this world. It gives you knowledge on how to craft everything and it will even show you how many resources it takes to craft something by pressing on the little tree icon next to the product lost of the recipe.

When in your inventory, on the right is your main browser. On your left will be your bookmarks.

### Let's go over some actions.
- To find the recipe of an item, anywhere in a GUI, hover over it with your mouse and press the letter **R** on your keyboard. If you hover over the item *in* the recipe browser itself, you can simply **Left-Click** on it.
- To find the uses of an item, anywhere in a GUI, hover over it with your mouse and press the letter **U** on your keyboard. If you hover over the item *in* the recipe browser itself, you can simply **Right-Click** on it.
- To bookmark the item, hover over it in any GUI, and press the letter **A** on your keyboard.
- To bookmark a recipe, be in the window that shows a recipe, hover over the recipe (but *not* on a specific ingredient) and press the letter **A** on your keyboard.
- To un-bookmark an item/recipe, hover over the item/recipe in your bookmark section and press the letter **A**.
- To view a recipe tree that includes the total amount of resources to craft that item, press on the button that looks like the `T` shape from the hit game *Tetris*, usually to the right of the output slot in a recipe.
- To favorite a recipe and ensure your EMI views it as the default, press on the `❤` button usually to the right of the output slot in a recipe.
- To auto-fill a recipe into a workstation, open a valid workstation, open the recipe in your EMI, then press the `+` button, usually to the right of the output slot in a recipe.

<hr/>

## How much memory should you allocate?
We recommend `6GB-8GB` allocation on most computers built within the last 6-ish years.
For older computers, similar allocation may work, but you must ensure your video settings in game are lowered considerably.

### For the following allocation amounts, use the proper Java arguments for optimal performance:
If you're allocating 6GB or more, use `-XX:+UseZGC -XX:+ZGenerational`
If you're allocating less than 6GB, use `-XX:+UseG1GC`

<hr/>

## Connection lost when joining a server? Something about "channels" and "missing mods"?
Normally, when you get this message, you should see two boxes of orange text. One talks about the "Channel Name" and the other a "Reason." For 99.9% of cases, this purely means that the version of the modpack you are on does *not* align with the version of the modpack the server is running.

- For the public servers, the version says on the server's MOTD (the message on the server, in the multiplayer list). It also states it in the channel topic for the specific server.
- For other servers ensure that you are on the right version and that the server host has not modified the pack in any meaningful way.
- For your own self-hosted server, ensure that you are on a matching version. If that is checked, a possibility could be a failed server install. Sometimes Windows Firewall/Defender can deny downloads with seemingly no reason. Ensure your firewall/defender is not blocking some of these downloads.

<hr/>

## Modded Server lagging?
Your ping may be fine. Your computer may be fine as well. But that doesn't necessary mean the server *isn't* fine. You must remember that Minecraft isn't exactly optimized with heavy modification in mind, especially when it comes to hosting a modified version of Minecraft to many people.
A lower TPS (Ticks Per Second) is very common. 20 TPS is the most fluid a server can be, but you will rarely see that, especially if a server has a lot going on in the world.
From someone who has played on modded servers with TPS dipping into, and below, 5 TPS: It takes some getting used to, but it's definitely playable.

Although, sometimes, it stays *very* low for little apparent reason, such as low (or one) player count(s), newer server, etc. This could be a bug, but most of the time, it isn't.

<hr/>

## Want to force load chunks?
There's really only two ways to do it. Either use a vanilla chunk loader (yes it exists, look it up) or use FTBChunks!

- For FTBChunks, open your inventory and locate the map looking button with a beige border in the top left corner of your screen labeled "FTB Chunks: Claim Manager" and click on it.
- To claim a chunk, **Right-Click** or **Right-Click + Hold-Down** on the chunk(s) you wish to claim. You must claim before you can force load. Do the same with the **Left-Click** to un-claim.
- To force load a chunk, **Shift + Right-Click** or **Shift + Right-Click + Hold-Down** on the *claimed* chunk(s) you wish to force load. Do the same with **Left-Click** to un-force load.
- Keep in mind the number of claimed chunks and force load chunks are limited and display at the bottom of your chunk manager screen.

<hr/>

## Have *power* on a server and want to adjust values such as max claim/force-load chunks, homes, and more?
You'll need to use the power of commands for this one.
### For Chunk related things, use the following command and node permissions:
`/ftbranks node add member <node> <value>`
- `ftbchunks.max_claimed` This uses an integer for `<value>`
- `ftbchunks.max_force_loaded` This uses an integer for `<value>`
- `ftbchunks.chunk_load_offline` This uses a boolean (`true` or `false`) for `<value>` **This permission is highly recommended you remain false to prevent excessive lag.**

### For Home and Teleportation related things, use the following command and node permissions:
`/ftbranks node add member <node> <value>`
- `ftbessentials.home.max` This uses an integer for `<value>`
- `ftbessentials.back.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.spawn.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.home.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.tpa.cooldown` This uses an integer (seconds) for `<value>`
- `ftbessentials.rtp.cooldown` This uses an integer (seconds) for `<value>`

## Quest have a *gray* question mark and cannot be completed, even though all dependencies have been finished?
This is a common bug with the mod FTBQuests. In the latest versions, we've disabled the ability to "finish" a quest before it's unlocked to prevent this issue, but if you've already pre-competed a quest, you might need to forcefully complete (or reset) the quest using level 2 Operator commands.

If you have the ability to do so, enter your FTBQuests screen, locate the quest you'd like to reset, enter "Edit Mode" by pressing on the pencil button in the bottom right corner of the screen, then **Right-Click** on the desired quest, and press **Reset Progress**.
If you need to reset the progress of someone else's quest, enter your FTBQuests screen, locate the quest you'd like to reset, enter "Edit Mode" by pressing on the pencil button in the bottom right corner of the screen, then **Right-Click** on the desired quest, and press **Copy ID**. Then run the command: `/ftbquests change_progress <IGN> reset <Quest ID>`
