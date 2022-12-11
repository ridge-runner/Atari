Learning how to Program Atari ROMs
=====
![image](https://user-images.githubusercontent.com/1127580/206881506-313db347-1771-47f5-9a31-39eeebf28393.png)

## Contents of the repo:
* XMACROS.h - helps with the program clock.
* MACROS.h - contains macros that clean up the registry and other utilities.
* VCS.h - contains critical macros that control video output and input for the console.
* exercises - currently the practice file.
* other files standard with git repos.

## DEV LOG 
### Starting point.
**2/10/22** Just getting used to the development environment and "platform" of the Atari 2600/VCS. So far, I've learned how to switch on the controls for the TIA chip that controls screen output for NTSC/PAL devices. I haven't made it to audio output and controller input yet.  I have become relatively comfortable with the 6502 Opcodes/Nemonics over the last day or two.

**Cathod Ray Tube TVs**
Having grown up around CRT-TVs, I had no idea how these were programmed. So, this has been a worthwhile time investment just to come to grips with how the Atari developers managed to build user experiences with these systems.

**The unseen areas of CRT-TVs**
There are unseen areas of CRT TVs that viewers don't see.  That is the Vertical Sync scanlines, Vertical Blank, Horizontal Blank, and Overscan regions of the picture. These regions help keep the CRT and incoming video signal syncronized.  Since, back in the days of over-air broadcast, there could be delays or disturbances in signal strength and quality.  Further, closed captioning data could be stored in the "Blanks". 

As far as Atari programming goes, we have to wait (progammaticly) for the CR to return from the blank to the viewable area. In the VCS.h file, there are helper macros that handle that process.


## Resources
8bit Workshop is a website with an online IDE that supports Atari 2600, NES, and other old school sytems.
[Open this project in 8bitworkshop](http://8bitworkshop.com/redir.html?platform=vcs&githubURL=https%3A%2F%2Fgithub.com%2Fridge-runner%2FAtari&file=excersizes.dasm).

[PIKUMA.com](https://www.pikuma.com) is the homepage of Gustavo Pezzi, the course instructor that I'm following for these exercizes. You can find his Atari course for cheap on Udemy.com. His other courses are also very good, but more expensive. Those are on Pikuma.com. I've only taken his Atari Udemy Course thus far, so can't comment on the others from firsthand experience.
