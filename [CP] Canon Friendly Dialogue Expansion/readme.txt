hello! This readme is for mod makers and translators~

Canon Friendly Dialogue Expansion has just receieved a massive update to it's code! Now there is i18n functionality, a config to toggle individual npcs on/off, and shared key compatibility options. If you would like compatibility with CDE on our side, please reach out to Gizzymo on Nexus for writing/story releated compat, or Koda on Discord (Sour_Creamier) for coding or complex mod related compat

How to translate i18n:
https://github.com/Pathoschild/StardewMods/blob/develop/ContentPatcher/docs/author-guide/translations.md
https://stardewvalleywiki.com/Modding:Translations

** Please note! you only need to translate the dialogue lines found in default.json. you won't find anything to translate in the Data folder.
**Do not translate anything inside {{braces}}, and be careful when translating questions that you don't translate any of the question code! 
**Example:   "CFE_Abigail_fallSun8": "[Hmm... what should I do tonight?]#$q 27/28 fall_Sun_old#[I was thinking about dyeing my hair again... what do you think?]#$r 27 10 Sun_27#[Dye it black.]#$r 27 10 Sun_27#[Why not blonde?]#$r 27 20 Sun_WildColor#[How about bubblegum pink?]#$r 28 0 Sun_28#[I like your hair just the way it is!]", only translate the portions shown in [brackets] above, and not anything that looks like this: {{GenericNoun}} 


**EVEN IF YOUR LANGUAGE IS NOT AVAILABLE FOR MODS LIKE DIVERSE STARDEW VALLEY OR GENDER NEUTRALITY MOD TOKENS, PLEASE DO NOT REMOVE THOSE i18n KEYS FROM YOUR i18n.json FILE. THIS WILL CAUSE ERRORS FOR USERS USING YOUR TRANSLATION ALONGSIDE THOSE OTHER MODS. BILINGUAL USERS HAVE REPORTED MULTIPLE BUGS OF THIS NATURE TO US. LEAVE THEM IN, IF NECESSARY THEY CAN REMAIN IN ENGLISH.


How to upload your translation:
**Publish your i18n file alone, please do not publish the full mod/Data files! Players will drag and drop your i18n file, with your language's i18n.json inside, into CFE's i18n folder. You can also reach out to Gizzymo to include your file in the base mod, and we will mention you as a translator in our credits! We encourage you to upload the file itself though so that you can get DP and manage bugs or translation errors directly. 


List of changes made to keys used in this update:
-exact duplicates from the vanilla code have been removed across all files!
-some other keys may have been removed or added over the course of the beta of this update, but most should not be problematic for your compatibility updates. if you are unsure about a change, feel free to ask WitchWeed on Nexus or Discord.

list of new lines added (or edited) by this update:

[Stable updates]
VERSION 3.0.5 DEFAULT.JSON CHANGES
no changes were made to the default.json between updates! all translations should remain up to date with the stable release of this mod.

please ensure you have included ALL i18n tokens in your translation, even if they correspond to mods that are not translated for your language. this prevents errrors for users who are bilingual or choose to use those mods without a translation. you can leave those lines in english if they are hard to translate into your language because of syntax or cultural differences, and warn in your mod description that those lines are untranslated. Please do not translate these lines and remove their intended edits. 

ie: it would be inappropritate to translate "_gn" lines to re-add gendered language, or ".dsv" lines to remove Alex's grandparents' ethnicity. We understand localization and translation are complex, and gender is different across languages and cultures, so instead of removing inclusivity for multilingual players who want gender neutrality compatibility, please just leave those lines in english if you cannot effectively translate them into your own language. The intentional removal of lgbt+ or cultural diversity themes from the dialogue are not permittable- these edits are few and far between, and retain the canon-esq, family friendly nature of this mod. 

