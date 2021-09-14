+++
author = "Gamey"
title = "Browsers on the Pinephone."
date = "2021-04-25"
description = "A list of most current Browsers for the Pinephone."
tags = [
    "Pinephone", "ArchLinux", "Browsers",
]

+++

Today I thought I would do a full rewrite of my Pinephone browsers post because it's obviously a important peace on every phone specially with a limited app selection. I hope this is helpful to some of you and as always all my testing is done on my 2GB Pinephone with DanctNIX Arch Linux.

## Firefox:
The browser I use by far the most and one that worked decent since I got my device. The UI isn't perfect since it's essentially the desktop one with a few tricks applied via the mobile config package but it's definitely usable. Firefox is decently fast, scales well enough to be usable and generally is still the browser that works best for me. Some issues are that Addons can't scale so while I can and do use UBlock I can't use it's UI, the removal of SSB/PWA features broke my Matrix setup over the minimal web UI Hydrogen, videos work but I can't get back out of fullscreen when I toggled it on once and some settings don't work because of scaling issues (mostly the ones that open a small window). If you use a Pinephone FF is most likely your default browser and it deserves that in my opinion but ultimately a mobile UI would be really cool to have.

| ![](https://gateway.pinata.cloud/ipfs/QmXmq8N1otd7EWJDhZH5gStUVazLFM8t4aADLqd1qa1kJw/20210422_09h56m38s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXmq8N1otd7EWJDhZH5gStUVazLFM8t4aADLqd1qa1kJw/20210422_09h57m03s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXmq8N1otd7EWJDhZH5gStUVazLFM8t4aADLqd1qa1kJw/20210422_09h57m29s_grim.png) |
|---|---|---|

## Angelfish:
The default Plasma mobile browser and only "mobile first" browser for the Pinephone. It uses Plasmas awesome mobile UI frameworks as a base (Qt based), runs on QtWebEngine (a fork of Googles Blink) and implements Braves Rust adblocker which I consider to be one of the best out there. I have really high hopes for the future of Angelfish but currently it still crashes from time to time, like FF can't go out of fullscreen, lacks a lot of features I would really like to have, has some issues to scale bigger and smaller when the keyboard is in use (probably framework related since it's a issue on all Plasma mobile apps when running them in Phosh), no addon support yet, doesn't support PWAs (progressive web apps) in Phosh yet and can't trigger Squeekboard (the Phosh keyboard). I currently use it as second browser next to FF and view it as a great option but it still has a long way to go.
**Extra:** You can delete cookies in Angelfish with the following commands:
``rm ~/.local/share/KDE/angelfish/QtWebEngine/DefaultProfile/Cookies``
``rm ~/.local/share/KDE/angelfish/QtWebEngine/DefaultProfile/Cookies-journal``

