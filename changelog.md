# 2.1 - "Lemur"
This update fixes some bugs in the installation script, and changes the installation cache directory to `~/.mcpe-linux-tmp` in order to clean up the home directory during installation and prevent accidental removal during installation and/or corruption of the installation files.
# 2.0.1 - "Koala"
Minor amendments made to the scripts.
# 2.0 - "Koala"
- The main removal script no longer removes data from `~/.local/share`. Another removal script labelled `mcpe-linux-remove-data.sh` is now present to remove data. This is useful for people who only want to reinstall and/or do not want to lose data.
- Now you can cancel with CTRL+C instead of needing to kill the process!
# 1.9 - "Jaguar"
Fixed no sound issue on some devices; the script now installs audio dependencies. If you do not wish to re-run the entire script, you can manually install the dependenices with `sudo apt install libpulse0 libpulse0:i386`.
# 1.8 - "Iguana"
Minor amendment made to the end message strings.
# 1.7 - "Hedgehog"
Better support for i386 packages on Debian. You are now far less likely to experience package not found errors on Debian now.
# 1.6 - "Giraffe"
After the "Install core dependencies" step, the script will pause for 5 seconds to give you a chance to kill it if the step fails.
# 1.5 - "Frog"
The install script now automatically removes the installation files in /home after it's finished. This includes msa, mcpelauncher and mcpelauncher-ui.
# 1.4 - "Elephant"
The removal script now removes data in ~/.local/share.
# 1.3 - "Deer"
The removal script now removes the folders created in /home.
# 1.2 - "Chameleon"
Amendment made to the removal script.
# 1.1 - "Badger"
Fixed a syntax error in the removal script.
# 1.0 - "Aligator"
The official project launch!
