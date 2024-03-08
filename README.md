# Native Ethernet Library For Teensy 4.1

> **Notes on the SO-ETS Fork:**
> 
> This fork of the upstream NativeEthernet library is better at handling a failure to connect to a broker.  Add it to
> your library list using Sketch -> Include library -> Add .ZIP Library... in the Arduino IDE and selecting the folder
> where this README file is located.  This will *copy* the library files to the ArduinoIDE user library area (which
> you can find under File -> Preferences -> Sketchbook location).  Any updates to your local clone of the repository
> *must be copied manually* to the user library area.
> 
> After adding this library the Arduino IDE will use this SO-ETS fork for compiling code instead of the
> original NativeEthernet library that came with the Teensy download of the Arduino IDE.  You may see occasional
> warnings when building the code that two versions of the library were found and indicating which one was used.

Teensy 4.1 is automatically configured for Ethernet use.
This library uses my FNET fork and is a required download.
https://github.com/vjmuzik/FNET


Just change <Ethernet.h> to <NativeEthernet.h> to use this library and the rest is taken care of.
The API is a direct replacement for the normal Ethernet.h library aside from sketches that use direct calls to w5100.h

I've done quite a bit of testing to ensure compatibility as much as possible, but if you find any issues please report them.


http://www.pjrc.com/teensy/td_libs_Ethernet.html
