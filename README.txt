Fleet Carrier Generic Autopilot
by Cmdr REDACTED

Credit:
The REDACTED Expedition made the profile from which this profile is based on.
Cmdr REDACTED - Creator
Cmdr REDACTED - Updater


What is this?
This is a VoiceAttack profile that will do all of the keypresses required to pilot your fleet carrier without you needing to be present. 
If you do not have VoiceAttack, you can buy it here: https://voiceattack.com/. There is a free version that you can get to work with this 
profile, but this Readme assumes that you have the full version.

How do I make it work?
In order to get this profile working, you need to do some setup.
0. Install VoiceAttack
1. Import the profile
2. Edit the profile
3. Setup the environment. Go to EnvSetup and edit 
	a. Decide what bindings you want to use, keyboard/numpad/custom. Set the boolean variables. 
	b. If you choose custom, set the custom keybinds.
		Keyboard bindings are used by default. It's recommended that you use keyboard bindings. To do so, change your controls in ED to mouse and 
		keyboard, use the autopilot, and when you're done, change back to whatever bindings you use.
	c. Once you've completed all other setup in EnvSetup, set system_is_setup to True
4. Plot a route. See existing routes as examples
	a. Right click -> Duplicate an existing route. Name the new route and set a new keybind for calling the route.
	b. Edit the route to go where you want to go.
		i. Go to spansh and plot your route. https://spansh.co.uk/fleet-carrier
		ii. Copy the systems into the new route you made in step a). (Double check that you correctly increase the itinerary numbers!)
		iii. Set 'InitialDestIndex' to the first system that you want your FC to jump to. 
		iv. Set 'LastDestIndex' to the last system that you want your FC to jump to.
		v. hit "OK" and then "Apply"
5. Activate the autopilot
	a. Have ED open and running.
	b. If you set 'trit_refill_from_carrier', make sure that trit is the only commodity on your ship and FC. 
		Make sure that you have your right comms panel set to the inventory tab and that that tritium is selected/highlighted. 
		Make sure that the right comms panel is not up.
	c. You should be in the pilot's seat and the rearm/refuel/repair row should be selected/highlighted.
	d. Hit the key command that you set for your route.
	e. Don't hit keys, unfocus ED, or otherwise use your computer until you have arrived, or aborted the autopilot.	

NOTES:
Autopilot will continue to "plot" routes if there are systems remaining, even if you are out of fuel. This is harmless. Just abort Autopilot.
Autopilot will only be able to make ~8 jumps (1k fuel tank + your ships' hold) if you do not refill your ships' hold. Setting 'trit_refill_from_carrier' will attempt to use trit in your FC cargo hold.
If you stop in the middle of your route, make sure to update 'InitialDestIndex' in your route before starting again.
If you make a route that you think others would use, consider making a PR and adding it to this profile.