[Beta updates]
VERSION 3.0.4 DEFAULT.JSON CHANGES
**this update fixes some persistent bugs with question code, please be careful to update accurately to minimize bugs!**

 "CFE_Abigail_fallSun8": Sun_ instances became fall_Sun8_: fall_Sun8_old, fall_Sun8_27, fall_Sun8_27, fall_Sun8_WildColor, fall_Sun8_28
 "CFE_Abigail_fall_Sun8_old": added
 "CFE_Abigail_fall_Sun8_27": added
 "CFE_Abigail_fall_Sun8_28": added
 "CFE_Abigail_fall_Sun8_WildColor": added
 "CFE_Elliott_winterMon4":Mon_ and winterMon_ instances became winter_Mon4_: winter_Mon4_old, winter_Mon4_060, winter_Mon4_061, winter_Mon4_062, winter_Mon4_063
 "CFE_Elliott_winterMon_old": renamed CFE_Elliott_winter_Mon4_old
 "CFE_Elliott_winterMon_060": renamed CFE_Elliott_winter_Mon4_060
 "CFE_Elliott_winterMon_061": renamed CFE_Elliott_winter_Mon4_061
 "CFE_Elliott_winterMon_062": renamed CFE_Elliott_winter_Mon4_062
 "CFE_Elliott_winterMon_063": renamed CFE_Elliott_winter_Mon4_063
 "CFE_Emily_summerThu4": Thu_ instances became summer_Thu4_: summer_Thu4_old, summer_Thu4_040, summer_Thu4_041, summer_Thu4_042
 "CFE_Emily_summerThu_old": renamed CFE_Emily_summer_Thu4_old
 "CFE_Emily_Thu_040": renamed CFE_Emily_summer_Thu4_040
 "CFE_Emily_Thu_041": renamed CFE_Emily_summer_Thu4_041
 "CFE_Emily_Thu_042": renamed CFE_Emily_summer_Thu4_042
 "CFE_Gus_Mon8": instances of Mon_ became Mon8_: Mon8_old Mon8_010 Mon8_011
 "CFE_Gus_Mon8.DSV.TurkishGus": instances of Mon_ became Mon8_: Mon8_old Mon8_010 Mon8_011
 "CFE_Gus_Mon_old": renamed CFE_Gus_Mon8_old
 "CFE_Gus_Mon_010": renamed CFE_Gus_Mon8_010
 "CFE_Gus_Mon_011": renamed CFE_Gus_Mon8_011
 "CFE_Haley_Sat2": Sat_ instances became Sat2_: Sat2_old, Sat2_070 ,Sat2_070, Sat2_072, Sat2_073
 "CFE_Haley_Sat2_GN": Sat_ instances became Sat2_: Sat2_old, Sat2_070 ,Sat2_070, Sat2_072, Sat2_073 
 "CFE_Haley_Sat_old": renamed CFE_Haley_Sat2_old
 "CFE_Haley_Sat_070": renamed CFE_Haley_Sat2_070
 "CFE_Haley_Sat_072": renamed CFE_Haley_Sat2_072
 "CFE_Haley_Sat_073": renamed CFE_Haley_Sat2_073
 "CFE_Harvey_Mon2": Mon_ instances became Mon2_: Mon2_old, Mon2_080, Mon2_081, Mon2_082, Mon2_083
 "CFE_Harvey_Mon_old": renamed CFE_Harvey_Mon2_old
 "CFE_Harvey_Mon_080": renamed CFE_Harvey_Mon2_080
 "CFE_Harvey_Mon_081": renamed CFE_Harvey_Mon2_081
 "CFE_Harvey_Mon_082": renamed CFE_Harvey_Mon2_082
 "CFE_Harvey_Mon_083": renamed CFE_Harvey_Mon2_083
 "CFE_Kent_Tue10": instances of Tue_ became Tue10_: Tue10_old, Tue10_018, Tue10_019
 "CFE_Kent_Tue_old": renamed CFE_Kent_Tue10_old
 "CFE_Kent_Tue_018": renamed CFE_Kent_Tue10_018
 "CFE_Kent_Tue_019": renamed CFE_Kent_Tue10_019
 "CFE_Kent_Tue_019.DSV.NoMoreWar": renamed CFE_Kent_Tue10_019.DSV.NoMoreWar
 "CFE_Leah_Wed8": Wed_ instances became Wed8_: Wed8_old, Wed8_225, Wed8_226
 "CFE_Leah_Wed_old": renamed CFE_Leah_Wed8_old
 "CFE_Leah_Wed_225": renamed CFE_Leah_Wed8_225
 "CFE_Leah_Wed_226": renamed CFE_Leah_Wed8_226
 "CFE_Lewis_summerMon4": summer_Mon instances became summer_Mon4: summer_Mon4_old, summer_Mon4_007, summer_Mon4_007, summer_Mon4_008, summer_Mon4_008
 "CFE_Lewis_summer_Mon_old": renamed CFE_Lewis_summer_Mon4_old
 "CFE_Lewis_summer_Mon4_007": renamed CFE_Lewis_summer_Mon4_007
 "CFE_Lewis_summer_Mon4_008":  renamed CFE_Lewis_summer_Mon4_008
 "CFE_Penny_Mon4": Mon_ instances became Mon4: Mon4_old, Mon4_237, Mon4_238
 "CFE_Penny_Mon_old": renamed CFE_Penny_Mon4_old
 "CFE_Penny_Mon_237": renamed CFE_Penny_Mon4_237
 "CFE_Penny_Mon_238": renamed CFE_Penny_Mon4_238
 "CFE_Shane_Sat10": Sat_ instances became Sat10_: Sat10_old, Sat10_530, Sat10_531, Sat10_531, Sat10_532
 "CFE_Shane_Sat_old": renamed CFE_Shane_Sat10_old
 "CFE_Shane_Sat_530": renamed CFE_Shane_Sat10_530
 "CFE_Shane_Sat_531": renamed CFE_Shane_Sat10_531
 "CFE_Shane_Sat_532": renamed CFE_Shane_Sat10_532
 "CFE_SpiritsEve_Vincent": added "?" to the end of the sentence
 

