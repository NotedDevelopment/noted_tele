# noted_tele
Uses Angelicxs teleport as a base, but is heavily modified and transformative in nature. Allows Staff to place points which players can interact with to teleport from one location to another acting like an elevator, transport, train, bus, etc.


This script was modified/made by me, Edward. If I make a tebex I'll probably add a link bellow
My discord username is "not.ex" if you would like to reach out to me for any reason
I say modified, I used Angelicxs Elevator as a base. Will give more credits below 
This is my github: https://github.com/NotedDevelopment

This script uses Angelicxs Elevator as a "jumping off point", aka it was built on top of it. 
The github to the original will be here: https://github.com/GouveiaXS/angelicxs-elevators
Angelicxs Github: https://angelicxs.tebex.io/

The changes this script made are the following:

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
