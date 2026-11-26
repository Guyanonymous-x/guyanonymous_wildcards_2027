Guyanonymous' Wildcards 2027: Medical Graphic v1.0   18+ / NSFW
===============================================================

18+ / NSFW. This module holds explicit adult content. For adults only.

File: Guyanonymous_Wildcards_2027_Medical_Graphic_v1.0.zip (version v1.0)
An add-on. Needs: People v1.0, Clothing v1.0 and Helpers v1.0 (the core), installed in the same wildcards folder. It needs no other add-on.

What it holds: medical scenes above PG-13: intimate clinical exams (pelvic, Pap, breast, mammogram, prostate, rectal, testicular), surgery in progress, and all of childbirth: labour scenes at levels 1 to 4 and the full-term birth at levels 1 to 6.

1,135 lists in 9 folders. 117 of them end in _prompt: each of those builds a whole prompt.

Top folders (lists in each):
  childbirth (539)
  death_and_autopsy (2)
  intimate_exams (212)
  pickers (7)
  shared_pieces (118)
  surgery_in_progress (257)

Some folders, in plain words:
  intimate_exams: clinical exams of the intimate parts of the body: pelvic and Pap exams, breast exams and mammograms, prostate, rectal and testicular exams. Genitals or bare breasts are shown, in a clinic setting.
  surgery_in_progress: operations under way: open cuts, flowing blood, surgical tools in use, and the operating room team at work.
  death_and_autopsy: the dead: a body in a mortuary viewing room, a blanket covering it to the chest.
  childbirth: all of childbirth, kept apart, with its own levels, 1 the mildest. Start with __birth_prompt__.
  full_term: whole birth scenes at full term, step by step: active labour, pushing, the birth, tears and stitching.
  labour_and_helpers: the person in labour and the people helping, including labour at home.
  unclothed: the bare body of the person giving birth, by age and build.
  after_birth: the moments right after the birth.
  pickers: lists that pick one scene or piece from the folders above (their names start with graphic_).
  shared_pieces: medical lists the scenes here call, the same as in the Medical module.

Good first ones:
  __birth_prompt__
  __birth_l1_prompt__
  __birth_l2_prompt__
  __birth_l3_prompt__
  __birth_l4_prompt__
  __birth_full_prompt__
  __birth_full_l1_prompt__
  __birth_full_l2_prompt__

How to use a name
-----------------
Type a list's name between double underscores in your prompt, for example __birth_prompt__. Each time a picture is made, one line of the list is picked at random, and any names inside that line are filled in too. The catalog_medical_graphic.pdf in this zip lists every folder and every list name of this module; names in bold end in _prompt and are good places to start. The full guide is README_Guyanonymous_Wildcards_2027.txt (in the People zip and the release folder).

Install
-------
1. Install and switch on the Dynamic Prompts extension (see below). It is required.
2. Find the Dynamic Prompts wildcards folder: extensions\sd-dynamic-prompts\wildcards\ inside your Forge or A1111 folder, or the folder set in Dynamic Prompts' settings.
3. Unzip this zip into that wildcards folder, together with the three core zips (People, Clothing, Helpers) and any add-ons you want, all into the same folder. Each zip makes its own folder (for example medical_graphic\); keep its folders as they are.
4. Restart the UI so Dynamic Prompts finds the new lists.
This README file sits at the top of the zip, so it can show in Dynamic Prompts' list of wildcards as __README_medical_graphic__. That entry is harmless; ignore it.

Dynamic Prompts is required
---------------------------
Tested with sd-dynamic-prompts v2.17.1 in Forge Neo.
The other tested way to use these lists: Guyanonymous' Prompt Studio v3.4 (https://github.com/Guyanonymous-x/guyanonymous_prompt_studio). In it, bare names find their lists in any subfolder and the names inside picked lines are filled.
To switch Dynamic Prompts on: Extensions tab, Installed, tick sd-dynamic-prompts, then Apply and restart UI.
If it is not in your Extensions list: Extensions tab, Install from URL, paste https://github.com/adieyal/sd-dynamic-prompts and press Install; then on the Installed tab press Apply and restart UI. (Or: Available tab, Load from, find Dynamic Prompts, Install.) These install steps come from the extension's own guides and were not tested here.
Without it:
- With the basic "stable-diffusion-webui-wildcards" extension, only the first name is filled; the names inside the picked line stay in the prompt as raw __name__ text, and a list in a subfolder comes out as the bare word.
- With no wildcard extension at all, the __name__ text goes straight into the image prompt.
Switch off any other wildcard extension while you use these lists.

Why it is needed
----------------
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
