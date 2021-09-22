+++
author = "Gamey"
title = "PINEPHONE: 5 amazing Linux phone apps! Part 3"
date = "2021-09-05"
description = "List of awesome Pinephone apps"
tags = [
"Pinephone", "5 Apps Pinephone", "Linux Phone",
]

+++

Yet another post about five of the in my opinion best Pinephone apps but I promised to make a small series out of this so it's probably not a big surprise. You can find the last two posts linked down below if you are interested in more after this and as always the screenshots and testing where done on my 2GB Pinephone model in DanctNIX mobile Archlinux.
<!--more-->

## Fluffychat:
Fluffychat is a responsive Matrix client build with Flutter and replaced Hydrogen for me. It still suffers from Flutter related issues like a top bar that looks like a desktop Gnome one and really messes with the beautiful look of the app, lacks notification support on the Pinephone (that's actually WIP and not related to Flutter) and a really annoying issue with the onscreen keyboard which triggers every time you open the window switcher and basically forces you to restart Fluffychat before you can type properly again but aside of that it's a actually well working and good looking Matrix client. There also where some performance issues but those seem to have improved a ton since the last Flutter release and I really hope for future patches that fix the other issues. All in all it's the Matrix client I would currently recommend the most and the only reason it wasn't in my past "Matrix on the Pinephone" posts is that it simply didn't work back then.

**Notes:**
- I actually didn't use Fluffy on Arch yet those screenshots are from my PostmarketOS daily driver setup instead and there I just used the Flatpak where it's part of my daily driver setup.

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/1672d1d81-1ab3fb/7KZo37K5swuk/7Y1F4bU4pu1R1z7jCLwU2uDGj0NWRQaLhBBljbux.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/1672d1d81-1ab3fb/9xLMO3fpzIov/OeI4ZxBvL3N2znQ5sRtAAPaSU71uXeQXdLwryZmD.png) |
|-------|-------|
| ![](https://pixelfed.social/storage/m/_v2/245825453661753344/1672d1d81-1ab3fb/fWirm1AfJJyU/qIMqTcsan2HIuCZrOBMyD43edQ4jlK1MF6OOuzE4.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/1672d1d81-1ab3fb/tdwDPV3wswYD/subqwf5mGsq8LepVOuxB2eA43uSXHMZwN1qwenoJ.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.com/famedly/fluffychat/ |
| AUR | fluffychat fluffychat-git |
| Flathub | https://flathub.org/apps/details/im.fluffychat.Fluffychat |
| Mobian |  |
| PostmarketOS |  |

## Cawbird:
Cawbird is a adaptive Twitter client made with GTK. This app improved a LOT since I last tried it, back then it was a lagging mess and basically unusable and now it's almost smoother then Tootle. The only issue I have is that it seems to lack a notification tab which is really annoying to me. I assume it's probably intentional to change the social media experience but I wish it wasn't the case. Beside of that it's absolutely fantastic tho and while I am fairly new to Twitter and probably wouldn't be on there if it wasn't for this blog I think most people would really enjoy the experience Cawbird offers. If you are in need of a Pinephone friendly Twitter client this one definitely seems like a great choice!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/uP7o5XyaThzH/GwqvF5cf41fShuR8Pq74ErvQ2VCGU0kx3QrWxGTM.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/Rr7VoXGXzOsB/wwqnGO6Xi8DSJWewPInPNfu5YpYPiJz6XgF5VfvV.png) |
|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/lrjgxOudLI6N/Gjq0sDnGEXpOnRnlaBIzPIbPv1IWcgWqNGMuoJfH.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/7kRkvgqzdHvX/vCXAimBIo9RycePnVzregFxu4cBWIfWilrQX7Ae7.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/IBBoard/cawbird |
| AUR | cawbird (repo) cawbird-git |
| Flathub | https://flathub.org/apps/details/uk.co.ibboard.cawbird |
| Mobian | cawbird |
| PostmarketOS | cawbird |

