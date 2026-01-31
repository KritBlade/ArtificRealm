# ArtificRealm
SillyTavern Character Card - license GPL 3.0, NOT for commerical use.


--------- Regular player -------------

I am releasing the MVU Zod Character card Artific Realm (アーティフィック レルム 創世域). Installation video guide here https://youtu.be/whRF0pJAzvs

The game character card is here to download at https://github.com/KritBlade/ArtificRealm/tree/main/CharacterCard  You are required to follow the youtube video above to do the installation of an extension or it won't work. PC for playing is recommended due to the large interface.

This character card is a iSeikai world which have magic, dwarf, elf, demon , fairy..etc. A powerful suction drag you 'the main char' into this world. As you arrived the world, you were supercharged with four ex-plugins [Soul Covenant], [Inventory], [System Panel], and [Phoenix Pact].

[Soul Covenant] - Can bind female characters as Familiars

[Inventory] - A four-dimensional space that can store any small non-living objects, such as items, clothes, food, etc.

[System Panel] - An RPG game-like display panel, visible only to the main character. It shows the target's basic stats as well as surface and hidden personality traits

[Phoenix Pact] - The player can actively record the current point in time as a "Save Point".

When you wake up inside a damaged wooden hut, a nun called Engni was staring at you nervously……

This is a NSFW game. Unlike all other RPG NSFW game, the personality of all the Heroine inside the game have serious flaws in their personality. Aka...bitches one way or the other. You as the main character would need to know their personality flaws and use it as your advantage to survive in the iseikai world. Bitches can be deadly towards enemy if you use it the right way.

You will need to takes 6 minutes to do the installation of extension correctly for SillyTavern in order to get it to work. I assume you have already have a working connection to AI service provider, so installation won't cover the standard installation of SillyTavern. This card heavily utilize the extension Tarven Helper so that it will enable javascript in the SillyTavern engine, which will allow you to have persistent data in your story. That means every single stats in the status menu you see is persistent locally in your harddrive. AI do NOT need to remember these stats or need to remember it's state.

You will need some decent AI to pull this off. My testing platform was on Gemini Flash 3.0 preview. I know Gemini 2.5 and 3.0 pro works, Claude most model works as well. Kimi 2.5 *can* work, but the thought time take ages to finish. Deepseek 3.2? I can't get that not to show the <think> process. For all other lower end model, it might or might not getting the stats update correctly.

Since the game is required to use a preset that works with Tavern Helper, most of the preset in the Western world wouldn't get the stats update in chat correctly, you will have to download a preset that works with Tavern Helper. There is one I found that have some English translation can be downloaded Izumi preset from https://discord.gg/C6HabNwzn7 inside a discord channel as you see in the installation video. You will need to patch 2 places as you saw in the video so that it works correctly in English.

In case you have a hard time to get the Izumi preset, I found that Megumin Preset here at reddit works OK, although not optimal, but it works. You will have to read the post below to setup the preset (including the first comment by the OP) https://www.reddit.com/r/SillyTavernAI/comments/1q2bwdp/megumins_secret_sauce_gemini_v15_3_and_25/

Once you get into the game/chat, you can view the storage of the stats in JSON format at the red arrow https://i.vgy.me/zoLtSs.jpg , and you can view every single floor of the chat at this tab https://i.vgy.me/G9kcUQ.jpg . You can modify the stat right here if you need to. The blue arrow would allow you to see the prompt that will be sent to AI for preset builder.

This game is far from polished, but it serve as a showcase what the extension can be done. I believe Tavern Helper would have a English version soon as I saw they are doing translation on Github.

-------------------------------------------

I have to give credit to where it's due. It is loosely based on another card "The Fallen Psalms of Terrarien" which I hack the hell out of this card and only leaving the world lore in place. Character design is coming from another card called "Building a Harem in an Otherworld Full of Villainous Bitches" which most of the characters idea is based on this card. The lorebook was huge in "The Fallen Psalms of Terrarien" so I decided to keep it as is and translate that into English. The most difficult part of this project was to do the translation while keep the name consistent. No, you will still see AI translation issue here or there...but that's too big of a effort to get all of them right.

Since the game is required to use a preset that works with Tavern Helper, most of the preset in the Western world wouldn't get the stats update in chat correctly, and I hope eventually someone here will build a preset that works with Tavern helper. During the mean time, I found one preset that have "kind of" English translation that at least you can read the title. You can download this preset from https://discord.gg/C6HabNwzn7 inside a discord channel. I am not the owner of the preset and I was told that people will have to get into discord to download the preset. I can't redistribute the preset, the preset is called Izumi Preset.

--------- Preset Builder -------------

As you can see in the video, player are required to download a preset so that it will work correctly with MVU variable update. I am not a preset builder. I hope someone here will eventually make a preset that works with Tavern Helper with MVU Zod support. The main issue of making a preset for Tavern Helper is not adding how many bells and whistles in your preset, it's how much you can SQUEEZE minimum required features while keeping the output token small. You can check out Izume preset here https://discord.gg/C6HabNwzn7, which I know it works well. The preset comes with quest number generator on main quest and side quest , which is super friendly for JSONpatch add into MVU variable. It also feature the MVU update structure

<UpdateVariable>

<Analysis>

</Analysis>

<JSONPatch>

</JSONPatch>

</UpdateVariable>

Since this is a Chinese preset so it doesn't work quite well with English thought as well as Jailbreak on English story. I provided two patches on thoughts and jailbreak from

https://github.com/KritBlade/ArtificRealm/blob/main/PresetPatch/chain_of_thought.txt

https://github.com/KritBlade/ArtificRealm/blob/main/PresetPatch/jailbreak.txt

which you can see where to patch in the video

https://youtu.be/whRF0pJAzvs.

--------- Game Card builder -------------

You can hack the hell out of this card as you like, you just need to give a reference your card is based on https://github.com/KritBlade/ArtificRealm and it's all I am asking for.

For beginners, you can just delete any entry after lorebook entry "-------------- Your lorebook start here -------------- ", just keep one entry "Heroine" and one entry "Bluewatch". You can duplicate these two entries for characters and lores. You can pretty much build your own game here. Anything before "-------------- Your lorebook start here -------------- ", it's the logic of the game, unless you need to change how the logic works, you shouldn't need to touch this part. Feel free to amend those if you know what you are doing. <Attribute_system>, <monster_guide>, <Battle_system>, <healing_guide> and <progression_system> goes hand to hand with each other, so if you modify any one of those, make sure the number works out correctly for the other tag.

For intermediate creator, since the card use javascript, you can check out how lorebook is used. The end of lorebook entry "Resources" have some resources that teach you how to use INSIDE World info lorebook.

For Advance creator, the status menu you can see the code from Regex StatusMenu. Pay attention to function updateVariablesWith which can be used to save MVU variable, and function getCurrentCharPrimaryLorebook and getLorebookEntries for retrieving data from World Info lorebook. The code of status menu by no mean is good, I just use Antigravity to hack it. I know I can separate the logic and presentation into two layer, but that will make it really difficult for new coder to Tavern Helper to know what the heck is going on. So, I just keep that simple in one single file. Moreover, there is a schema under Tavern helper third tab called "schema", which will govern what data can be written into MVU variable. There is a bunch of regex under scope you can turn on or off to enable or disable battle raw data, update JSONpatch command..etc.

Tavern helper github https://github.com/N0VI028/JS-Slash-Runner

ST Prompt template source code https://codeberg.org/zonde306/ST-Prompt-Template/

ps. Tavern Helper is *the* default installation extension for the Chinese SillyTavern commnuity, we are talking about hundred of thousand of users have this installed by default.