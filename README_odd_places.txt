Guyanonymous' Wildcards 2027: Odd Places v1.0
=============================================

File: Guyanonymous_Wildcards_2027_Odd_Places_v1.0.zip (version v1.0)
An add-on. Needs: People v1.0, Clothing v1.0 and Helpers v1.0 (the core), installed in the same wildcards folder. It needs no other add-on.

What it holds: odd places: abandoned and ruined places, curious rooms and crafts, hidden and underground places, wild nature extremes.

6,155 lists in 6 folders. None end in _prompt; the _scene lists below build a whole scene.

Top folders (lists in each):
  abandoned_ruined (959)
  curious_rooms_and_crafts (3,255)
  hidden_underground (822)
  pickers (119)
  shared_pieces (9)
  wild_nature_extremes (991)

Good first ones:
  __loc_odd_scene__
  __loc_odd_era_scene__
  __loc_odd_time_scene__
  __loc_odd_grotto_scene__
  __loc_odd_region_scene__
  __loc_odd_sawmill_scene__
  __loc_odd_tannery_scene__
  __loc_odd_dovecote_scene__

How to use a name
-----------------
Type a list's name between double underscores in your prompt, for example __loc_odd_scene__. Each time a picture is made, one line of the list is picked at random, and any names inside that line are filled in too. The catalog_odd_places.pdf in this zip lists every folder and every list name of this module; names in bold end in _prompt and are good places to start. The full guide is README_Guyanonymous_Wildcards_2027.txt (in the People zip and the release folder).

Install
-------
1. Install and switch on a wildcard extension, for example Dynamic Prompts (see below). It is not required, but it makes things easier.
2. Find the Dynamic Prompts wildcards folder: extensions\sd-dynamic-prompts\wildcards\ inside your Forge or A1111 folder, or the folder set in Dynamic Prompts' settings.
3. Unzip this zip into that wildcards folder, together with the three core zips (People, Clothing, Helpers) and any add-ons you want, all into the same folder. Each zip makes its own folder (for example odd_places\); keep its folders as they are.
4. Restart the UI so Dynamic Prompts finds the new lists.
This README file sits at the top of the zip, so it can show in Dynamic Prompts' list of wildcards as __README_odd_places__. That entry is harmless; ignore it.

Dynamic Prompts is not required, but it makes things easier
-----------------------------------------------------------
So does Guyanonymous' Prompt Studio Extension, soon at https://github.com/Guyanonymous-x/guyanonymous_prompt_studio_sdwebui_extension. Both are examples of extensions that can be used with this wildcard project.
Tested with sd-dynamic-prompts v2.17.1 in Forge Neo.
The other tested way to use these lists: Guyanonymous' Prompt Studio v3.4 (https://github.com/Guyanonymous-x/guyanonymous_prompt_studio). In it, bare names find their lists in any subfolder and the names inside picked lines are filled.
To switch Dynamic Prompts on: Extensions tab, Installed, tick sd-dynamic-prompts, then Apply and restart UI.
If it is not in your Extensions list: Extensions tab, Install from URL, paste https://github.com/adieyal/sd-dynamic-prompts and press Install; then on the Installed tab press Apply and restart UI. (Or: Available tab, Load from, find Dynamic Prompts, Install.) These install steps come from the extension's own guides and were not tested here.
Without it:
- With the basic "stable-diffusion-webui-wildcards" extension, only the first name is filled; the names inside the picked line stay in the prompt as raw __name__ text, and a list in a subfolder comes out as the bare word.
- With no wildcard extension at all, the __name__ text goes straight into the image prompt.
Switch off any other wildcard extension while you use these lists.

Why an extension helps
----------------------
The lists are plain text files; your image app does not read them by itself. A name such as __f_create_random_woman_short__ only calls a list. The add-on swaps the name for a random line from that list, and because most lines call more lists, it must keep filling those in until a whole prompt is built.

You type:  __f_create_random_woman_short__

No wildcard add-on: the model gets the raw text
  __f_create_random_woman_short__

Basic wildcards extension (stable-diffusion-webui-wildcards): only the first name is filled; the name inside it stays raw
  __f_create_random_woman_short_age25_34__

Dynamic Prompts: every name is filled, down to the last list
  A woman, 28 years old, in her late twenties, from Vietnam, has light brown skin with warm golden undertones, medium brown eyes with a slightly lighter centre and jet black dark shiny hair, styled as waist-length hair with a V-shaped cut at the back, with a center part, and has a build described as rangy build with good posture. Her face stays smooth, with only faint expression lines.

Guyanonymous' Prompt Studio: every name is filled the same way (another random pick)
  A woman, 30 years old, in her early thirties, from Germany, has tan skin with a matte look, with cool blue-pink undertones, brown-hazel eyes with a lighter inner ring and jet black dark shiny hair, styled as mid-back-length hair with long face-framing layers, slicked back and tucked behind the ears, and has a build described as thick heavy-set build. The woman's complexion is clear and taut, with bright, clear eyes.

Works with
----------
- Forge Neo with Dynamic Prompts (sd-dynamic-prompts v2.17.1): tested, works.
- Guyanonymous' Prompt Studio v3.4 (https://github.com/Guyanonymous-x/guyanonymous_prompt_studio): tested in Chrome, works. A bare __name__ finds the list in any subfolder; names inside picked lines are filled; a full path from the module folder works too (for example __people/body/nudity/irnude_prompt__). A partial path shows "Missing". When two files have the same name, it uses the first in sorted path order.
- SD.Next: its guide says bare names work in subfolders; not tested here.
- ComfyUI wildcard nodes: not tested; their guides show folder/name calls, so bare names may not be found.
- The basic "stable-diffusion-webui-wildcards" extension: does not work (see above).

Lists that call other lists
---------------------------
Many lists are templates: their lines call other lists, which can call more lists, several layers deep. If your tool does not fill nested names fully, or stops at a fixed depth, raw text such as __name__ is left in the final prompt. Check a few prompts before a big batch, and make sure your tool's wildcard depth or recursion setting is on.

Names in prompts with two or more people
----------------------------------------
Image models tend to mix up several people in one picture. So these prompts name everyone first ("The photo contains two people, Nancy and Alan."), describe each person after their name, and then use the names for place, pose and action. The names are only there to keep people apart. By default they come from a widely used pool of first names that fit each person; in faith and culture scenes people get names from their own tradition where those are known, and real historic and religious figures keep their own names.

More
----
Guyanonymous' Wildcards 2027 on GitHub, the place for every 2027 version: https://github.com/Guyanonymous-x/guyanonymous_wildcards_2027
