# mcpe-linux
This script automatically downloads, sets up and install Minecraft: Bedrock Edition on your Debian-based Linux device!
# Disclaimer
We (SupDroid Studio) have written this script, but we did not create the Minecraft: Bedrock Edition Linux port. It's source is available at https://github.com/minecraft-linux/mcpelauncher-manifest/wiki. In short, this script automatically executes the instructions found at https://mcpelauncher.readthedocs.io/en/latest/source_build/index.html, instead of you needing to manually run all the commands. You may need to manually run the commands if you are not on a Debian-based distro, or if you are not on Ubuntu 18.04+ or equivalent. More about that below.
# Compatibility
The script will work on all Debian-based distros that run the equivalent of Ubuntu 18.04 or above. If your distro or version is not supported, please manually build from https://mcpelauncher.readthedocs.io/en/latest/source_build/index.html.
# Instructions
1. Open a terminal tab.
2. (Skip to step 4 if you already have the script downloaded) Run `wget https://github.com/SupDroidStudio/mcpe-linux/raw/master/mcpe-linux.zip`.
3. Unzip should be preinstalled on your system, but if it isn't, run `sudo apt install unzip`. Now run `unzip mcpe-linux.zip`.
4. Run `sudo bash mcpe-linux-setup.sh`. Ensure you are running it as root (sudo), or some parts will fail and MCPE will be only half-installed on your machine - not very helpful!
5. Assuming everything went well, you should find the Minecraft launcher in your apps list.
6. Sign in with Google to verify that you own Minecraft on Google Play. If you don't own Minecraft or don't want to sign in, you may use an APK file instead.
7. Now you should be able to download and play Minecraft from there!
# Removal
Run `sudo bash mcpe-linux-remove.sh`. This will unistall Minecraft and all its components from /usr/local. It will also remove the folders created in your home directory, however it won't remove the core dependencies, as some of them were already needed by the system and it is impossible to determine which ones were and were not. You can manually remove dependencies if you know which ones are safe to remove, however it may harm your system, so do so at your own risk!
# Help / Support
If you are stuck or are facing an issue, contact us at supdroid@mail.uk, or write an issue from the issues tab. The script has been tested and should work without fail, providing your device is supported.
