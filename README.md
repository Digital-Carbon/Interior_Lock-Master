# Interior_Lock-Master
This adds the ability to lock and unlock vehicles from the inside with either scroll wheel functions or the Exile default hot key to lock and unlock objects.

Installation Instruction

Step 1: Open your initPlayerLocal.sqf and paste the following into it (There is an example initPlayerLocal.sqf you can use to copy from)

[] execVM "Custom\Actions\fnc_showActions.sqf";

Step 2: In your mission root open config.sqf and find class CfgExileCustomCode and insert the below

//Custom keys
ExileClient_gui_hud_event_onKeyUp = "Custom\overwrites\ExileClient_gui_hud_event_onKeyUp.sqf";

For Example:
class CfgExileCustomCode 
{	
	//Custom keys
	ExileClient_gui_hud_event_onKeyUp = "Custom\overwrites\ExileClient_gui_hud_event_onKeyUp.sqf";
};

Step 3: Edit your description.exe and add the following

class CfgFunctions
{
	#include "Custom\CfgFunctions.cpp"
};

Step 4: Place the Custom folder into your mission folder

That's it Enjoy!
