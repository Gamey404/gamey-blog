+++
author = "Gamey"
title = "PINEPHONE: 5 amazing Linux phone apps! Part 2"
date = "2021-08-05"
description = "List of awesome Pinephone apps."
tags = [
"Pinephone", "5 Apps Pinephone", "Linux Phone",
]

+++

Today I want to highlight five more of the in my opinion best Pinephone apps in a little more detail. I think I will make a series out of this because I like to do it and apparently people like to read it. As always all of my testing is done on my 2GB Pinephone with DanctNIX Arch Linux.
<!--more-->

## Tubefeeder:
Tubefeeder is something in between a feed reader and Youtube client made with GTK and written in Rust. It allows you to follow Youtube channels and builds a convenient feed out of them, it then plays the videos using youtube-dl and MPV to improve performance and allow for somewhat fluid 720p video playback even on the Pinephone. Additionally it has a "watch later" list, a easy way to follow channels with just the name and some filters I don't really understand.

| ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/MojrbLPF7jSA/dSiWHNb3CUyLOym1lVrbI2LSq8SoJZUN0clFRJHf.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/WNas9Z7NEe4f/LU8v2yzmQHg1SzcBMnArXhITRR8olU3f5vqVPnx0.png) |
|-------|-------|
| ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/0kTiEU1okFaB/Ky0EUk3C5Xe6LsI9EUMdraOy6tHgSkY1zRz3pd6m.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/aZL7bgskGtwt/xnFA7Y0inzHR7KdJcmByA5AFJhu0rRt5RtUeyAiH.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/Schmiddiii/Tubefeeder |
| AUR |  |
| Flathub | https://flathub.org/apps/details/de.schmidhuberj.tubefeeder |
| Mobian |  |
| PostmarketOS |  |

## KWeather:
KWeather is a weather app made with QT/Kirigami and written in C++ and QML. It's fairly simple but covers everything you need like a simple forecast, the option to add multiple locations and the ability to switch Temperature and wind speed units. There are also two themes but only the "flat" theme runs decently well on the Pinephone (in terms of performance) so that's the one you should probably use!

**Note:** Kirigami apps require a "mobile mode" which Phosh doesn't seem to implement and many Distros (including Arch) don't yet ether so I used ``QT_QUICK_CONTROLS_MOBILE=1 kweather`` but my daily driver PostmarketOS doesn't need it so I didn't bother to get rid of the top bar or find a better solution.

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/eV2egPKhxXyA/CiDVeZEhPoByDkUm27f8p3be1CLKiCmwn254VUjo.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/4qY7mn72ui81/4h64sGOUIejeivsa0HEwHarA8CkmKFSCOMAWVKDr.png) |
|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/gtiqaaW9RX97/uqNsVhI4aVhpEVPdj2S5PgqEJAc40krTtJF3qtsb.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/63QcHzTAlwvX/LthfrMNq1KjTEbmr5pWi4o1zVDQSgtnHZhoX3Zvz.png) |

| Type: | Package: |
|-------|-------|
| Source | https://invent.kde.org/plasma-mobile/kweather |
| AUR | kweather-git |
| Flathub | https://flathub.org/apps/details/org.kde.kweather |
| Mobian |  |
| PostmarketOS | kweather |

## Wake Mobile:
Wake mobile is a proof of concept alarm clock for the Pinephone made with GTK and written in Python and C. It utilize SystemD to wake up the device from deepsleep which makes it useless on my PmOS daily driver setup but work on most other distros. I used this app multiple times to wake me up and it worked reliably so while it's a proof of concept it's a must have for anyone who wants to use the Pinephone as alarm clock!

| ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/QRnJdSrQG6FT/V1jFY1NySd10SIyF9am9DAM6lo7UjpNuneIGMYpD.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/j5MyZm2sj7ct/69VBztkTiXtMRUtBblsqKlJoHSDeRwKD48MJ1qqr.png) |
|-------|-------|

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.gnome.org/kailueke/wake-mobile |
| AUR |  |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |

## Fragments:
Fragments is a simple Bittorrent client made with GTK and written in Vala. I wouldn't use it on my computer because it lacks a lot of features I like to have as somewhat frequent Torrent user but it's really nice on the Pinephone. I admit that on a device with 16GB storage I don't use torrents that frequently and haven't used Fragments much yet but it's really handy to have!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/vWJwYNy5AaBF/LwiRWeUuPoHO5DjlAWpvThrWzU0tcTDDPgGMssI8.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/vQIALEVi6Jpc/lwcvCgzYIPzVwW18HkKfq6jWjwjNdYzMQC8970Ad.png) |
|-------|-------|
| ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/ofN7x2fxqNKb/SjIQoENnSUTIxP91A9QLGrydiu5kYbAEfhJmvcPO.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/xcVQqprAycGc/xLgf5zJ3gvGsSDSsqgGm5MBSFDmdqvgiErrfGB07.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.gnome.org/World/Fragments |
| AUR | fragments-git |
| Flathub | https://flathub.org/apps/details/de.haeckerfelix.Fragments |
| Mobian |  |
| PostmarketOS |  |

## Shattered-pixel-Dungeon:
Shattered-Pixel-Dungeon is a amazing Rougelike RPG made with Java/LibGDX. I originally played this game on a Android phone years ago and it quickly became my favorite mobile game of all time but what I only realized years (when I got my Pinephone) is that it's cross platform and works on the Pinephone. There only was one issue, it had some sort of dependency issues so the .jar files didn't work and while there was a working ``.deb`` that for obviouse reasons limited it to Mobian till [Moxvallix](https://github.com/moxvallix) who currently runs the LinMob Games list and repo (A extra list to [LinMobApps](https://linmobapps.frama.io/) that houses games) added a working ``.jar`` to the repo. If you want a fun little game to play from time to time on your Pinephone you just have to try this one because it's simple but also simply awesome! :D

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/xTrWBGHEieky/2W59QUYkglImsN25LsZ062RsQnygdeDrKp8sngRo.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/Jb7JW5o6lh3w/GC2qyzPKDtYl94cZiILiTu7cOnKS5Bf0nSwJUmLS.png) |
|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/OA3DIn1JZKfr/ddTAzssMEG4lz0Bq0AHVAlTIleSQgIj8NFlXWbn4.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/ZZeFTIONnwap/5lNKp1HBo35qFx481cKhNFkeNMTcgV6h5YH7oDOQ.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/moxvallix/LinMobGames |
| AUR |  |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |
| Working .jar | https://github.com/moxvallix/LinMobGames |

**Previouse Post:**
https://gamey.tech/posts/pinephone-5-amazing-linux-phone-apps/
