+++
author = "Gamey"
title = "PINEPHONE: 5 amazing Linux phone apps!"
date = "2021-10-07"
description = "List of awesome Pinephone apps."
tags = [
    "Pinephone", "ArchLinux", "5 Apps",
]

+++

Today I thought I would make a small list with some of the in my opinion best Pinephone apps. As always it's done on DanctNIX Arch with Phosh and my 2GB Pinephone and since I don't have a Librem5 I can't say anything specific about it but most of the apps should work across all true mobile GNU/Linux Phones.

**Note:** This is a old article but I rewrote most of it on 07.10.2021 to fix and update various things so enjoy! :D

## Tootle: 
One of my by far favorite Linux Phone apps with awesome adaptive design using GTK3 and a somewhat minimal approach is the Mastodon client Tootle. The app relies a lot on other system defaults for things like videos and images which probably contributes to the amazing performance even on a low power ARM chip like the Pinephones and the feature-set is kept minimal. Additionally there are design approaches like somewhat hiding things like stars and boosts which I really appreciate. There is a work in progress GTK4 app but sadly the dev Beaklegray tolled me he just switched job and has a fairly strict time limit so he will take some time off from coding to get everything sorted. I totally understand that and can't specially brag about my track record when it comes to writing new articles ether even without any excuse but I still hope that it wont be to long till he continues. I am absolutely in love with Tootle and GTK4/Libadwaita and think the two together would be awesome to have! Till then just get Tootle, trust me it pays off!

| ![](/../screenshots/Tootle/20210804_15h09m35s_grim.png) | ![](/../screenshots/Tootle/20210722_15h41m10s_grim.png) |
|-------|-------|
| ![](/../screenshots/Tootle/20210804_15h10m16s_grim.png) | ![](/../screenshots/Tootle/20210804_15h10m32s_grim.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/bleakgrey/tootle |
| AUR | tootle tootle-git |
| Flathub | https://flathub.org/apps/details/com.github.bleakgrey.tootle |
| Mobian | tootle |
| PostmarketOS | tootle |

## Audiotube:
If you like streaming music like me but don't have a Spotify premium account Youtube is probably your go to and this QML/Kirigami app provides a really convenient way to stream audio only content from it using youtube-dl and ytmusicapi. With Audiotube you can find and easily stream basically every song on Youtube and that with a fairly nice UI and neat queue functionality. It's still a relatively new app and there are features I really miss like downloading songs, local playlists, proxy functionality over something like Invidious or Piped and a few more but I already use it a ton and absolutely love the app! If you haven't tried it yet you really should do so independent of your DE and distro.

| ![](/../screenshots/Audiotube/20210324_23h03m03s_grim.png) | ![](/../screenshots/Audiotube/20210324_23h03m55s_grim.png) | ![](/../screenshots/Audiotube/20210324_23h04m48s_grim.png) |
|-------|-------|-------|
| ![](/../screenshots/Audiotube/20210324_23h05m12s_grim.png) | ![](/../screenshots/Audiotube/20210324_23h05m32s_grim.png) | ![](/../screenshots/Audiotube/20210324_23h06m23s_grim.png) |

| Type: | Package: |
|-------|-------|
| Source | https://invent.kde.org/jbbgameich/audiotube |
| AUR | audiotube-git |
| Flathub |  |
| Mobian |  |
| PostmarketOS | audiotube |

## Foliate:
A feature rich and nice to look at EBook reader made with GTK3. I am not that much of a EBook reader and generally prefer actual books because I find it hard to read for longer periods on a screen and like to read more complex books which aren't great to consume in short bites but I did read quite a bit on my Pinephone and Foliate is what I used for that. If you search for a good EBook reader that works well on Linux Phones like the Pinephone Foliate is my number one recommendation.

| ![](/../screenshots/Foliate/20210404_19h48m01s_grim.png) | ![](/../screenshots/Foliate/20210404_20h02m01s_grim.png) | ![](/../screenshots/Foliate/20210404_20h02m31s_grim.png) |
|-------|-------|-------|
| ![](/../screenshots/Foliate/20210404_20h03m19s_grim.png) | ![](/../screenshots/Foliate/20210404_20h03m57s_grim.png) | ![](/../screenshots/Foliate/20210404_20h04m52s_grim.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/johnfactotum/foliate |
| AUR | foliate (repo) |
| Flathub |  https://flathub.org/apps/details/com.github.johnfactotum.Foliate |
| Mobian |  |
| PostmarketOS | foliate |

## Portfolio:
Portfolio is a very minimal mobile first file manager made with GTK3 and written in Python. It's now the default for most Phosh distros and I probably wouldn't add it here nowdays because people know about it quite well but it's here and it's awesome so whatever I guess. There are still some nice to have features lacking like proper archive support and favorites but if you used Portfolio once you just have to love it. While mobile optimized apps are great only the mobile first approach shows what Libhandy can truly do and it's amazing!

| ![](/../screenshots/Portfolio/20210724_08h48m36s_grim.png) | ![](/../screenshots/Portfolio/20210724_08h49m01s_grim.png) |
|-------|-------|-------|
| ![](/../screenshots/Portfolio/20210724_08h49m19s_grim.png) | ![](/../screenshots/Portfolio/20210724_08h49m34s_grim.png) |  |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/tchx84/Portfolio |
| AUR | portfolio-file-manager |
| Flathub | https://flathub.org/apps/details/dev.tchx84.Portfolio |
| Mobian |  |
| PostmarketOS | portfolio (edge) |

## Quickddit:
Quickddit is a awesome and feature rich Reddit client for users with and without a account. It was originally made for Ubuntu Touch but somehow also works on other distros and while it may not be the best looking Linux Phone app (at least in Phosh) it sure dose deliver on the feature and usability front. Specially the option to move the top bar to the bottom for one handed use is something I wish more apps did and the featureset just isn't comparable to any other Reddit client for Linux Phones. It isn't my personal pick anymore but that's just because I don't need all the features and fell in love with [Headlines](https://gitlab.com/caveman250/Headlines) and has very little to do with this truly fantastic Reddit client so I still highly recommend giving it a shot!

**Note:** Since it's a Ubuntu Touch app building is a bit different but you can find build instructions in Peters article on Reddit clients for the Pinephone [here](https://linmob.net/reddit-clients-for-mobile-linux/)! 

| ![](/../screenshots/Quickddit/quickddit-1.png) | ![](/../screenshots/Quickddit/quickddit-2.png) | ![](/../screenshots/Quickddit/quickddit-3.png) |
|-------|-------|-------|
| ![](/../screenshots/Quickddit/quickddit-4.png) | ![](/../screenshots/Quickddit/quickddit-5.png) | ![](/../screenshots/Quickddit/quickddit-6.png) |
| ![](/../screenshots/Quickddit/quickddit-7.png) | ![](/../screenshots/Quickddit/quickddit-8.png) | ![](/../screenshots/Quickddit/quickddit-9.png) |

| Type: | Package: |
|-------|-------|
| Source | 	https://github.com/accumulator/Quickddit |
| AUR | quickddit |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |
