## Nintendo GameCube/Wii "Romhack Patches" datfiles</br>
No pre-patched ISOs are included here.</br>
This is only for the files required to create the romhack, you must supply your own totally-legal dump.</br>
### What is allowed:</br>
1. Romhack Patches (Patches that modify the core game in some form, major or minor)</br>
2. Translation Patches (Patches that translate the game or romhack from one language to another)</br>
3. Texture/Resource Packs (Enhanced or changed textures, models, sounds, etc.)</br>
4. Patch Tools (Tools required by specific patches to apply them)</br>
5. Select Hack Tools (Tools used to modify game files in some form, including saves, included at own discretion)</br>
6. NSFW Hacks (Not a common category, but a romhack nonetheless and will be included)</br>
### What is NOT allowed:</br>
1. Discriminatory/Offensive content (Definition is at own discretion, I try not to police this for the sake of preservation, but some content is too extreme to include.)</br>
2. Illegal content (Content that would be considered illegal on most sites)</br>
3. Malware (I don't scan patches, if malware is present I am not at fault. However, if notified, I will remove said content.)</br>
4. Pre-Patched ISO/RVZ/NKIT/WBFS/etc (xdeltas will be created when distributed in this manner to avoid datting/distributing copyrighted content -see below-)</br>
### Naming rules:</br>
Primarily following Redump.org naming scheme with a few key exceptions:</br>
1. Languages are omitted entirely unless absolutely necessary.</br>
2. Version listed is the version of the romhack, not the ISO required.  ## Look into dat metadata for required ISO info?</br>
3. ```<Original Game Title> ~ <Romhack Title> (Regions) (Version) (Edition/Demo)```</br>
4. Tool files get [Tool] prepended to the title to separate them from romhacks. Many romhacks require specific tools to patch properly.</br>
5. If the *full* title of the game is repeated in the romhack name, omit that repeated section.</br>
   e.g. ```Super Mario Sunshine ~ Super Mario Sunshine Arcade``` -> ```Super Mario Sunshine ~ Arcade```</br>
   5b. This rule is ignored if the romhack title comes before the main game title.</br>
      e.g. ```A Very Prideful Harvest Moon``` -> ```Harvest Moon ~ A Very Prideful Harvest Moon```</br>
6. If a symbol is added to the romhack name (e.g. +) then write out the symbol name followed by the actual symbol in parathesis.</br>
   UNLESS the symbol is not a valid symbol for filenames.</br>
   e.g. ```Paper Mario+``` -> ```Paper Mario Plus (+)```</br>
   e.g. ```Paper Mario?``` -> ```Paper Mario Question Mark```</br>
7. [Wii Specific] Romhack Patches for WiiWare titles get (WiiWare WAD) added to the name.</br>
### What files get datted?</br>
Ideally the original format of how the patches were distributed gets preserved. (Loose files dat as loose files, .zip dat as .zip, etc.)</br>
This isn't possible in a few scenarios:</br>
1. Distributed in ISO/GCM/RVZ format -> Convert to xdelta patch (see below)</br>
2. Distributed .zip/.rar/.7z is non-deterministic (hash varies each download attempt) -> Extract and hash loose files</br>
### About Custom xdeltas
Sometimes romhacks are only distributed pre-patched, in this case, I create a custom xdelta using the following steps:</br>
1. Delta Patcher (v3.1.5)</br>
2. Original File: (Original official game in ISO format)</br>
3. Modified File: (Pre-patched romhack supplied by author)</br>
4. Settings > Main Compression Level > 5 (Default)</br>
5. Secondary Compression > None</br>
6. Src Window Size > Auto</br>
7. Add Checksum to patch (Checked)</br>
This should result in a reproducible deterministic xdelta (xdeltaUI doesn't appear to be deterministic).</br>
### What determines region?</br>
Region is determined by the originating ISO region, however some regions are simplified (Europe, Australia -> Europe).</br>
Sometimes a patch is built to accomodate multiple regions, if they work on all versions (World) is applied. Tools automatically get (World) region.</br>
It's entirely possible a USA-labeled hack will work in other regions but is untested, do so at your own discretion.</br>
### Distribution:</br>
Feel free to distribute the entire or any portion of the data included in the datfiles.</br>
</br>
~ NovaAurora ~