| ![](https://gateway.pinata.cloud/ipfs/QmQDBxW69mBELsmPnf1sexiDDL9PHM4qAmbHwC46yo49Nh/20210421_23h04m13s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmQDBxW69mBELsmPnf1sexiDDL9PHM4qAmbHwC46yo49Nh/20210421_23h04m30s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmQDBxW69mBELsmPnf1sexiDDL9PHM4qAmbHwC46yo49Nh/20210421_23h05m01s_grim.png) |
|---|---|---|
| ![](https://gateway.pinata.cloud/ipfs/QmQDBxW69mBELsmPnf1sexiDDL9PHM4qAmbHwC46yo49Nh/20210421_23h05m16s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmQDBxW69mBELsmPnf1sexiDDL9PHM4qAmbHwC46yo49Nh/20210421_23h05m36s_grim.png) | ![]() |

## Chromium/Ungoogled Chromium:
Yea ik it's Googles browser and many of us (including me) refuse to use it at least as main browser but as the only browser I know of that can get out of fullscreen when watching videos I currently use it for exactly that. Negatives about it include a UI that scales a bit worse then the FF one, No well working Wayland support so it currently uses XWayland to translate all calls which has a impact on performance and to balance that out the Pinephone renders it at reduced resolution, there is a keyboard glitch that blocks your from typing a "@" (you can just copy paste), I haven't spend much time exploring but I wasn't able to get Addons installed, it uses the Blink rendering engine which is the fastest and most feature rich but forms a total monopoly on most platforms and the hamburger menu can be really tricky to navigate. Over all I will try to avoid this browser as much as possible but currently have a good usecase for it on my Pinephone.
**Extra:** If you want to try Ozone (Wayland compatible Chromium) yourself you can do so using the following flags. ``--enable-features=UseOzoneProject --ozone-platform=wayland``

| ![](https://gateway.pinata.cloud/ipfs/QmST4vd1GZk4XKRV8Cs7cFF5WBfAdpzseNBQe9R56VKwds/20210421_23h06m53s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmST4vd1GZk4XKRV8Cs7cFF5WBfAdpzseNBQe9R56VKwds/20210421_23h07m07s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmST4vd1GZk4XKRV8Cs7cFF5WBfAdpzseNBQe9R56VKwds/20210421_23h07m34s_grim.png) |
|---|---|---|

## Castor:
Not actually a "webbrowser" because instead of the world wide web it's build on Gemini a alternative, minimal and text only protocol and as far as I understand a attempt to modernise Gopher (a competitor of www in the early days of the internet). I really like CSS, images and even light weight scripts so this isn't really something I will use but it's a really interesting project and I love that we have a browser for it that works on the Pinephone. Obviously Gemini has no way to build mobile friendly websites and there generally aren't many Gemini/Gopher websites out there but it's a fun project and you should at least try it out once if you are a true FOSS nerd :D

(Pinata which I usually use to upload images apparently removed folders so I have to search a alternative before adding screenshots here.)

## Qutebrowser:
I had to include this QtWebEngine/QtWebKit based browser because it's terminal driven vim like UI and input method makes it the only feature rich option in which all features beside of website scaling just work (shouldn't be more then changing the user agent string tho). It can be a bit annoying to use on a mobile device but works really well even with the default keybindings (requires the terminal Keyboard layout).

| ![](https://gateway.pinata.cloud/ipfs/QmWicYQTNbqL8SSm1mjKXG6eDGUeA7YTN3NwfmX4BeXT4F/20210422_10h15m26s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmWicYQTNbqL8SSm1mjKXG6eDGUeA7YTN3NwfmX4BeXT4F/20210422_10h16m09s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmWicYQTNbqL8SSm1mjKXG6eDGUeA7YTN3NwfmX4BeXT4F/20210422_10h16m28s_grim.png) |
|---|---|---|

## Others:
Here I list all the browsers I can't feature in full length because it would make very little sense to me and just extend the post to a ridiculous length. Also most of them are desktop only browsers some with awful UI for mobile devices but I still wanted to feature them here just because they work.

- **LibreWolf:** My favorite desktop browser and essentially just Firefox from a different source and with far better default settings. It works but there is no mobile config for it like for Firefox which makes it kind of useless on the Pinephone.
- **Dillo:** A extremely light weight browser that lacks many features the modern web includes. I honestly can't see much of a use case for this no matter what platform but I guess it's for a different audiance.
- **Liri Browser:** Part of the Liri app collection which uses Googles Material design over the UI toolkit Fluid and based on Chromium. I am not a big fan of Material design but many are so these apps are a really cool idea and I wish them luck. Once again a case of not that great scaling and just in general nothing for me.
- **Epiphany/Gnome Web:** The default Gnome browser based on GTK and WebKitGTK and one of the only cases of actually great scaling via Libhandy (a library to help GTK to scale). If there wasn't the problem of HW acceleration issues with WebKit (GPU based acceleration doesn't work) Epiphany would probably be the best mobile GNU/Linux browser. In short it's currently so slow and laggy I would highly recommend to just stay away (not even worth a try in my optinion)
- **Midori:** A GTK and WebKitGTK based "minimal" browser which scales somewhat okay but again using WebKit. It has some more small bugs and issues but it's generally usable if you disable JS or just wait a very long time for each site to load.
- **Vivaldi:** I have no idea why someone from this "community" would even touch a closed source browser when we have so many open source versions but it works. Like Chromium it also uses x11 so XWayland only and the UI is just awful for mobile devices. I have to note that I haven't done basically any testing and uninstalled it again right away.
- **Falkon:** The Plasma desktop browser and based on QT and QtWebEngine. I am so not a fan of this browser and it doesn't scale specially well ether. Additionally it won't ever scale because the Plasma mobile team decided to instead make Angelfish (a great choice in my opinion) but still another working browser.
- **QtWebBrowser** A touch optimized browser from the QT team for some kind of tablet like devices. It works but the UI components are far to big which forces you to turn the screen for every search.

## Sources:
First of all a huge thanks to the people who helped me find info on Mastodon and with that out of the way here are the sources.
https://forum.pine64.org/showthread.php?tid=13669
https://linmobapps.frama.io
https://fosstodon.org/@gamey/106104815889084213