VERSION 3.0.3 DEFAULT.JSON CHANGES
 CFE_Caroline_Mon6: fixed a $ error
 CFE_Caroline_Mon6.DSV.NonbinaryAbigail: fixed a $ error
 CFE_Demetrius_Tue6: fixed a $ error
 CFE_Elliott_winterMon4: winterMon_old became winter_Mon_old
 CFE_Elliott_Married_IndoorNight_6: removed an extra #
 CFE_Harvey_rainy_3: "it" changed to "at"
 CFE_Sam_Tigerseye: renamed CFE_Sam_TigersEye
 CFE_Wizard_PurpleMushroom: "elixer" became "elixir"
 CFE_WinterStar_Emily: an extra $h removed

VERSION 3.0.2 DEFAULT.JSON CHANGES
 CFE_Jodi_Mon2: renamed CFE_Jodi_Mon2y1
 CFE_Jodi_Mon2y2: added!

VERSION 3.0.1 DEFAULT.JSON CHANGES
 CFE_Elliott_Mon_060 : renamed CFE_Elliott_winterMon_060
 CFE_Elliott_Mon_061: renamed CFE_Elliott_winterMon_061
 CFE_Elliott_Mon_062: renamed CFE_Elliott_winterMon_062
 CFE_Elliott_Mon_063: renamed CFE_Elliott_winterMon_063
 CFE_Harvey_Tue2.DSV.ModdedSikhHarvey: renamed CFE_Harvey_Tue2.DSV.ModdedHarvey
 CFE_Penny_Married_spring13: renamed CFE_Penny_Married_spring12
 CFE_Sandy_fall_Fri4: renamed CFE_Sandy_fallFri4

VERSION 3.0.0 DEFAULT.JSON NOTES
A suite of Gender Neutrality Mod Tokens compatible lines! Search "_GN" in the default to find these new or adapted lines.
A suite of Diverse Stardew Valley compatible lines! Search ".DSV" in the default to find these new or adapted lines.

-Abigail-
CFE_Abigail_rainy_3
CFE_Abigail_Married_patio_3
CFE_Abigail_Married_spouseRoom_1
CFE_Abigail_Married_spouseRoom_2
CFE_Abigail_Married_spouseRoom_3
CFE_Abigail_Married_spouseRoom_4
CFE_Abigail_Married_spouseRoom_5
CFE_Abigail_Married_RainyDay_3
CFE_Abigail_Married_RainyDay_4
CFE_Abigail_Married_RainyDay_5
CFE_Abigail_Married_RainyDay_6
CFE_Abigail_Married_IndoorDay_3
CFE_Abigail_Married_IndoorDay_4
CFE_Abigail_Married_IndoorDay_11
CFE_Abigail_Married_IndoorDay_12
CFE_Abigail_Married_IndoorDay_13
CFE_Abigail_Married_IndoorDay_14
CFE_Abigail_Married_IndoorDay_15
CFE_Abigail_Married_OneKid_3
CFE_Abigail_Married_OneKid_4
CFE_Abigail_Married_OneKid_5
CFE_Abigail_Married_OneKid_6
CFE_Abigail_Married_OneKid_7
CFE_Abigail_Married_OneKid_8
CFE_Abigail_Married_TwoKids_7
CFE_Abigail_Married_TwoKids_8
CFE_Abigail_Married_Outdoor_3
CFE_Abigail_Married_Outdoor_4

