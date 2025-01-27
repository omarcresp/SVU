This is a guide to the player config options in the config.json file. Feel free to contact me with any questions not answered here.

The "Relationship Type" category specifies your relationship with each marriage candidate as "FullyPlatonic," "RomanceWithoutSex," "SexWithoutRomance," or "RomanceAndSex." 
	By default, all vanilla marriage candidates are set to FullyPlatonic. Currently, only vanilla characters are supported.
        If a character is set to FullyPlatonic or SexWithoutRomance, their romantic dialogue and heart events will be patched with platonic rewrites, and marriage will be replaced with platonic partnership (with customizable relationship label and term of endearment). This also enables moving them onto your farm with the Friendship Bracelet as an alternative to the Mermaid's Pendant.
	If a character is set to FullyPlatonic or RomanceWithoutSex, their partnership (FullyPlatonic) or marriage (RomanceWithoutSex) dialogue is edited to remove sexual implications. Penny's and Sam's 10-heart events are also slightly edited if they are set to one of these options.
	FullyPlatonic is the best choice for friendships and aromantic asexual partnerships. RomanceWithoutSex is the best choice for asexual marriages. SexWithoutRomance is the best choice for "friends with benefits"-style partnerships. RomanceAndSex is the best choice for NPCs that you want to exempt from all platonic edits (e.g., NPCs with whom you want a vanilla dating relationship or marriage).
        Switching a character's relationship type may cause continuity errors in their story arc, but shouldn't cause any mechanical bugs. 
        If you have downloaded another mod's compatibility patch for Platonic Friends, you will need to specify which characters are set as non-romantic in that mod's config options as well.

