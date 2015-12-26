These macros were designed to work on EcoCityCraft, most of them have no function at all in singleplayer.

Available commands:

.about		Shows general PMC information.			- Core functionality
.help		Calls the help pages.					- Core functionality
.join		Toggles the Join alert.					- JoinAlert module
.sg			Allows use of further PMC SG commands.	- SurvivalGames module
.shout		Toggles the visibility of shouts		- ShoutIgnore module
.stats		Shows or resets various statistics.		- Statistics module
.tool		Toggles the automated ToolSwitcher.		- ToolSwitch module







If you plan to modify the macros in any way, the following tables may be of use.


Occupied global variables:

Variable name		Type			Description
----------------------------------------------------------------------------------------------------------
pmcerrorc			Boolean			Check for a valid command inside the PMC_Core.
pmcerror			Boolean			Check for a valid command inside a module.

pmctoolswitch		Boolean			Status of the ToolSwitcher.
pmctoolsilk			Integer			Slot ID of the silk touch pickaxe.
pmctoolspade		Integer			Slot ID of the spade.
pmctoolaxe			Integer			Slot ID of the axe.
pmctoolsword		Integer			Slot ID of the sword.
pmctoolfort			Integer			Slot ID of the fortune pickaxe.

pmcstatsmelon		Integer			Statistics module - Melons farmed since reset.
pmcstatspumpkin		Integer			Statistics module - Pumpkinss farmed since reset.
pmcstatspotato		Integer			Statistics module - Potatoes farmed since reset.
pmcstatscarrot		Integer			Statistics module - Carrots farmed since reset.
pmcstatswheat		Integer			Statistics module - Wheat farmed since reset.
pmcstatscane		Integer			Statistics module - Sugar cane farmed since reset.
pmcstatscocoa		Integer			Statistics module - Cocoa beans farmed since reset.
pmcstatsnwart		Integer			Statistics module - Netherwarts farmed since reset.
pmcstatsdatef		String			Statistics module - Date of last farming reset.
pmcstatstimef		String			Statistics module - Time of last farming reset.

pmcstatscoal		Integer			Statistics module - Coal mined since reset.
pmcstatsiron		Integer			Statistics module - Iron mined since reset.
pmcstatsgold		Integer			Statistics module - Gold mined since reset.
pmcstatslapis		Integer			Statistics module - Lapislazuli mined since reset.
pmcstatsredstone	Integer			Statistics module - Redstone mined since reset.
pmcstatsdiamond		Integer			Statistics module - Diamonds mined since reset.
pmcstatsemerald		Integer			Statistics module - Emeralds mined since reset.
pmcstatsstone		Integer			Statistics module - Stone mined since reset.
pmcstatsdatem		String			Statistics module - Date of last mining reset.
pmcstatstimem		String			Statistics module - Time of last mining reset.

pmcstatssgplayed	Integer			Statistics module - SGs played since reset.	
pmcstatssgkills		Integer			Statistics module - SG kills since reset.
pmcstatssgmoney		Integer			Statistics module - SG money since reset.
pmcstatssgwins		Integer			Statistics module - SG wins since reset.										
pmcstatsdatesg		String			Statistics module - Date of last SG reset.						
pmcstatstimesg		String			Statistics module - Time of last SG reset.

pmcchatr1			Integer			Statistics module - Rank 1 (Builder)
pmcchatr2			Integer			Statistics module - Rank 2 (Resident)
pmcchatr3			Integer			Statistics module - Rank 3 (Mayor)
pmcchatr4			Integer			Statistics module - Rank 4 (President)
pmcchatr5			Integer			Statistics module - Rank 5 (Tycoon)
pmcchatr6			Integer			Statistics module - Rank 6 (EcoLeader)
pmcchatr7			Integer			Statistics module - Rank 7 (EcoMaster)
pmcchatr8			Integer			Statistics module - Rank 8 (EcoLegend)
pmcchats1			Integer			Statistics module - Staff 1 (Moderator)
pmcchats2			Integer			Statistics module - Staff 2 (SuperMod)
pmcchats3			Integer			Statistics module - Staff 3 (GameAdmin)
pmcchats4			Integer			Statistics module - Staff 4 (ServerAdmin)
pmcchats5			Integer			Statistics module - Staff 5 (ServerOwner)
pmcchats6			Integer			Statistics module - Staff 6 (Founder)

