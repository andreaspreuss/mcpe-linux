# mcpe-linux
This script automatically downloads, sets up and install Minecraft: Bedrock Edition on your Debian-based Linux device!
# Disclaimer
We (SupDroid Studio) have written this script, but we did not create the Minecraft: Bedrock Edition Linux port. It's source is available at https://github.com/minecraft-linux/mcpelauncher-manifest/wiki. In short, this script automatically executes the instructions found at https://mcpelauncher.readthedocs.io/en/latest/source_build/index.html, instead of you needing to manually run all the commands. You may need to manually run the commands if you are not on a Debian-based distro, or if you are not on Ubuntu 18.04+ or equivalent. More about that below.
# Version naming scheme?
It's not that original, we just choose an animal beginning with each letter going through the alphabet. Read all the versions in the changelog.md file!
# Compatibility
The script will work on all Debian-based distros that run the equivalent of Ubuntu 18.04/Debian 10 or above. If your distro or version is not supported, please manually build from https://mcpelauncher.readthedocs.io/en/latest/source_build/index.html.
# Instructions
1. Open a terminal tab.
2. (Skip to step 4 if you already have the script downloaded) Run `wget https://github.com/SupDroidStudio/mcpe-linux/raw/master/mcpe-linux.zip`.
3. Unzip should be preinstalled on your system, but if it isn't, run `sudo apt install unzip`. Now run `unzip mcpe-linux.zip`.
4. Run `sudo bash mcpe-linux-setup.sh`. Ensure you are running it as root (sudo), or some parts will fail and MCPE will be only half-installed on your machine - not very helpful!
5. Assuming everything went well, you should find the Minecraft launcher in your apps list.
6. Sign in with Google to be able to download Minecraft and play.
**Please See Below If You Don't Own Minecraft On Google Play!**
# Import custom resource/behaviour packs
1. If the target pack is in .MCPACK format, please rename the extension to *.ZIP*.
2. Extract the ZIP to a location of your choice.
3. Copy the folder with extracted ZIP to `~/.local/share/mcpelauncher/games/com.mojang/resource_packs` if resource pack or `~/.local/share/mcpelauncher/games/com.mojang/behaviour_packs` if behaviour pack. *NOTE: If you need the pack to be imported as a global resource, then also copy to `~/.local/share/mcpelauncher/premium_cache/resource_packs`*.
4. Restart Minecraft and now your pack is imported!
# Removal
Run `sudo bash mcpe-linux-remove.sh`. This will unistall Minecraft and all its components from /usr/local. It will also remove the folders created in your home directory, however it won't remove the core dependencies, as some of them were already needed by the system and it is impossible to determine which ones were and were not. You can manually remove dependencies if you know which ones are safe to remove, however it may harm your system, so do so at your own risk!
# Help / Support
If you are stuck or are facing an issue, contact us at supdroid@mail.uk, or write an issue from the issues tab. The script has been tested and should work without fail, providing your device is supported.
# I don't own Minecraft on Google Play!
That's alright! Please do the following to play Minecraft without purchasing it:
1. Sign in with Google Play. Even if you don't own Minecraft, you must sign in for this to work.
2. Go to http://bit.ly/mcpe-linux-zip. Read the "READ THIS FIRST!!!" text file - it contains instructions on how to download and install Minecraft. At this link, you can download the latest release of Minecraft in a ZIP file.
# There is no sound!
Install sound drivers - `sudo apt install libpulse0 libpulse0:i386` (this will install both amd64 and i386 varients which are both required). The latest version of the script "1.9 - Jaguar" (see: changelog.md), the sound drivers are installed as part of the "Core Dependencies".
# Arch Linux support?
Support for Arch Linux is currently **under development**. There is no ETA for this, however we hope to have it finalized very soon!
