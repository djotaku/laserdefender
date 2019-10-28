# Laser Defender
A Galaxian/Galaga clone from a Unity 2D Udemy Class I'm taking

![Screenshot](https://github.com/djotaku/laserdefender/blob/master/Assets/Screenshots/Screenshot.png)

Get binaries from this repo (click on "releases")

Play on the net via WebGL:
http://server.ericsbinaryworld.com/WebGL/LaserDefenderWebGL/
 (On Linux (at least for me in Fedora 30) only was able to hear the music when playing in Google Chrome. Firefox had sound effects. Vivaldi did not have any sounds)

A video of me playing version 1.0:
https://youtu.be/OJpaR-YUXxk

Also a couple funny videos:

I forgot to set the collider as a trigger: https://youtu.be/GI_9VChCHVE

Hilarious enemy shooting pattern: https://youtu.be/e5PS3fW1Of0

# Visual and Audio Credits

Sprites: Kenny Assets. Specifically these: https://kenney.nl/assets/space-shooter-redux  - Available under Creative Commons 0 license (AKA Public Domain)

Sound FX: Kenny Assets. Specifically these: https://kenney.nl/assets/digital-audio - Available under Creative Commons 0 license (AKA Public Domain)

Music: NES Shooter Mysic by SketchyLogic (here: https://opengameart.org/content/nes-shooter-music-5-tracks-3-jingles) - Available under Creative Commons 0 license (AKA Public Domain)

# What I've Done Since Finishing this section of the class

N/A - stay tuned!

# What I learned in this module of the class

 - Using input.getaxis and time.deltatime to be frame-rate independent. Otherwise, the faster your computer is, the faster the character will move. (Also allows for controllers to work)

 - Also learned a different way: ViewportToWorldPoint() to figure out where we are on the screen on a scale of 0 to 1 in both x and y directions. 
 Compare with https://github.com/djotaku/BlockDestroyer/blob/master/Assets/Scripts/Paddle.cs where we originall used Input.mousePosition.x / Screen.width * screenWidthInUnits (before I modified to add controller support)

  - Learned some ideas of how to figure out which features to work on next. Essentially, start with Player Movement and then choose after that based on what's necessary for the game

  - Learned about coroutines - A method that can yield its execution until conditions are met. Eg: when player gets to zero health, start the KillPlayer coroutine. The first Coroutine we used was in the FireContinuously() 
  method where we set a delay between bullets fired out.

  - Learned to spawn enemy waves in a 2D game

   - Learned both how to use advanced particle effects for the explosions and for the starfields that give a parallax view

   - Learned about changing the render layer order to keep the laser from appearing on top of the player or enemy launching it.
