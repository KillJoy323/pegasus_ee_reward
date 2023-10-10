//PASTE THIS LEVEL THREAD WHEN YOU COMPLETE YOUR CUSTOM MAPS EASTER EGG
level thread pegasus_ee_reward();

//PASTE THIS FUNCTION AT THE BOTTOM OF YOUR SCRIPT SEPARATELY
function pegasus_ee_reward() {
mod = GetDvarString("fs_game");
wait(.05);
	if( mod == "2804432292" )
	{
		foreach(player in GetPlayers())
		{
			player notify("pegasus_ee_complete");
		}
	}
}
