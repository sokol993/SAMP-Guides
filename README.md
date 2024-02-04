# Start of saving / loading data (YSI)
Use YSI and place it into your include folder, in the pawno folder, within the SA-MP server folder.

Path looks like this:

``\pawno\include\YSI``

In your gamemode (example.pwn) script, put at the top an include that says this:

``#include <YSI\y_ini>``

#### I couldn't find the original YSI folder online so I eventually found it in an old github repo and copied it from there. I'll upload the full YSI folder here for anyone else to use if they encounter the same issue.

# Save & Load data

To be added!! Currently it's 1AM so I'm gonna add this later lol

# Server Playtime

Use the following:

```pawn
PlayingTime[playerid] = GetTickCount(); //To store when the player connected
PlayingTime[playerid] = GetTickCount() - PlayingTime[playerid]; // Here we get the difference between when the player joined the game and left the game
```

This will store the time in miliseconds (1000ms = 1s). Combine this with the storage of data using YSI and you will be able to store the time played into a integer and use it as you see fit.
Don't use timers as a lot of them will increase CPU usage and lag the server - So I've read and it really makes sense, 20 people online each with a timer and god knows what.

# PS
I will keep adding stuff here as I go along my coding journey, this is mainly to help ME remember stuff and others along the way if it helps :D