"RelationshipLabel" specifies what you would like to call a long-term platonic commitment with an NPC (i.e., when you give someone set as FullyPlatonic or SexWithoutRomance a pendant or bracelet). 
	It defaults to "partners," but you could set it to "housemates," "QPPs," "business partners," "FWBs," or whatever you prefer. You can change this label whenever you like.
	Characters will refer to your relationship with the label you chose.
	Avoid using special characters ($, @, ", %, etc), since this may cause errors. 
	You should phrase your label in a way that would grammatically fit into a sentence like "I can't believe we're going to be [label]!" or "I love being [label] with you."

"SocialMenuLabel" specifies how you would like your romantic spouse(s) and/or platonic partner(s) to be labeled in the social menu. 
	It defaults to "partner," but you could set it to "housemate," "husband," "wife," or whatever you prefer. You can change this label whenever you like.
	It's not possible to specify different social menu labels for different characters, so if you are using Multiple Spouses/Free Love, all housemates will have the same label.
	You can disable the custom label by setting "DisableSocialMenuLabel" to true. This will make characters you moved in with the pendant display as "husband/wife" and characters you moved in with the pendant display as "housemate" as normal.

"TermofEndearment" specifies one affectionate term you would like a platonic partner to use for you.
	It defaults to your farmer's name (represented by "@"), but you could change it to "Bestie," "My dear," "Angel," "Homie," or whatever you prefer.
	The term you choose should start with a capital letter. It will be automatically converted to lowercase when used in the middle of sentences, unless it's "@" or "BFF". (I can add more exceptions to the lowercasing on request.)
	Avoid using special characters ($, @, ", %, etc), since this may cause errors. 
	Your partner will alternate between the term you choose here, your farmer's name, and one or two terms unique to that NPC.

"AlwaysAdopt" determines whether dialogue and game messages will be edited to indicate you are adopting your child/children (in relationships where the game would normally indicate that you and your spouse/partner are having a biological child). 
	It defaults to true. This affects all NPCs REGARDLESS of their Relationship Type, even RomanceAndSex, so if you want to have biological children, you must set this option to false. 

"BraceletTheme" determines which of four color themes will be used for the Friendship Bracelet item. 
	The Friendship Bracelet is used to ask an NPC set as FullyPlatonic or SexWithoutRomance to move in as a platonic roommate. 
	The Mermaid's Pendant can also be used for this purpose, but using the Friendship Bracelet replaces kissing with hugging, removes the wedding/committment ceremony, and disables having/adopting children with that NPC.
	The four color themes can be viewed in the mod's asset files or in the images on the mod's Nexus page.
	All versions of the bracelet were created by Airyn of the Diverse Stardew Valley team! Thank you, Airyn!

"EnablePortraitEdits" determines whether this patch will affect the portraits of NPCs with a given relationship type. By default, portraits are edited for NPCs set to anything other than "RomanceAndSex". 
	For NPCs set to the enabled relationship types, blush will be removed from "love" portraits.
	These changes are fully compatible with Diverse Stardew Valley 2.4.0 or later. You will need to configure DSV to enable blush edits (see DSV's documentation for instructions).
        These changes are also fully compatible with Seasonal Outfits - Slightly Cuter Aesthetic. No action is required. 
        These changes are also compatible with most, but not all, portraits in Seasonal Villager Outfits. (For example, the portraits where Haley wears sunglasses will look odd.)
	If you are using another mod that changes character portraits, you can disable portrait edits for all relationship types to prevent conflicts.
        If you are using a rival event mod, the blush edits will also affect those events if the NPCs involved are set to platonic. This shouldn't affect the tone too badly since the 'love' portraits still have very loving expressions, but you can disable this option for the affected NPCs' relationship types if you prefer these events to involve blushing.

"UseLovePortraits" determines whether this patch will use the "love" portrait in edited dialogue and events. 
	When true, "love" portraits will be used. If EnablePortraitEdits is set to true for a given relationship type, blushing will be removed from these portraits, so they will have a vibe of affection and emotional vulnerability without the implied romantic attraction.
        When false, different portraits (usually either the default portrait or the "happy" portrait) will be used in place of the "love" portraits. (Dialogue added by other mods may still use the 'love' portraits, unless/until I add compatibility for said mods.)
        If you had to set EnablePortraitEdits to false to prevent a conflict with another mod, you can set UseLovePortraits to false to avoid blushing portraits.
        Alternatively, if you want platonic characters to blush, you can set EnablePortraitEdits to false and UseLovePortraits to true. 

"EnableSpriteEdits" determines whether this patch will alter wedding sprites. 
	When true, wedding dresses will be recolored to something other than white when "marrying" an NPC you have set to platonic.
        These changes are compatible with Seasonal Villager Outfits.
        If you have Diverse Stardew Valley 2.4.0 or later installed, enabling PlatonicNPCs in its config settings will replace platonic NPCs' wedding outfits with unique commitment ceremony outfits, designed by DSV team member Airyn (thanks Airyn!). This will happen regardless of the EnableSpriteEdits setting.
        If you have another mod thats affect sprite body shapes or wedding outfits, you can set this option to false to disable it, preventing conflicts.

"EnableScheduleChanges" makes some small changes to Alex, Elliott, and Abigail's schedules.
	In vanilla, getting to 6+ hearts with Haley stops Alex from visiting her house; 6+ hearts with Leah stops Elliott from visiting her at the saloon; and 6+ hearts with either Abigail or Sebastian stops Abigail from visiting Sebastian's room.
	When EnableScheduleChanges is set to true, these interactions won't stop occurring unless you get to 6+ hearts with one of the affected characters AND they are not set to either FullyPlatonic or SexWithoutRomance.
	For example, if you're at 6+ hearts with Haley, Alex will still visit her if you're platonic with her; otherwise, he'll stop. If Abigail and Sebastian are both 6+ hearts, Abigail will keep visiting his room if you're non-romantic with both of them; if you're romantic with either one, she'll stop.
	Set this to false if it conflicts with another mod that changes schedules or maps. 

"Auncle" specifies the title you would like NPCs in a niece/nephew/nibling-like relationship with you to use. 
	It defaults to the gender-neutral title Nini. As an example, Jas might call you "Nini" or "Nini [Farmer's name]" if you are in a platonic partnership with Shane.
	It should be capitalized, as in "Aunt", "Uncle", etc.
	This option is only relevant if you use certain dialogue and event mods that PPaF has compatibility patches for; currently, the only affected mods are Immersive Characters: Shane and Immersive Spouses. 

"SpousesReactExInvolvement" is only relevant if you are using the "Spouses React to Player 'Death'" mod, which has a config option to allow an ex-spouse to visit you in the hospital if you haven't remarried.
	When true (the default), when you have Spouses React installed and an ex-platonic partner visits you in the hospital, platonic edits are applied. 
	If you have the ExInvolvement config option set to false in Spouses React because you don't want exes to visit you in the hospital, set this option to false as well. Otherwise, the platonic edits will cause some ex-partners to visit you anyway.