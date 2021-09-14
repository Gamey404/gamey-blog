+++
author = "Gamey"
title = "Plasma mobile apps in Phosh"
date = "2021-09-13"
description = "A short guide on how to properly use Kirigami apps in Phosh."
tags = [
"Pinephone", "Linux Phone", "Kirigami in Phosh",
]

+++

Today I will touch on a topic that I had issues with for a long time till I somewhat figured it out or I at least hope I did. It's not at all hard to do but you have to know what to do and since I found no proper guide or anything about this except for a environment variable [list](https://github.com/1peter10/linuxphone-tweaks/blob/main/etc/environment) by Peter from linmob I thought I would make my own. I want to clarify that I am not a expert and my experience with Plasma apps is fairly limited but I got the few things that I struggled with together and wrote a quick post that will hopefully help some of you out there! As always all of my testing is done on my 2GB Pinephone running DanctNIX Archlinux mobile and these are things I also did on my PostmarketOS install.

## Install dependencies:
First of all you have to make sure to install the required QT packages which you can for the most part do using the meta package ``plasma-framework``.

Now you also have to ensure that there is a valid qt theme and icon pack installed since these are interchangeable and therefor not in the dependency lists. For that you ether install your preferred theme or for the defaults ``breeze`` and ``breeze-icons``.

There are also certain runtime dependencies which are preinstalled in Plasma mobile and not required to build the app but totally required to run it in Phosh. These are very easy to miss for package maintainers so no matter the distro you are on you will probably run into a few of those. Ones that I found missing from a few packages are ``qt5-svg`` and ``qt5-wayland`` but there are a  few more specially QML and Kirigami related ones so if you find any please just comment them down below!

If you plan to build a Kirigami app in Phosh you probably want to just install the following dependencies: ``knotifications kdbusaddons kservice kcmutils purpose breeze breeze-icons plasma-framework cmake``. *There are obviously many more dependencies you may need but these should be a decent start*

## Set Environment variables:
Most Phosh distros miss a few environment variables that Kirigami apps need to run well on smartphones which you will have to set in ``/etc`` for a optimal experience.

- First of is ``QT_QPA_PLATFORM=wayland`` which ensures that the app uses Wayland and not XWayland which has a quite big performance impact and when using Wayland you probably also want to ensure it's window decorations are disabled or you will see a ugly frame around your app ``QT_WAYLAND_DISABLE_WINDOWDECORATION=1``.
- With that out of the way you have to make sure the theming is right to make them look roughly how they would in Plasma mobile and for that you need ``QT_QPA_SYSTEM_ICON_THEME=breeze`` which ensures the app uses Plasmas Breeze theme, ``QT_QUICK_CONTROLS_MOBILE=1`` which sets QTQuick to a mobile mode without which the scaling and position of certain elements isn't correct and ``QT_QUICK_CONTROLS_STYLE=org.kde.breeze`` which also ensures you use the Breeze theme.
- Last up Kirigami has a low performance mode to reduce lags on devices like the Pinephone which you can set with ``KIRIGAMI_LOWPOWER_HARDWARE=1``

To actually set these you just have to edit ``/etc/environment`` with a text editor like nano or Gedit and add all of them which should look like this when you are done:
```
#
# This file is parsed by pam_env module
#
# Syntax: simple "KEY=VAL" pairs on separate lines
#

QT_QPA_PLATFORM=wayland
QT_WAYLAND_DISABLE_WINDOWDECORATION=1
QT_QPA_SYSTEM_ICON_THEME=breeze
QT_QUICK_CONTROLS_MOBILE=1
QT_QUICK_CONTROLS_STYLE=org.kde.breeze
KIRIGAMI_LOWPOWER_HARDWARE=1
```

## Conclusion:
It can be a bit more complicated then just installing the App if you want a good experience but it's no witchcraft and there are some awesome QT apps so the effort definitely pays off! To end this I want to show a few screenshots of the amazing Kirigami app Kasts running in Phosh:

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/FhAVXgMky16N/D01gBVbHCxxnbzKKNNA6ydymdOjaeaUVQna71oTu.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/7qyi9aZ3srDj/1qoe5mkMXLUet1lynMoBlxdBMzIpHUc64BrN99q0.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/RGs10KIacwDp/hIJXRtA2e7vtLadqZqYVX0m8ZMGyPFroNHUj8aCn.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/VgolPETugqIC/xfn8rYtTXT1G7zogC6UONIzpQUv8TZ7hKr9SWq16.png) |
|-------|-------|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/brcDb1HVBWMA/pvrdnQ7e5PprSFIjM7KF19CrOqYQ4c6DaNGGSGcs.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/g6mz47Pq9rvl/ua5xUKHTiTydvZrHGjHKri0kWBO92TYx2YiTwrM7.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/CqCgNzD0EVHO/Yv63rBFExka2D1ILF6EffPoxiEJA9WErns8XWzxg.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/1672d1d81-1ab3fb/8a33KJo0gPCk/8Gq5VC6DJcy72jx3aZAACkZr6NHT8iQAvDfyEDN2.png) |

5 Awesome Pinephone apps: https://gamey.tech/posts/pinephone-5-amazing-linux-phone-apps-part-3/
Podcasts on the Pinephone: https://gamey.tech/posts/podcasts-on-the-pinephone./