pmcchatd1			Integer			Statistics module - Donator 1 ($)
pmcchatd2			Integer			Statistics module - Donator 2 ($$)
pmcchatd3			Integer			Statistics module - Donator 3 ($$$)
pmcchatd4			Integer			Statistics module - Donator 4 ($$$$)
pmcchatd5			Integer			Statistics module - Donator 5 (VIP)
pmcchatd6			Integer			Statistics module - Donator 6 (VIP+)
pmcchatd7			Integer			Statistics module - Donator 7 (*VIP*)

pmcchatg			Integer			Statistics module - Global chat
pmcchattr			Integer			Statistics module - Trade chat
pmcchattrv			Integer			Statistics module - Trivia chat
pmcchatauc			Integer			Statistics module - Auction chat
pmcchatv			Integer			Statistics module - VIP chat
pmcchatn			Integer			Statistics module - Nether chat
pmcchatl			Integer			Statistics module - Local chat
pmcchatp			Integer			Statistics module - PvP chat
pmcchatm			Integer			Statistics module - Mining chat
pmcchata			Integer			Statistics module - Aether chat
pmcchatal			Integer			Statistics module - Alert chat
pmcchats			Integer			Statistics module - Staff chat
pmcchatad			Integer			Statistics module - Admin chat
pmcchatsg			Integer			Statistics module - SG chat

pmcchatdate			String			Statistics module - Date of last chat reset.
pmcchattime			String			Statistics module - Time of last chat reset.

pmccommand			String			Internal core variable for executing commands.




Occupied Local variables:

Variable name	Type		Module			Description
----------------------------------------------------------------------------------------------------------
pmctoolswitch1	String		ToolSwitch		Regex pattern for silk pickaxe.
pmctoolswitch2	String		ToolSwitch		Regex pattern for shovel.
pmctoolswitch3	String		ToolSwitch		Regex pattern for axe.
pmctoolswitch4	String		ToolSwitch		--Currently unused, reserved--
pmctoolswitch9	String		ToolSwitch		Regex pattern for fortune pickaxe.

founder			String		JoinAlert		Regex pattern for [|||Founder|||].
serverowner		String		JoinAlert		Regex pattern for [ServerOwner].
serveradmin		String		JoinAlert		Regex pattern for [ServerAdmin].
gameadmin		String		JoinAlert		Regex pattern for [GameAdmin].
supermod		String		JoinAlert		Regex pattern for [SuperMod].
moderator		String		JoinAlert		Regex pattern for [Moderator].
developer		String		JoinAlert		Regex pattern for [Developer].
notable			String		JoinAlert		Regex pattern for players of interest.
bot				String		JoinAlert		Regex pattern for bots.
special			Boolean		JoinAlert		Assigns special colours to user groups.



Used Files:

File name					Module			Description
----------------------------------------------------------------------------------------------------------
PMC_Core					Main			Evaluates commands; executes other files.
PMC_Internal_Help			Main			Displays help pages.
PMC_Internal_Join			JoinAlert		Toggles the JoinAlert.
PMC_Internal_SG				SurvivalGames	Evaluates .sg commands.
PMC_Internal_Shout			ShoutIgnore		Toggles the ShoutIgnore.
PMC_Internal_Stats			Statistics		Displays or resets statistics.
PMC_Internal_ToolSwitch		ToolSwitch		Toggles the ToolSwitch.
PMC_Join					JoinAlert		Announces a joined player.			
PMC_Stats					Statistics		Updates statistics.
PMC_ToolSwitch				ToolSwitch		Adjusts inventory slot when enabled.
PMC README									PMC main manual. Never executed ingame.
