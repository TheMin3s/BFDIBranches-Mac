Heyo there!
Welcome to the BFDI: Branches installation guide for Mac!
NOTE THAT THIS IS UNOFFICIAL!! Made by @themines. See the actual download page at https://teambranches.itch.io/bfdi-branches

Requirements
- MacOS Monterey (12.0.0) and newer (MacOS Sequoia (15 beta) support not tested)
- Intel x86 or Apple Silicon CPUs
- Internet connection (this does not come with any of the files pre-installed, which is why this is so small)

Install

A video tutorial can be found at https://objectshows.net/bfdibranchesmacos.mp4.
BFDI: Branches will be automatically installed, so you’ll recieve the latest version upon downloading.

To install, run the install executable inside this folder. This will result in the terminal app opening. This is expected. You will be prompted to install command line developer tools if you haven’t already, which you should accept. After this, the terminal app will install everything required and put the “BFDIBranches” folder (with the game inside) in the Macintosh HD/Users/<your username>/ folder. You may be asked to input your password at certain points in the installation. For example, for me it would be located in Macintosh HD/Users/themines/.

Scroll down for more info and uninstallation instructions









This guide installs the following applications:

- Homebrew (brew) - https://brew.sh/ -  Package (or app) manager that we’ll use to install what we need to run the game. This makes it so you don’t have to do anything on your end. This will not affect any other apps you have on your computer, and uninstalling the app can be done through the guide below or with the “uninstall-brew.sh” file in this folder. If you already have homebrew installed, the installer will do nothing to the already existing installation.

- XCode Command Line Tools - https://developer.apple.com/xcode/resources/ - Homebrew requires XCode’s command line tools to function. This is an app provided by apple and can be removed after the installation with the “uninstall-xcode.sh” script. To install the app we run the xcode-select command which we simply use to trigger the installation prompt.

- Wine, WineTricks, XQuartz - https://www.winehq.org/ - Apps that “translate” windows code to mac code. You will need to keep the apps on your computer. While installing XQuartz, it will add a background item you can remove in Settings > General > Login Items > XQuartz. BFDI: Branches will still work.

- BFDI: Branches - https://teambranches.itch.io/bfdi-branches - what, we did you think we wouldn’t install the actual game? what are you using this guide for then?
Branches will be installed through a mirror due to itch.io having constantly changing download links, which implementing is beyond my scope of coding. If the version is outdated it should update upon starting or upon second startup.

Uninstallation

BFDI: Branches
Delete the “BFDIBranches” folder from your computer.
Other stuff we downloaded
Homebrew

Uninstalling will not break BFDI: Branches, though if you update your MacOS you may need this to get the game to continue working if there were major changes.
Homebrew (or otherwise known as brew) can be uninstalled through the “uninstall-brew” executable in this folder or with the command
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall.sh)"
in Terminal.
Once you’re done, you can check that brew has been removed with
brew --version

Wine, WineTricks, & XQuartz
Uninstalling WILL BREAK BFDI: Branches.
These can all be uninstalled with the “uninstall-full” executable in this folder (will not remove homebrew) or with the commands
brew uninstall wine-stable
brew uninstall winetricks
brew uninstall xquartz

XCode Command Line Tools
Uninstalling will not break BFDI: Branches, but will break Homebrew which is required for updates.
XCode’s command line tools can be uninstalled through the “uninstall-xcode” file or by deleting the folder located in /Macintosh HD/Library/Developer/ titled “CommandLineTools
