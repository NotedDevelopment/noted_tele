# noted_tele
Uses Angelicxs teleport as a base, but is heavily modified and transformative in nature. Allows Staff to place points which players can interact with to teleport from one location to another acting like an elevator, transport, train, bus, etc.

I'm releasing this a little early, will add some features over time when im less burnt out. I honestly just wanted to get this out there ;-;

This script was modified/made by me, Edward. If I make a tebex I'll probably add a link bellow
My discord username is "not.ex" if you would like to reach out to me for any reason
I say modified, I used Angelicxs Elevator as a base. Will give more credits below 
This is my github: https://github.com/NotedDevelopment

This script uses Angelicxs Elevator as a "jumping off point", aka it was built on top of it. 
The github to the original will be here: https://github.com/GouveiaXS/angelicxs-elevators
Angelicxs Tebex: https://angelicxs.tebex.io/

The differences between Angelicxs Elevator and this script include:

* Removed a lot of compatibility becuase I can't be asked ;-; just use qbox or qbcore with oxlib idk
* Switched from manual distance checking to oxlib points
* Added the ability to customize the display 3dtext that appears for each location
* Added the ability to enable or disable alerting the police when wanted people or those wearing gang apparel Travel
* In addition to the above feature, added the ability for police alert to have a chance at also displaying suspect's name
* Both of the above features are configured to ps-dispatch and ps-mdt, may need some tweaking to work on other systems
* Added the ability to charge money for using certain teleport spots. The price can be charged based on a flat rate or configured based on where the person is teleporting from,  or both. You can also enable or disable a confirmation menu when paying
* Allows you to hide teleport zones from the menu if they're not unlocked (aka if player doesn't have right job or item)
* If there are two seperate teleport spots, players will automatically teleport between the two rather than selecting from a mneu
* You can add a progressbar when attempting to use teleports


How to utelize the config:

Config.ElevatorWaitTime is in charge of how long players will experience being faded out when attempting to use teleports. This number will be in seconds, so 3 = 3 seconds
Config.TeleButton is meant to be a future feature where players can adjust what button allows them to use the elevator while the button that appears is a "default". For now, admins can change what button players use.
This script uses the QBCore export, cringe I know but I'll change it eventually I guess to add compatibility for ESX and direct QBox
Config.DefaultText is the text that will appear for players in the Draw3dText by default
Config.SuspectNameChance is important in the following scenario: If a teleport checks whether a suspect is wanted or not by the police, this setting will roll to see if that individual should be declared by name when identified. So if it fails, it will say "Suspect seen on Transit" vs "John Doe seen on transit".
Config.GangMasks Will have a female and male component. if the player model is female, it will check under the female table. If they are using the male ped, it'll check the male ped tag:
Female: Uses the clothing index of the mask the player may be wearing. If the index is documented, it will then check the number. If the number is documented, it will return the string associated. So for example, if player is wearing Mask 51 with texture 5, it will return the word GSF. 