-Alex-
CFE_Alex_rainy_3
CFE_Alex_Married_patio_3
CFE_Alex_Married_spouseRoom_1
CFE_Alex_Married_spouseRoom_2
CFE_Alex_Married_spouseRoom_3
CFE_Alex_Married_spouseRoom_4
CFE_Alex_Married_spouseRoom_5
CFE_Alex_Married_IndoorDay_11
CFE_Alex_Married_IndoorDay_12
CFE_Alex_Married_IndoorDay_13
CFE_Alex_Married_IndoorDay_14
CFE_Alex_Married_IndoorDay_15
CFE_Alex_Married_OneKid_7
CFE_Alex_Married_OneKid_8
CFE_Alex_Married_TwoKids_5
CFE_Alex_Married_TwoKids_6
CFE_Alex_Married_TwoKids_7
CFE_Alex_Married_TwoKids_8

-Caroline-
CFE_Caroline_rainy_3

-Clint-
CFE_Clint_rainy_3

-Demetrius-
CFE_Demetriust_rainy_3

-Dwarf-
CFE_Dwarf_rainy_3

-Elliott-
CFE_Elliott_rainy_2
CFE_Elliott_rainy_3
CFE_Elliott_Married_patio_3
CFE_Elliott_Married_spouseRoom_1
CFE_Elliott_Married_spouseRoom_2
CFE_Elliott_Married_spouseRoom_3
CFE_Elliott_Married_spouseRoom_4
CFE_Elliott_Married_spouseRoom_5
CFE_Elliott_Married_RainyDay_3
CFE_Elliott_Married_RainyDay_4
CFE_Elliott_Married_RainyDay_5
CFE_Elliott_Married_RainyDay_6
CFE_Elliott_Married_IndoorDay_3
CFE_Elliott_Married_IndoorDay_4
CFE_Elliott_Married_IndoorDay_9
CFE_Elliott_Married_IndoorDay_10
CFE_Elliott_Married_IndoorDay_10
CFE_Elliott_Married_IndoorDay_11
CFE_Elliott_Married_IndoorDay_12
CFE_Elliott_Married_IndoorDay_13
CFE_Elliott_Married_IndoorDay_14
CFE_Elliott_Married_IndoorDay_15
CFE_Elliott_Married_IndoorNight_5
CFE_Elliott_Married_IndoorNight_6
CFE_Elliott_Married_IndoorNight_7
CFE_Elliott_Married_IndoorNight_8
CFE_Elliott_Married_OneKid_7
CFE_Elliott_Married_OneKid_8
CFE_Elliott_Married_Outdoor_9
CFE_Elliott_Married_Outdoor_10

-Emily-
CFE_Emily_rainy_3
CFE_Emily_Married_patio_3
CFE_Emily_Married_spouseRoom_1
CFE_Emily_Married_spouseRoom_2
CFE_Emily_Married_spouseRoom_3
CFE_Emily_Married_spouseRoom_4
CFE_Emily_Married_spouseRoom_5
CFE_Emily_Married_IndoorDay_11
CFE_Emily_Married_IndoorDay_12
CFE_Emily_Married_IndoorDay_13
CFE_Emily_Married_IndoorDay_14
CFE_Emily_Married_IndoorDay_15
CFE_Emily_Married_OneKid_7
CFE_Emily_Married_OneKid_8
CFE_Emily_Married_TwoKids_2
CFE_Emily_Married_TwoKids_5
CFE_Emily_Married_Outdoor_7
CFE_Emily_Married_Outdoor_8

-Evelyn-
CFE_Evelyn_rainy_3

-George-
CFE_George_rainy_3

-Gus-
CFE_Gus_rainy_3

