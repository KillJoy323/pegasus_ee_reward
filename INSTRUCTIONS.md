//PASTE THIS WHEN YOU COMPLETE YOUR CUSTOM MAPS EASTER EGG, BEFORE YOU END THE GAME !
pegasus_ee_reward();

//PASTE THIS FUNCTION AT THE BOTTOM OF YOUR SCRIPT SEPARATELY ( NOT INSIDE ANY OTHER FUNCTION )
function pegasus_ee_reward() {
mod = GetDvarString("fs_game");
wait(.05);
	if( isdefined(mod) && mod == "2804432292" )
	{
		foreach(player in GetPlayers())
		{
			player notify("pegasus_ee_complete");
		}
	}
}
