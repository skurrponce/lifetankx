====================================

	LifeTank X
	
====================================

 Authors:
 - Original LifeTank: Spk/Spax (spk@darkside-online.com)
 - LTx Development : Xeon Xarid / XeonX
 - LTXI Development : C'relic





Release History:

 Version 11.7.9
 --------------------

 - Now paints a red arrow above your target



 Version 11.5.3
 --------------------
 - Buff Buddy: Can setup buff profile for a buff buddy
 - Fellow Helper: Stam regen for fellows now works
 - Misc other bug fixes




 Version 9.6
 --------------------
 - New Option: Multiple Salvages At Once - lets you benefit from the new AC salvaging mechanic which allows you to salvage more than
   one material at once. Note: you must also have the option enabled in your AC client settings.
 - New Option: Answer LT commands in-game - Allows you to enable/disable commands sent to your macro from the game by people (like Sweet Mary)
 - Monarch accounts owning an allegiance authorization should now be able to use LT too!
 - A bug that let allegiance members using the auto-salvager has been fixed.
 - The Auto-Salvager will now only salvage items that have been IDed at least once. This will prevent the macro from salvaging these majors 
   that you let in your main pack after relogging.
 - Brand New Shiney Sophisticated Admin Alert! UCMers rejoice!
 - Fixed a bug that would let tell alert sounds stop the looping admin alert sound. Admin alert sound has now been given top priority over
   other sounds.
 - A bug caused by the introduction of the new Salvaging skill was bugging the Xp code, causing LT to not displaying your real xp/hour and level. 
   This has been fixed.
 - Expiration Date Updated

 Version 9.5
 --------------------
 - Expiration Date Updated
 - Owners of Single & Patron Lifetank Authorizations will now have access to the Auto-Salvager once
   the server-side database will be updated

 Version 9.4
 --------------------
 - Changed the way Buff Spells are removed from the buff queue once casted. LifeTank now checks for the "You cast XXX spell" message from the AC console, and remove the buff spell from the queue if XXX is the last buff spell casted
 - Fixed the RunState error happening for people using LifeTank through an Allegiance or Patron access. This prevented the macro from looting as a side effect.
 - LifeTank now detects vulns expirations and will recast them accordingly
 - Improved AutoLooter : 
	- LifeTank will no longer get stuck for 4 seconds when trying to open a body already in use, too far,
   	  or trying to loot an item from a body that is no longer opened.
	- LifeTank won't try to ID items it has already assessed in the last 2 minutes, speeding up the looting process when
	  opening the bodies again after getting interupted while looting
	- Added the Chiran/Nariyid/Lorica/Leather armor types in the Armor Filters tab
	- Replaced the Min AL dropdown control by a text field, in the Armor Filters tab
	- Added more options for Majors/Minors looting : you can now choose to only loot minor wards/attributes/masteries, and 
	  can skip Major Bane items
 	- Fixed Wand Filter bug - The minimum defense/magicD modifiers criteras were actually considered maximums!
 - Fellowship recruit range increased to 9 units
 - The Async Web Request code is now asynchronous for real !
 
 Version 9.3
 --------------------
 - Added Auto-Salvager - Please note that this feature is currently restricted : DO NOT email me about this, I will
   just ignore any message relating to this topic.
 - Fixed Navigation
 - New asynchronous web request code - should fix some problems people were having with Http Request Timeouts and
   excessive lag at login
 - Fixed weapon looting bug
 - Added Melee & MagicD bonus criteras for the Wand Filter
 - You can now ignore some types of monsters again by disabling them in the monster list (first column)
   and making sure the "Attack anything" option in the Macro>Targeting tab is unchecked
 - LifeTank no longer requires ImpFilter to run. You can disable it to increase performances (or rather,
   to decrease lag ;) You can even turn off WorldFilter to further improve performances and reduce RAM/CPU 
   usage.
 - Lifetank will now display your current level as shown on TreeStats on the Stats HUD and in the #cmdmacro report string
 - Fixed issues with Xp Tracker


 Version 9.2
 --------------------
 - Fixed Armor Looting bug, where LT would not be able to recognise armor types
 - Added an Exceptions list in the Loot tab, where you can add all these valuable items you don't
   want to see salvaged/sold at shop by mistake ;)

 Version 9.1
 --------------------
 - Quick-Sell : open a vendor (i.e armorer, jeweler) and hit the CTRL+F5 key or type "/lt sell" 
   (without the quotes) to automatically move all the sellable items from your main pack to the vendor
   window. This new feature take your current Lifetank Loot filters settings into account, and only moves
   items that don't match your salvages/armors/weapons/wands/major filters. That way, you can sell all the
   garbage in 2 seconds, and keep all the important items ! Thanks LT, one more tedius task removed from the
   game! ;)
 - Quick-Ust : open your ust, select an item to salvage, then hit CTRL+F6 or type "/lt ust sel" (without the quotes)
   to automatically move all the items of the same salvage type from your main pack to the ust. This isn't the autosalvager
   yet, but we're getting closer ! :)
 - Expiration Date update
 

 Version 9.0 beta
 --------------------
 - All AC protocol code moved to DarksideFilter
 - Major changes to the code structure
 - Targetting Code rewritten
 - Fixed special items looting bugs (you can now loot peas, yay!!)
 - Updated the monster tab to auto-search monster name as you type it
 - Fixed Debuff All Monsters first
 - Fixed myFormatTimer Overflow error
 - Many performance boosts
 - Added Dire's BuffSelf.dat modified buff list to the installer
 - Macro should now wait until the melee/archer attack move is completed before changing state. This
   will prevent the macro from getting stuck when trying to equip a wand to restam, etc.
 - Melee Restam will now correctly handle mana
 - Added emergency revitalize if both mana and stamina drop under 40
 - Macro will find a default vuln/war if you haven't picked one
 - No longer spams you for invalid vuln/war if you don't have War trained
 - Fellowship and Allegiance members are considered friendly by the macro

 ** Known Issues **
 - Doesn't loot scrolls *yet*
 - Sometimes skips a spell or two while buffing
 - Some people are having problems connecting to the authorization server

 Version 8.9
 --------------------

 ## NOTE: MAKE SURE YOU UNINSTALL ANY PREVIOUS LT VERSION BEFORE INSTALLING THIS ONE ! ##

 - Removed SmartFilter
 - Introduced Darkside Filter
 - Fixed Patron Authorization issues
 - Expiration date set to 20th of August

 I'm currently rewritting some parts of the macro (hence the new Network Filter). I believe it's
 necessary and will strongly benefit the plugin in the long run. However, due to the amount of work
 involved in this, I haven't been able to fix the targetting issues yet. This is definately on my priority
 list and another version should be up soon to adress these problems.

 Version 8.8
 --------------------
 - Added support for Verdantine server
 - Added option to select attack height in melee/archer mode
 - Added support for the new item banes changes : check "Select self to bane" in the Buffs>Item tabs to use it
     Warning : don't forget to set your minimum mana treshold high enough to always be able to cast your item banes
 - Added support for Patron Authorizations. Check out the website for more info.
 - Added Death Alarm to alert you when your macro somehow managed to get owned
 - Added back support for LifeTank admins
 - Added support for server-dependant profiles - If you have the same character name on Winterseeb and Verdantine, then your
   VT profile will be called "<Yourcharname> (VT)" and your WE profile "<Yourcharname> (WE)" to prevent collisions.
   Make sure you rename your old profile folders using this new convention.
 - Fixed case sensitiviness on authorization names
 - Added ImpFilterV2 8.0.

 
 Version 8.7
 --------------------
 - New authorization system : LifeTank is now using a web-based authorization system. You will have to register
   for a darkside account at www.darkside-online.com and request an allegiance or single-account authorization
   for each server you want to macro on. If you're a former lifetank user/purchaser please mention is in the 
   comments section (give the name you used back then) and I will activate it after verification.
 - Added Defender Item Buff for Wands
 - Fixed the Fellowship Recruit (will now work with chat box expanded or not)
 - Added options to select the spell level for stam/mana revitalization spells, healing spells, and emergency spells
 - Removed some debug spam
 - Expiration date set to 20th June

 Another update will follow shortly to add support for the upcoming July's patch changes to the Item Banes, and add
 support for the new server.

 Version 8.6
 --------------------
 - #revision 6 : fixed authorization error due to the 6th character slot
 - April Fix (never too late!)
 - Expiration date pushed to 1st of July

 Version 8.5
 --------------------
 - Fixed authorization problems on the Darktide server
 - LifeTank2 Trial system implemented

 Version 8.4
 --------------------
 - Support for Decal 2.6.1.0 (everything should be functionnal now)
 - The chat logger should now be logging tells and allegiance chat as intended
 - Now installs Darkside SmartFilter used by LifeTank2

 Version 8.1 (Hotfix)
 --------------------
 - Fixed broken Fletching code
 - Increased the AutoLooter Open Corpse secure timer value
 - Fixed the Imperil bug, where imperil would be casted over and over on the same target

 Version 8
 --------------------
 - Turbo mode added - Will make the macro spam a bit more, and be slightly unstable, but should make it more reactive and
   cast spells faster - Don't modifity the Cast Breaker slider unless you know what it's used for.
 - Added a slider to set the main macro timer refresh interval
 - '#cmdmacro where' is supported again
 - New channel command '#cmdmacro server' to get the macro to report their AC server
 - New option in the IRC tab to add a prefix to your IRC name (max 3 chars) - LT2_XXX|Yourroxorname
 - Added AntiBan option to report Open chat & private tells to the IRC channel when enabled
 - Fixed continuous buffing mode - Should now behave as intended
 - Fixed the IRC bug where not all the users in the channel were visible
 - Force Rebuff should now work even if you have Enable Buffing unchecked
 - The buff list is now rebuilt on every buff cycle, to take into account equipment & buff spells changes
   without having to restart the macro
 - The Lifetank Casting Messages Filter is now working ! There you go, Observer ;)

 Pea Splitting will be added in next release.

 Beta 7
 --------------------
 - Reworked the Auto-Looter : 
	- new Filters for all your Salvages, Weapons, Armors and Wands needs. A Must Check !
   	If you need to test your filters on an item : select it, ID it, then type /validpickup. LT2 will tell you if this
   	item passed at least one of your currently activated loot filters.
	- Rewrote the looting algorithm to be faster, more efficient and a lot more CPU friendly
 - Fixed the Healing code so that the macro will be able to use healing kits/potions even in Mage macro mode if the "Spells" regen
   method is unchecked
 - Fixed slow Elapsed-Time timer bug
 - Bow should now get buffed as intended in Archer Mode
 - Fixed the Timers Midnight Bug
 - Added code to "Logout on Death" - Macro will logout after exiting portal space (at Lifestone)
 - If you uncheck "Enable Buffing" while the macro is running, it will now prevent it from casting buffs until
   you check it again
 - Added a litlle hack to the ToggleCombat function so that it will push the Left Arrow Key before the Toggle Combat Mode key. This
   is supposed to ensure that the AC client will always react to the change combat mode order.
 - Fixed a bug wher some buff spells would get skiped after a fizzle in Force rebuff mode while the macro is not running
 - Increased the macro's Combat Reaction time

 
 Beta 6
 --------------------
 - OMG Looting is in ! :p Havent been able to hardcore-test it, but it should work decently. I'm working on a new filter
   system to replace the current one.
 - Added Profile support -> You now have 3 kinds of profiles : Macro, Buffs and Loot profiles. Loot profiles are shared
   between all your different characters, while the Macro & Buffs profiles are character-specific. The macro profiles
   cover the macro settings part (attack ranges, nav, weapons to use, etc...).
 - Auto Missing-Keys detection at login. An error message will be displayed telling you which keys are missing.
 - Fixed a major bug in the timer code. Basically, LT seconds were getting longer and longer ;) This was, for instance,
   causing the macro to start rebuffing at 62 minutes instead of 55, making it look like it was skipping some buffs.
 - Fixed many bug from previous versions (IRC spam, xp to next level, etc)
 - Fixed flaws in the healing code, where the macro would fall into an infinite loop and end up killed
 - Added more checks in the CombatMode Change code
 - Improved performances
 - <Insert stuff I forgot here>

 Beta 5
 --------------------
 A lot of new content here. Most important include :
 - Remote IRC / Remote Commands from LT1
 - Anti-Ban arsenal (admin alerts, unfriend player detection...)
 - Fellowship Auto-Recruit (resolution independant please!)
 - Restam for melees/archers (Stamina Elixir implemented!)
 - Private/Public Chat Logging
 - Selectable Logout Conditions (macro > options tab - logout on death, or low tapers, scarabs,healing kits)
 - Shortcut keys are now all CTRL+ based (ie CTRL+F1 to start macro, CTRL+F4 to show the route editor, etc) except for PAUSE
 - Danger Zone
 - Xp Stats (on HUD too)
 - Elapsed/Next Rebuff timers display
 - Selectable spell levels for buff spells, macro spells (heal/revitalize/stam2mana, etc)
 - Filters
 - Server-Based Authorization code
 - HUD options (Options > HUD)
 - Improved User Interface (made it smaller, to match LT1's UI dimension)
 - 100 other stuff Im forgetting...

 > What will be added in the next release(s) : Looting, AutoSalvage, Fellow Helper, Buff Others

 NOTE : The macro should be fully operationnal for xp-whorage now. Please report any bug or wierd behaviors (beside the occasionnal
 	warnings). If you enjoy it please show your support and donate a bit, even $5 or $10 will do ! Im hardly playing AC at all now,
	and this is my last motivation factor ;) You should be able to kiss Eltank goodbye on the next release !

 Beta 4
 --------------------
 - Added the Navigation System :
	- Hit F4 to open the Route Editor (not 100% complete)
	- Don't forget to SAVE your new routes after adding waypoints, as they don't get saved if you change route or logout
	- There currently are 3 types of navigation :
		- One Time Travel : the macro will try to reach the last waypoint of the route, and stop there definitivly (note: this will disable navigation)
		- Loop : once the macro reachs the last waypoint of the route, it will move on to the first waypoint of the list
		- Reverse : once the macro reachs the last waypoint of the route, the macro will use the same route again but in a reversed waypoint order
	  NOTE: at the moment, the route navtype is independant of the route data
	- To make the macro use a route while it's running, you must select the current route in the Route Editor, and define the navigation type. 
	  Then you must enable navigation in the Macro > Nav tab.
	- While it's running, the macro will :
		- Check if you need healing
		- Look for targets
	   --> If one of these criteras is met, the macro will stop running and move to Idle state to resume the regular macro behavior
	- If the macro is in idle state, with no valid targets nearby, the navigation system will be triggered and the macro will try to move to the next waypoint
	- Upon reaching a waypoint, the macro will stop for a short period (0.5 seconds at the moment, but this will be customizable later on) 
	  and wait for targets in idle state
	- When the macro will try to move to its first waypoint, it will look up in its route data to find the closest waypoint and go for this one
 - Added code for War/Vuln/Default Damage selection
 - Fixed Force Default Damage

 Beta 3
 --------------------
 - AC Client Idle Timer is now forced to 1+ year (decal 2.6 functionnality)
 - Simple HUD (will be improved later) - Also display numeric ranges
 - Melee mode implemented
 - Archer mode implemented
 - Fletching implemented
 - New Keyboard shorcuts :
    - F2 = Toggle HUD On/Off
    - F3 = Force Rebuff

	Tests Needed:
 	---------------
 	- Archer/Melee combat
	- Fletching behavior when the craft fails (should restart fletching and not get stuck)
	- PK attack (PKL not supported yet) : need to check if a PK Macro attacks other unfriendly PKs nearby
	- Stability checks (the macro must not get stuck forever in a state)

 Beta 2
 --------------------
 - Keyboard shorcuts :
    - F1 = Start/Stop Macro
    - PAUSE = Pause/Resume Macro
 - Healing
 - Combat (Mage - only the basic options implemented : vuln/arc/yield/imperil/debuff all first)

 Beta 1
 --------------------------------
 - Can't attack yet
 - new Buffer
 - new UI 
 - Many functionnalities aren't working yet