-Haley-
CFE_Haley_rainy_3
CFE_Haley_Married_patio_3
CFE_Haley_Married_spouseRoom_1
CFE_Haley_Married_spouseRoom_2
CFE_Haley_Married_spouseRoom_3
CFE_Haley_Married_spouseRoom_4
CFE_Haley_Married_spouseRoom_5
CFE_Haley_Married_RainyDay_3
CFE_Haley_Married_RainyDay_4
CFE_Haley_Married_RainyDay_5
CFE_Haley_Married_RainyDay_6
CFE_Haley_Married_RainyDay_7
CFE_Haley_Married_RainyDay_8
CFE_Haley_Married_RainyDay_9
CFE_Haley_Married_RainyDay_10
CFE_Haley_Married_IndoorDay_1
CFE_Haley_Married_IndoorDay_2
CFE_Haley_Married_IndoorDay_3
CFE_Haley_Married_IndoorDay_4
CFE_Haley_Married_IndoorDay_5
CFE_Haley_Married_IndoorDay_6
CFE_Haley_Married_IndoorDay_7
CFE_Haley_Married_IndoorDay_8
CFE_Haley_Married_IndoorDay_11
CFE_Haley_Married_IndoorDay_12
CFE_Haley_Married_IndoorDay_13
CFE_Haley_Married_IndoorDay_14
CFE_Haley_Married_IndoorDay_15
CFE_Haley_Married_IndoorNight_5
CFE_Haley_Married_IndoorNight_6
CFE_Haley_Married_OneKid_3
CFE_Haley_Married_OneKid_4
CFE_Haley_Married_OneKid_5
CFE_Haley_Married_OneKid_6
CFE_Haley_Married_OneKid_7
CFE_Haley_Married_OneKid_8
CFE_Haley_Married_TwoKids_5
CFE_Haley_Married_TwoKids_6
CFE_Haley_Married_TwoKids_7
CFE_Haley_Married_TwoKids_8
CFE_Haley_Married_Outdoor_1
CFE_Haley_Married_Outdoor_2
CFE_Haley_Married_Outdoor_5
CFE_Haley_Married_Outdoor_6

-Harvey-
CFE_Harvey_rainy_3
CFE_Harvey_Married_jobLeave_1
CFE_Harvey_Married_jobLeave_2
CFE_Harvey_Married_jobLeave_3
CFE_Harvey_Married_jobLeave_4
CFE_Harvey_Married_jobReturn_1
CFE_Harvey_Married_jobReturn_2
CFE_Harvey_Married_jobReturn_3
CFE_Harvey_Married_jobReturn_4
CFE_Harvey_Married_patio_3
CFE_Harvey_Married_spouseRoom_1
CFE_Harvey_Married_spouseRoom_2
CFE_Harvey_Married_spouseRoom_3
CFE_Harvey_Married_spouseRoom_4
CFE_Harvey_Married_spouseRoom_5
CFE_Harvey_Married_RainyDay_1
CFE_Harvey_Married_RainyDay_2
CFE_Harvey_Married_RainyDay_7
CFE_Harvey_Married_RainyDay_8
CFE_Harvey_Married_IndoorDay_1
CFE_Harvey_Married_IndoorDay_2
CFE_Harvey_Married_IndoorDay_3
CFE_Harvey_Married_IndoorDay_4
CFE_Harvey_Married_IndoorDay_11
CFE_Harvey_Married_IndoorDay_12
CFE_Harvey_Married_IndoorDay_13
CFE_Harvey_Married_IndoorDay_14
CFE_Harvey_Married_IndoorDay_15
CFE_Harvey_Married_IndoorNight_3
CFE_Harvey_Married_IndoorNight_4
CFE_Harvey_Married_OneKid_5
CFE_Harvey_Married_OneKid_6
CFE_Harvey_Married_OneKid_7
CFE_Harvey_Married_OneKid_8
CFE_Harvey_Married_TwoKids_8

-Jas-

-Jodi-
CFE_Jodi_rainy_2
CFE_Jodi_rainy_3

-Kent-
CFE_Kent_RoastedHazelnuts_1
CFE_Kent_RoastedHazelnuts_2

-Krobus-
CFE_Krobus_rainy_3
CFE_Krobus_Married_spouseRoom_1
CFE_Krobus_Married_spouseRoom_2
CFE_Krobus_Married_spouseRoom_3
CFE_Krobus_Married_spouseRoom_4
CFE_Krobus_Married_spouseRoom_5
CFE_Krobus_Married_IndoorDay_13
CFE_Krobus_Married_IndoorDay_14
CFE_Krobus_Married_IndoorDay_15

