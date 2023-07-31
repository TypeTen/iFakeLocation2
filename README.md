# iFakeLocation functionality+

This is a fork of the original iFakeLocation that I plan to update with the ability to connect to your phone over wi-fi, but I now have a child so I'll stick to what I can do quick and fast: FE Web Dev.
The only differences in this repo to the original is the .html and .css files relating to the Front End you'll be interacting with as a user. Hence, I'm not going to recompile master131's work and take any clicks from them. Go to their repo to get the app, come to mine to get the extended functionality such as:

- [x] Route plotting and walking
- [x] Random walking starting from a chosen point
- [x] Controllable move speed and update rate
- [ ] Saving and loading routes
- [ ] Connecting to mobile device over wi-fi

In the new front end I've updated the About modal with some more info for you that I'll repeat here so that you have no excuses.

I didn't write this for anyone but myself. I didn't want to pay some shmuck with a crap track record (not gonna throw shade here, but the app's antonym name is youYourLandline and others that look like it are all rebranded apps by the same gonk) for an auto walker with really basic functionality, so I just used Smartlad master131's cracking work to laboriously teleport up and down my road to catch monsters of the pocket variety. Upon getting fed up of that, I looked into how it was moving me and found it controlled by js, so I just added in some functionality I'd like to have. I then began working on refactoring all the code and got burned out so I scrapped most of it and now it's your spaghetti to adopt.

Don't *consider* this a warning, it **is** a warning. I couldn't give any less of a shit what you consider it. I will take no responsibility for your actions and will continue not to.
# If you use this for Walking Games, you stand the chance of being banned. Like with all tools. The only difference is, this is free and still has the main feature you need: an auto walker that allows you to plot a route without leaving your computer/laptop.

### Route Plotting

* Toggle the 'Off' button in the Route Plotting section to the right of the map, the button will highlight
* Double click in multiple places on the map
* Each double click will add a route destination and the last point will circle back to the first point placed
* Once your route is entirely mapped out, click the 'Start Walking Route' button under the map
**THE ROUTE PLOTTING IS QUITE HEAVY ON THE JS, MAKE SURE YOU'RE ZOOMED IN ON YOUR CHOSEN LOCATION AND NOT TRYING TO WALK ACROSS THE ENTIRETY OF A CONTINENT. I HAVE WROTE NO SAFETIES INTO MY ADDITIONS TO STOP YOU FROM NUKING YOUR BROWSER.**

There is no pause/play feature. If you want to stop at a place, then plot a route there then click 'Stop Walking Route' when you get to it; clicking the button will move the user icon back to the first plot point, but it won't actually move your mobile device back so don't worry. This is a quirk I've literally just noticed as I wrote this, so it might be fixed one day when I get back around to this.

### Potter About

* Toggling this option on will just walk your GPS around randomly in a short range near to your selected area.
* Each 'walk' is completely random and so you could end up being exactly where you started after an hour, or you could be an hours walk from your position in exactly one direction.

### Use in Walking Games

I wrote the additions to iFakeLocation for this; you're probably using it for this. These are some tips to help you suck less at being a cheater:

* If you want to avoid bans in these types of games, set your starting point to your phsyical location.
* If you use it to teleport, make sure your Walking Game is off for an adequate amount of time for you to get that far were you to travel to it from the last place you played the game logged in at.
* **Basically: don't actually teleport as far as the game is concerned.**
* If you want to move faster than 5m/s then you'll probably be in for a bad time. The move speed is set to a default of 3 and a bit metre/s, which is still a really good clip.
* Smoothing is just how many times the app will send a GPS spoof to your device. 2 = twice per second and twice per your metres/s setting.
<sub>If you really want it tremendously smooth, go for it, but keep in mind it's going to take longer to generate each path.</sub>
* You're already cheating, have some patience.

### Potter About

* Toggling this option on will just walk your GPS around randomly in a short range near to your selected area.
* Each 'walk' is completely random and so you could end up being exactly where you started after an hour, or you could be an hours walk from your position in exactly one direction.

## How to install my extra features:

* [Go to the main repo page and download your selected version of the app and unzip it](https://github.com/master131/iFakeLocation/releases)
* Then grab the [release in my repo](https://github.com/TypeTen/iFakeLocation2/releases) (the files aren't OS specific like master131's), unzip the folder, and drop it into the iFakeLocation download you got from the first link.
* That should prompt you to replace the files, replace all of them. Don't make copies, don't skip, just replace all. All the code is in this repo, scrutinise it if you're worried I'm some dodgy geezer.
* Launch iFakeLocation and you'll have the extended functionality

Done. If it's broken, doesn't work, or hasn't changed anything, then either:
* you've done it wrong (highest likelyhood)
* master131's updated his repo and made some changes that means my code no longer does the right stuff (good likelyhood)
<sub>if you suspect that is the case, this was written on [version 1.70](https://github.com/master131/iFakeLocation/releases/tag/v1.7.0) of master131's code, use that as your base</sub>
* I've done something wrong (also probably a really good likelyhood, but please exhaust the other options before you message me or submit an issue)

While we're on the topic of issues and merge requests, I don't know how often I'll check this repo but feel free make pull requests with fixes or whatever you want. Also feel free to make requests. I'll probably ignore them, though, so don't waste too much of your time making them.

If there's any butchered prose or language in this readme, blame my 3 month old for allowing me the kingly 3 hours of sleep I've had each night this week.

# Original iFakeLocation readme as of 1.70

![](https://i.imgur.com/ELFifkA.png)

## Requirements:
### Windows:
* .NET Framework 4.5 or newer (pre-installed on Windows 8 & Windows 10)  
https://dotnet.microsoft.com/download/dotnet-framework

* iTunes (Microsoft Store version or Win32/Win64 is fine)  
https://www.apple.com/itunes/download/
  
* Visual C++ Redistributable for Visual Studio 2015  
https://www.microsoft.com/en-us/download/details.aspx?id=48145
  
### Mac OSX:
* .NET 6.0 Runtime (macOS 10.13 "High Sierra" or newer) - **make sure it's the x64 version, even if you have an M1/M2 Mac**
https://dotnet.microsoft.com/en-us/download/dotnet/6.0

### Ubuntu:
* .NET 6.0 Runtime (only dotnet-runtime-6.0 package is required)  
https://docs.microsoft.com/en-gb/dotnet/core/install/linux-ubuntu
  
## Download:
See the [Releases](https://github.com/master131/iFakeLocation/releases) page.

## Running:
### Windows:
Run the executable called iFakeLocation.exe.

### Mac OSX
Open the DMG and drag the application to the Desktop or Applications folder. Double-click to run the app.

### Ubuntu
```
chmod +x ./iFakeLocation
./iFakeLocation

# or

dotnet ./iFakeLocation.dll
```

## How to make it work on iOS X.X?

If for whatever reason the automatic developer image retrieval doesn't work, you can manually download them to be used in iFakeLocation.
Create a folder called "DeveloperImages" (next to the iFakeLocation executable) and inside that folder make a folder for the iOS version you are running (eg. "12.4", "13.0", etc). Download the matching developer images from the following Github repo and unzip the DeveloperDiskImage.dmg + DeveloperDiskImage.dmg.signature file into the folder you created.

https://github.com/haikieu/xcode-developer-disk-image-all-platforms/tree/master/DiskImages/iPhoneOS.platform/DeviceSupport

## How to use:

* Connect your iDevice to your computer. Click the "Refresh" button and select your iDevice from the list.

* Enter the desired location (ie. Sydney NSW) in the box and hit "Search" (try to be
  more specific if you are getting strange results).

  You can also manually place a pin on the map by double-clicking anywhere.

* Click "Set Fake Location". If it is the first time doing this the tool
  needs to download some files to enable Developer Mode on your iDevice.

* Confirm your fake location using Apple Maps, Google Maps, etc. To stop the fake location,
  click "Stop Fake Location". If your device is still stuck at the faked location
  turn Location Services off and on in Settings > Privacy.

* Your device will also have a Developer menu now shown in Settings. You can get rid of it 
  by restarting your iDevice.

## Help:
Q: My device doesn't show up on the list?  
A: Ensure that it is plugged in, you have trusted your PC and that the device is visible on iTunes.

Q: Help, it says that it can't mount the image or some other generic error?  
A: Make sure your iDevice is trusted with the PC/Mac and if everything you've tried is not working, usually a reboot of your device will fix the issue

Q: Unable to load shared library 'imobiledevice' or one of its dependencies
A: set environment variable `DYLD_LIBRARY_PATH` to the folder which has the `libimobiledevice` files, and run the project with specified framework and runtime, e.g.
```shell
export DYLD_LIBRARY_PATH=$HOME/iFakeLocation/iFakeLocation/bin/Debug/net6.0/runtimes/osx-x64/native
dotnet run --project ./iFakeLocation/iFakeLocation.csproj --framework net6.0 --runtime osx-x64
```

## Special Thanks:
* [idevicelocation by JonGabilondoAngulo](https://github.com/JonGabilondoAngulo/idevicelocation)
* [Xcode-iOS-Developer-Disk-Image by xushuduo](https://github.com/xushuduo/Xcode-iOS-Developer-Disk-Image/)
