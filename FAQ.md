# Frequently Asked Questions
Here you will find answers to commonly asked questions regarding the script / the game.
# What distros are supported?
There are many distros out there, so it's impossible to list every supported distro, however compatible distros will meet these requirements:
- Uses `apt` or `apt-get` for package management.
- Equivalent of Ubuntu 18.04 (Bionic) or higher.
- Equivalent of Debian 10 (Buster) or higher.
- 64-bit OS.
# What are the system requirements?
The script requires at least 1GB of available RAM to be able to run without crashing your PC, and Minecraft will need at least 2GB of RAM to be able to run without lag (although 4GB+ is advised) (swap area does not count). The installation takes about 2GB of disk space, not including game data, and cannot be installed to an external disk. Having at least 4GB of free disk space is recommended. Unlike the Java edition, Bedrock edition is very friendly towards lower-spec machines.
# Why am I not hearing any sound?
You need to install the audio drivers - `sudo apt install libpulse libpulse:i386`. *NOTE: As of version 1.9 "Jaguar", audio drivers are installed by default when running the installation script.*
# I don't own Minecraft on Google Play. How can I play?
Head to http://bit.ly/mcpe-linux-zip and read the "READ THIS FIRST!!!" file - it contains instructions.
# Why I am hearing sound, but not hearing music?
Music is not present by default. Please go to the Marketplace, scroll to the bottom and download "Music" pack. After doing this, you will hear music in the menus and in game.
# The GUI scale is tiny!
Yep, this happens if you maximise the window without going fully fullscreen. To resolve this after maximising, go to Settings > Video and change the Splitscreen dropdown (it doesn't matter what you change it to, as long as you change it, since this will refresh the display). Alternatively you could try messing with the "GUI scale" slider, but that will most likely just cause more problems down the road.
# The game crashes on exit!
This is not an error. By default, when you close the game, the launcher does not expect it, therefore it thinks that the game has crashed. Just ignore the message.
# My question is not answered here!
That's fine! If you need support, simply drop us an email at supdroid@mail.uk and we will get back to you as soon as we can to resolve your issue.