-Leah-
CFE_Leah_rainy_3
CFE_Leah_fallMon6_1
CFE_Leah_fallMon6_2
CFE_Leah_Married_IndoorDay_3
CFE_Leah_Married_IndoorDay_4
CFE_Leah_Married_IndoorDay_7
CFE_Leah_Married_IndoorDay_8
CFE_Leah_Married_IndoorDay_11
CFE_Leah_Married_IndoorDay_12
CFE_Leah_Married_IndoorDay_13
CFE_Leah_Married_IndoorDay_14
CFE_Leah_Married_IndoorDay_15
CFE_Leah_Married_patio_3
CFE_Leah_Married_spouseRoom_3
CFE_Leah_Married_spouseRoom_4
CFE_Leah_Married_spouseRoom_5
CFE_Leah_Married_Outdoor_8
CFE_Leah_Married_Outdoor_9

-Leo-

-LeoMainland-
CFE_Leo_rainy_2
CFE_Leo_rainy_3

-Lewis-
CFE_Lewis_rainy_3

-Linus-
CFE_Linus_rainy_3

-Marnie-
CFE_Marnie_rainy_3

-Maru-
CFE_Maru_rainy_3
CFE_Maru_Married_jobLeave_1
CFE_Maru_Married_jobLeave_2
CFE_Maru_Married_jobLeave_3
CFE_Maru_Married_jobLeave_4
CFE_Maru_Married_jobReturn_1
CFE_Maru_Married_jobReturn_2
CFE_Maru_Married_jobReturn_3
CFE_Maru_Married_jobReturn_4
CFE_Maru_Married_patio_3
CFE_Maru_Married_spouseRoom_1
CFE_Maru_Married_spouseRoom_2
CFE_Maru_Married_spouseRoom_3
CFE_Maru_Married_spouseRoom_4
CFE_Maru_Married_spouseRoom_5
CFE_Maru_Married_RainyDay_3
CFE_Maru_Married_RainyDay_4
CFE_Maru_Married_RainyDay_5
CFE_Maru_Married_RainyDay_6
CFE_Maru_Married_RainyNight_5
CFE_Maru_Married_RainyNight_6
CFE_Maru_Married_IndoorDay_11
CFE_Maru_Married_IndoorDay_12
CFE_Maru_Married_IndoorDay_13
CFE_Maru_Married_IndoorDay_14
CFE_Maru_Married_IndoorDay_15
CFE_Maru_Married_IndoorNight_5
CFE_Maru_Married_IndoorNight_6
CFE_Maru_Married_OneKid_7
CFE_Maru_Married_OneKid_8
CFE_Maru_Married_TwoKids_3
CFE_Maru_Married_TwoKids_4
CFE_Maru_Married_TwoKids_5
CFE_Maru_Married_TwoKids_6
CFE_Maru_Married_TwoKids_7
CFE_Maru_Married_TwoKids_8

-Pam-
CFE_Pam_rainy_2
CFE_Pam_rainy_3

-Penny-
CFE_Penny_rainy_3
CFE_Penny_Married_jobLeave_1
CFE_Penny_Married_jobLeave_2
CFE_Penny_Married_jobLeave_3
CFE_Penny_Married_jobLeave_4
CFE_Penny_Married_jobReturn_1
CFE_Penny_Married_jobReturn_2
CFE_Penny_Married_jobReturn_3
CFE_Penny_Married_jobReturn_4
CFE_Penny_Married_patio_3
CFE_Penny_Married_spouseRoom_1
CFE_Penny_Married_spouseRoom_2
CFE_Penny_Married_spouseRoom_3
CFE_Penny_Married_spouseRoom_4
CFE_Penny_Married_spouseRoom_5
CFE_Penny_Married_RainyDay_3
CFE_Penny_Married_RainyDay_4
CFE_Penny_Married_IndoorDay_11
CFE_Penny_Married_IndoorDay_12
CFE_Penny_Married_IndoorDay_13
CFE_Penny_Married_IndoorDay_14
CFE_Penny_Married_IndoorDay_15
CFE_Penny_Married_OneKid_6
CFE_Penny_Married_OneKid_7
CFE_Penny_Married_OneKid_8
CFE_Penny_Married_Outdoor_1
CFE_Penny_Married_Outdoor_2
CFE_Penny_Married_Outdoor_5
CFE_Penny_Married_Outdoor_6

-Pierre-
CFE_Pierre_rainy_3

-Robin-
CFE_Robin_rainy_3

