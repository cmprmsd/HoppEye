# HoppEye
HoppEye is a simple payload picker for BashBunny based on linking payloads to LED color.

Have you ever wished to extend BashBunny with more payloads than just two?
Now this is possible by using a Picker and Runner payload combination.

# Concept and Configuration

The idea is to have up to eight scripts placed in their according folders just as they would be placed within switch1 or switch2. In order to use them plug the stick into a power source with the switch in the middle position. Now a colorwheel will start rolling, indicating each payload for one second. Just now in the right moment move the switch to position switch1 and the script will copy the content of payload\_[yourcolor]\_[anyName] to switch1, indicated by a solid light in your chosen color. When the copying is done, the stick will flash in your chosen color to indicate it is done and synced. Now unplug the stick and replug it or walk to the destination computer of your choice. ;) 

# TL;DR

Build:
1. Plug in your stick in ARM mode
2. Copy the git content to your payloads folder on the stick
3. Create your payloads within any of the colored payload folders
4. Rename the "empty" part for each payload folder to something you'll recognize
5. Remember which payload you put into which folder ;)

Use:
1. Switch Position 2
2. Plug in
3. See color wheel (Order will be R G B Y C M W OFF in an infinite loop only showing non-"empty" named)
4. Switch Position 1 to choose
5. Replug or carry arround
6. Profit

This will look like the folowing, where payload\_[color]\_[anyName] will be the naming scheme:

```
payloads/
	payload_B_BluePayload
	payload_G_Green
	payload_OFF_empty
	payload_W_network
	payload_C_empty  
	payload_M_PoisonBunnyTap
	payload_R_ReverseShellEmpire
	payload_Y_empty
```

Switch overview:
- switch1 (Execution mode)
- switch2 (Setup mode)
- switch3 (Classic arming mode)
