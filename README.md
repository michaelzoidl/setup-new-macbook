# Setup my new macbook
In the next days my new macbook will arrive, this is the software i've to install before i can start working on stuff.

### Apps
|      | Name                            | Description           | Website                                                                                                      | Homebrew Cask
| ---- | ------------------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------ | ----------------------------------
| ![](./resources/logos/atom.png)        | Atom                  | Code Editor                  | [atom.io](https://atom.io)                                                    | `atom`
| ![](./resources/logos/iterm.png)       | iTerm2                | Terminal emulator            | [iterm2.com](https://www.iterm2.com/)                                         | `iterm2`
| ![](./resources/logos/docker.png)      | Docker                | Virtual containers           | [docker.com](https://docker.com)                                              | `docker`
| ![](./resources/logos/kitematic.png)   | Kitematic             | UI/Toobox for docker         | [kitematic.com](https://kitematic.com/)                                       | `kitematic`
| ![](./resources/logos/tower.png)       | Tower                 | Git UI client                | [git-tower.com](https://www.git-tower.com/mac/)                               | `tower`
| ![](./resources/logos/bartender.png)   | Bartender             | Organize mac menu apps       | [macbartender.com](https://www.macbartender.com/)                             | `bartender`
| ![](./resources/logos/dropshare.png)   | Dropshare             | Private file sharing         | [getdropsha.re](https://getdropsha.re/)                                       | `dropshare`
| ![](./resources/logos/feeds.png)       | Feeds                 | RSS Reader for menu bar      | [feedsapp.com](http://www.feedsapp.com/)                                      | `feeds`
| ![](./resources/logos/fantastical.png) | Fantastical           | Calendar app                 | [flexbits.com/fantastical](https://flexibits.com/fantastical)                 | `fantastical`
| ![](./resources/logos/alfred.png)      | Alfred                | Search bar on steroids       | [alfredapp.com](https://www.alfredapp.com/)                                   | `alfred`
| ![](./resources/logos/sizeup.png)      | Size-Up               | Window manager               | [irradiatedsoftware.com/sizeup](http://www.irradiatedsoftware.com/sizeup/)    | `sizeup`
| ![](./resources/logos/resilio.png)     | Resilio Sync          | File synchronization         | [resilio.com](https://www.resilio.com/)                                       | `resilio-sync`
| ![](./resources/logos/1password.png)   | 1Password             | Password Manager             | [1password.com](https://1password.com/)                                       | `1password`
| ![](./resources/logos/spotify.png)     | Spotify               | Music                        | [spotify.com](https://www.spotify.com/)                                       | `spotify`
| ![](./resources/logos/chrome.png)      | Chrome                | Browser                      | [chrome.com](https://www.chrome.com/)                                         | `googlechrome`
| ![](./resources/logos/office.png)      | Microsoft Office      | Word, Excel etc..            | [office.com](https://www.office.com/)                                         | `microsoft-office`
| ![](./resources/logos/slack.png)       | Slack                 | Team Messenger               | [slack.com](https://www.slack.com/)                                           | `slack`
| ![](./resources/logos/postico.png)     | Postico               | Postgresql UI                | [eggeraps.at/postico](https://eggerapps.at/postico/)                          | `positco`
| ![](./resources/logos/vlc.png)         | VLC Player            | Video player                 | [vlc.com](https://www.vlc.com/)                                               | `vlc`
| ![](./resources/logos/adobe.png)       | Adobe Creative Cloud  | Photoshop, Illustrator etc.. | [adobe.com](https://www.adobe.com/)                                           | `adobe-creative-cloud`

### Package Manager
|      | Name                            | For        | Install
| ---- | ------------------------------- | ---------- | -------
|      | Homebrew                        | macOS      | `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
|      | npm                             | node       | _installed with node_
|      | yarn                            | node       | `brew install yarn`

### Version Manager
|      | Name                            | For        | Website
| ---- | ------------------------------- | ---------- | -------------------------------------------------------------------------------
|      | nvm                             | node       | `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash`

### Other
|      | Name                            | For        | Website
| ---- | ------------------------------- | ---------- | -------------------------------------------------------------------------------
|      | `htop`                          | Interactive process viewer       | [hisham.hm/htop](https://hisham.hm/htop/)
|      | `git`                           | Version control                  | [git-scm.com](https://git-scm.com/)

### Mac default changes
> Credits to [github/mathiasbynens/dotfiles](https://github.com/mathiasbynens/dotfiles)

```cl
# Set sidebar icon size to small
defaults write NSGlobalDomain NSTableViewDefaultSizeMode -int 1

# Restart automatically if the computer freezes
sudo systemsetup -setrestartfreeze on

# Never go into computer sleep mode
sudo systemsetup -setcomputersleep Off > /dev/null

# Disable smart quotes as they’re annoying when typing code
defaults write NSGlobalDomain NSAutomaticQuoteSubstitutionEnabled -bool false

# Increase sound quality for Bluetooth headphones/headsets
defaults write com.apple.BluetoothAudioAgent "Apple Bitpool Min (editable)" -int 40

# Finder: show hidden files by default
defaults write com.apple.finder AppleShowAllFiles -bool true

# Disable the warning when changing a file extension
defaults write com.apple.finder FXEnableExtensionChangeWarning -bool false

# Keep folders on top when sorting by name
defaults write com.apple.finder _FXSortFoldersFirst -bool true

## SizeUp.app default change:
# Don’t show the preferences window on next start
defaults write com.irradiatedsoftware.SizeUp ShowPrefsOnNextStart -bool false
```

### Macbook Specs
| Unit     | Spec
| -------- | -------------------------
| CPU      | 3,3 GHz Dual‑Core Intel Core i7, Turbo Boost til 3,6 GHz
| RAM      | 16 GB 2133 MHz
| GPU      | Intel Iris Graphics 550
| SSD      | 1 TB PCIe Basis
| Display  | 13"