-Sam-
CFE_Sam_rainy_3
CFE_Sam_Married_patio_3
CFE_Sam_Married_spouseRoom_1
CFE_Sam_Married_spouseRoom_2
CFE_Sam_Married_spouseRoom_3
CFE_Sam_Married_spouseRoom_4
CFE_Sam_Married_spouseRoom_5
CFE_Sam_Married_RainyNight_6
CFE_Sam_Married_RainyNight_7
CFE_Sam_Married_IndoorDay_3
CFE_Sam_Married_IndoorDay_4
CFE_Sam_Married_IndoorDay_7
CFE_Sam_Married_IndoorDay_8
CFE_Sam_Married_IndoorDay_9
CFE_Sam_Married_IndoorDay_10
CFE_Sam_Married_IndoorDay_11
CFE_Sam_Married_IndoorDay_12
CFE_Sam_Married_IndoorDay_13
CFE_Sam_Married_IndoorDay_14
CFE_Sam_Married_IndoorDay_15
CFE_Sam_Married_OneKid_5
CFE_Sam_Married_OneKid_6
CFE_Sam_Married_OneKid_7
CFE_Sam_Married_OneKid_8
CFE_Sam_Married_TwoKids_8
CFE_Sam_Married_Outdoor_5
CFE_Sam_Married_Outdoor_6

-Sandy-
CFE_Sandy_rainy_2
CFE_Sandy_rainy_3

-Sebastian-
CFE_Sebastian_rainy_3
CFE_Sebastian_Married_patio_3
CFE_Sebastian_Married_spouseRoom_1
CFE_Sebastian_Married_spouseRoom_2
CFE_Sebastian_Married_spouseRoom_3
CFE_Sebastian_Married_spouseRoom_4
CFE_Sebastian_Married_spouseRoom_5
CFE_Sebastian_Married_RainyDay_3
CFE_Sebastian_Married_RainyDay_4
CFE_Sebastian_Married_RainyDay_5
CFE_Sebastian_Married_RainyDay_6
CFE_Sebastian_Married_RainyDay_9
CFE_Sebastian_Married_RainyDay_10
CFE_Sebastian_Married_RainyNight_2
CFE_Sebastian_Married_RainyNight_3
CFE_Sebastian_Married_RainyNight_4
CFE_Sebastian_Married_RainyNight_5
CFE_Sebastian_Married_RainyNight_6
CFE_Sebastian_Married_RainyNight_7
CFE_Sebastian_Married_IndoorDay_1
CFE_Sebastian_Married_IndoorDay_2
CFE_Sebastian_Married_IndoorDay_3
CFE_Sebastian_Married_IndoorDay_4
CFE_Sebastian_Married_IndoorDay_5
CFE_Sebastian_Married_IndoorDay_6
CFE_Sebastian_Married_IndoorDay_7
CFE_Sebastian_Married_IndoorDay_8
CFE_Sebastian_Married_IndoorDay_11
CFE_Sebastian_Married_IndoorDay_12
CFE_Sebastian_Married_IndoorDay_13
CFE_Sebastian_Married_IndoorDay_14
CFE_Sebastian_Married_IndoorDay_15
CFE_Sebastian_Married_IndoorNight_1
CFE_Sebastian_Married_IndoorNight_2
CFE_Sebastian_Married_IndoorNight_3
CFE_Sebastian_Married_IndoorNight_4
CFE_Sebastian_Married_IndoorNight_5
CFE_Sebastian_Married_IndoorNight_6
CFE_Sebastian_Married_OneKid_7
CFE_Sebastian_Married_OneKid_8
CFE_Sebastian_Married_TwoKids_8
CFE_Sebastian_Married_Outdoor_1
CFE_Sebastian_Married_Outdoor_2

Shane
CFE_Shane_rainy_3
CFE_Shane_Married_patio_3
CFE_Shane_Married_spouseRoom_1
CFE_Shane_Married_spouseRoom_2
CFE_Shane_Married_spouseRoom_3
CFE_Shane_Married_spouseRoom_4
CFE_Shane_Married_spouseRoom_5
CFE_Shane_Married_IndoorDay_10
CFE_Shane_Married_IndoorDay_11
CFE_Shane_Married_IndoorDay_12
CFE_Shane_Married_IndoorDay_13
CFE_Shane_Married_IndoorDay_14
CFE_Shane_Married_IndoorDay_15
CFE_Shane_Married_OneKid_6
CFE_Shane_Married_OneKid_7
CFE_Shane_Married_OneKid_8
CFE_Shane_Married_TwoKids_7
CFE_Shane_Married_TwoKids_8

-Vincent-

-Willy-

-Wizard-
CFE_Wizard_rainy_3

CFE_npc_rainy_1; CFE_npc_rainy_2