## Gnome Weather:
Gnome Weather is a very minimal adaptive weather app that only covers the basics but that's actually exactly what I want. A while ago it still had a loading loop on start-up but that seems to be fixed now and beside of that I only experienced crashes if I try to enter a location it doesn't know. It has all the features I need and nothing more and I actually like it even more then KWeather and that means a LOT!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/BZ6Z2QhoFmx7/9CNwt1wnyh27nJUE9Bx3cfqnsb5kvv4sDOJL6YDT.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/AmIQFnHrcF2z/QGjaMaXwt6ji7G6U4IVNrWJUoeLiH7Dq5uQdJpGi.png) |
|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/DVqaQ5cmzVs2/klZn9ugfJ0CUInwhhViq5wwK4myz2coMzFGVUoJ1.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/sgCBJxCcd5au/PZo6wOmc8L1g59DWNxxLWaShL2conNukCuUH1lEO.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.gnome.org/GNOME/gnome-weather |
| AUR | gnome-weather (repo) gnome-weather-git |
| Flathub | https://flathub.org/apps/details/org.gnome.Weather |
| Mobian | gnome-weather |
| PostmarketOS | gnome-weather |

## Index:
Index is a feature rich file manager made with Kirigami and Mauikit. It's not my personal choice since I just like Portfolio more but there are features that I really miss which Index has build in like archive managing and creation and bookmarks. Those aren't enough to win me over but a lot of that is also just how much I love Portfolio. I really can't get used to the Mauikit UIs with the side scrolling menus, they just feel like desktop QT apps to me even in adaptive mode but that's really just my personal taste. Over all it's a really nice file manager with lots of cool features and if that's what you search you should definitely give it a shot!

**Note:**
To get Kirigami apps to work well under Phosh you need a few environment variables which Peter from Linmob has a [awesome list](https://github.com/1peter10/linuxphone-tweaks/blob/main/etc/environment) of!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/3eSXm1oHXppY/eCt6rLwtuIpZbuTOIikJhkrLwRVOSJjetEONkYKA.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/pftejfKVKALP/U6rduqu1nhVhggmr7w58zmyGV1gprY6wOQeN0BuW.png) |
|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/PPQ9g9DUosHr/NOU8aX3VgAhzoMl70sZG7Z89tgVVcW6AZxUbMS4Q.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/xR2ts8ve9G2Q/x788t19w5aANLQJd4WTKAPvCKWlWUQdHTBe0BVyQ.png) |

| Type: | Package: |
|-------|-------|
| Source | https://invent.kde.org/maui/index-fm |
| AUR | index-fm (repo) index-fm-git |
| Flathub | https://flathub.org/apps/details/org.kde.index |
| Mobian |  |
| PostmarketOS | index |

## Gnome Disks Utility:
This is a absolute must have for every GNU/Linux device no matter the form factor. It allows you to manage Disks, SD Cards, USB sticks and generally all storage you attach and do things like re-flash, format and re-size them. I actually already flashed a image of DanctNIX Arch to a SD card from the Pinephone using Disks and it took a while but actually worked! This is just a really handy tool and on Phosh it's a absolute must have!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/Td1un0vAfTV4/ByY5meTbvyMFzGp0g4i6GvZM1hIoO0zGO4lz9lhF.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/2v8zqkfHQouc/9yjWpktNl1Yvri7l97KLsapgsyQsDtPrpwPMlJNB.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/Uoq2SNnfM9Ai/ra7dXgc4SeLiUwdOUbHkCWVdLXhsNOh7IU6iCU96.png) |
|-------|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/WONNHBCN3IRn/qjpQgI5Og2eTUD4mOXeer3Xu4vE9MmOKO7hhiWvL.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/5b2iQEo6r7pa/0tOLztN6Co9L92yRkC7QUgOdhSjk9TaSLYYDOQK0.png) | ![]() |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.gnome.org/GNOME/gnome-disk-utility/ |
| AUR | gnome-disk-utility (repo) gnome-disk-utility-git |
| Flathub |  |
| Mobian | gnome-disk-utility |
| PostmarketOS | gnome-disk-utility |

**Previouse Post:**
https://gamey.tech/posts/pinephone-5-amazing-linux-phone-apps-part-2/
https://gamey.tech/posts/pinephone-5-amazing-linux-phone-apps/
