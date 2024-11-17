Nintendo GameCube/Wii "Romhack Patches" datfiles by NovaAurora

No pre-patched ISOs are included here.
This is only for the files required to create the romhack, you must supply your own totally-legal dump.

What is allowed:
1. Romhack Patches (Patches that modify the core game in some form, major or minor)
2. Translation Patches (Patches that translate the game or romhack from one language to another)
3. Texture/Resource Packs (Enhanced or changed textures, models, sounds, etc.)
4. Patch Tools (Tools required by specific patches to apply them)
5. Select Hack Tools (Tools used to modify game files in some form, including saves, included at own discretion)
6. NSFW Hacks (Not a common category, but a romhack nonetheless and will be included)

What is NOT allowed:
1. Discriminatory/Offensive content (Definition is at own discretion, I try not to police this for the sake of preservation, but some content is too extreme to include.)
2. Illegal content (Content that would be considered illegal on most sites)
3. Malware (I don't scan patches, if malware is present I am not at fault. However, if notified, I will remove said content.)
4. Pre-Patched ISO/RVZ/NKIT/WBFS/etc (xdeltas will be created when distributed in this manner to avoid datting/distributing copyrighted content -see below-)

Naming rules:
Primarily following Redump.org naming scheme with a few key exceptions:
1. Languages are omitted entirely unless absolutely necessary.
2. Version listed is the version of the romhack, not the ISO required.  ## Look into dat metadata for required ISO info?
3. <Original Game Title> ~ <Romhack Title> (Regions) (Version) (Edition/Demo)
4. Tool files get [Tool] prepended to the title to separate them from romhacks. Many romhacks require specific tools to patch properly.
5. If the *full* title of the game is repeated in the romhack name, omit that repeated section.
   e.g. (Super Mario Sunshine ~ Super Mario Sunshine Arcade) -> (Super Mario Sunshine ~ Arcade)
   5b. This rule is ignored if the romhack title comes before the main game title.
      e.g. (A Very Prideful Harvest Moon -> Harvest Moon ~ A Very Prideful Harvest Moon)
6. If a symbol is added to the romhack name (e.g. +) then write out the symbol name followed by the actual symbol in parathesis.
   UNLESS the symbol is not a valid symbol for filenames.
   e.g. (Paper Mario+) -> (Paper Mario Plus (+))
   e.g. (Paper Mario?) -> (Paper Mario Question Mark
7. [Wii Specific] Romhack Patches for WiiWare titles get (WiiWare WAD) added to the name.

What files get datted?
Ideally the original format of how the patches were distributed gets preserved. (Loose files dat as loose files, .zip dat as .zip, etc.)
This isn't always possible in a few scenarios:
A. Distributed in ISO/GCM/RVZ format -> Convert to xdelta patch (see below)
B. Distributed .zip/.rar/.7z is non-deterministic (hash varies each download attempt) -> Extract and hash loose files

Sometimes romhacks are only distributed pre-patched, in this case, I create a custom xdelta using the following steps:
1. Delta Patcher (v3.1.5)
2. Original File: (Original official game in ISO format)
3. Modified File: (Pre-patched romhack supplied by author)
4. Settings > Main Compression Level > 5 (Default)
5. Secondary Compression > None
6. Src Window Size > Auto
7. Add Checksum to patch (Checked)
This should result in a reproducible deterministic xdelta (xdeltaUI doesn't appear to be deterministic).

What determines region?
Region is determined by the originating ISO region, however some regions are simplified (Europe, Australia -> Europe).
Sometimes a patch is built to accomodate multiple regions, if they work on all versions (World) is applied. Tools automatically get (World) region.
It's entirely possible a USA-labeled hack will work in other regions but is untested, do so at your own discretion.

Distribution:
Feel free to distribute the entire or any portion of the data included in the datfiles.
