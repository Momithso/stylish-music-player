# Rainmeter | Stylish Music Player (Spotify working!)
Updated Version of Stylish Music Player 1.1.3 made by Vancruz06 and edited by Momithso

## Requirements

 - [Rainmeter](https://www.rainmeter.net/) (>=4.5.11)
 - Windows
 - [Spotify Desktop Version](https://www.spotify.com/de/download/windows/)

## Installing
### 1. Spicetify
This will install on your machine which we need to get access to Spotify. With this program you can also modify the design of Spotify, add new features and more but for our purposes, we will just enable the **[WebNowPlaying](https://github.com/tjhrulz/WebNowPlaying)** extension and disable all customizations.

These Powershell commands will install Spicetify on your computer which you need to get access to Spotify's Metadata like Song Title, Cover etc.
You can also change the Design of Spotify with this program but this is not what we directly want, we'll only need the plugin that comes with it ([WebNowPlaying](https://github.com/tjhrulz/WebNowPlaying)).


Paste this in your Windows Powershell - Recommended

    Invoke-WebRequest -UseBasicParsing "https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install.ps1" | Invoke-Expression
    spicetify
    spicetify config extensions webnowplaying.js
    spicetify config inject_css 0 replace_colors 0
    spicetify backup apply

If you have errors try this

    Invoke-WebRequest -UseBasicParsing "https://raw.githubusercontent.com/khanhas/spicetify-cli/master/install_curl.ps1" | Invoke-Expression
    spicetify
    spicetify config extensions webnowplaying.js
    spicetify config inject_css 0 replace_colors 0
    spicetify backup apply

### 2. Downloading latest Git Version
Download the skin and activate it on Rainmeter. It should work now!
