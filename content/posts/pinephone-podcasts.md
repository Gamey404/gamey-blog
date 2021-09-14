+++
author = "Gamey"
title = "Podcasts on the Pinephone"
date = "2021-08-12"
description = "A review of allk current Podcast clients for the Pinephone."
tags = [
    "Pinephone", "ArchLinux", "Podcasts",
]

+++

Today I want to talk about Podcasts on mobile GNU/Linux devices. As one of the last truly free media formats Podcasts are a perfect match with devices like the Pinephone and it's also what I enjoyed most of in terms of content formats on mine. I have to admit that I never really was into Podcasts but lately I discovered that one of my favorite newspapers (Der Falter) has one and from there it just went on with my all time favorite Darknet Diaries which is just fantastic, the Pinetalk and the PostmarketOS podcast. I bet I will discover many more in the future because now I am hooked!

## Kasts:
Kasts is the main Plasma mobile podcast app and my so far favorite. It's made with QT/Kirigami which causes a few lags here and there but nothing to bad considering the amount of episodes most of the podcasts I listen to have and it's definitely usable on Phosh to. It has all the features I want from a Podcast app like remembering where in the episode I was, keeping the device from going in deep sleep which would stop the playback after a few minute, downloading, a really good UI to manage downloaded episodes, a view that shows the episodes of all podcasts in chronological order and one that shows all the podcasts I subscribed to which is basically all I need. You may miss the ability to stream episodes but I prefer to download them anyway because I use a prepaid simcard and still like to be able to do stuff like take a walk while listening to a episode. Over all I really recommend Kasts and will probably keep using it for a while!

**Notes:**
- On many Phosh distros you need to start it with ``QT_QUICK_CONTROLS_MOBILE=1 kasts`` because Phosh currently doesn't implement KDEs mobile flag which is required to use the mobile mode of Kirigami apps so that is basically up to the distro rn.

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/c7AbwtTqgbcX/twiw85YI6gU1EJXHgX7frc6M7kRDEYSXqlUfbbYk.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/fJz3FI9tQq2c/kjf1lUHRmEJ3HBNxUnp07jMMEJXlcypHiGyzjgJw.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/iCCAPquT9YjS/KSN7Jdz8DO03RhCbxOua87YEmbN7s6a5ys5DPOQq.png) |
|-------|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/PtTYXBNcw00b/BrHaBhVKqv0c3t4gCmxBc0c7uy4sTqzPU9SnVHdE.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/vJ02UlXXNMB5/e4dC2NSjkPErbQt9U8BC2sv0YYkmDHDzacjiUwEP.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/SC3tBVkjYo5D/iq9FVOD8iH9ckt5FUeqRKKDTph0t1bTNZYPga9S8.png) |

| Type: | Package: |
|-------|-------|
| Source | https://invent.kde.org/plasma-mobile/kasts |
| AUR | kasts kasts-git |
| Flathub |  |
| Mobian |  |
| PostmarketOS | kasts |

## GPodder Adaptive:
The adaptive branch of GPodder works surprisingly well on the Pinephone. It takes some getting used to because most modern Podcast apps have a build in audio player and more streamlined interface but I actually did enjoy using GPodder after a while. A major issue is finding a audio player that blocks deep sleep in Phosh and remembers where in the episode you are without forgetting that when you listen to something else (music). The interface has a few rough edges but over all it dose what it's supposed to very well and is for sure the winner when it comes to performance so overall a nice choice!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/NLbyES1TO49A/k702xjqbGjIsjQQT2bmxtogXFhq9Ce6mJZNna8qR.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/TfrLsFr5edm8/hC6FBgsJ5VIZymz66yYUJaorRf6DdGfNHVu0av6G.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/3GI362240Rsi/LPrwwmW5ObEP31hjQjj1PfNCTL6DiMr5Kh0E4gjL.png) |
|-------|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/HIckuwqUTziB/WXOMm9v4NiiDZr9vhhpvjVYQSKVijdlxwIXhSUga.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/eZZ0tu5uEnN1/nazLNMDYVBPEXOJ7BlzEOSzg2o5s5zrVJmx8oY7x.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/ubGKYGxL9edE/IDzXLAFwngyRPmDqad12CHMotT9NJyqsMOTXAFRd.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/gpodder/gpodder/tree/adaptive |
| AUR | gpodder-adaptive-git |
| Flathub | https://flathub.org/apps/details/org.kde.kasts |
| Mobian |  |
| PostmarketOS | gpodder-adaptive |

## Gnome Podcasts:
Gnomes official Podcast app is about what you would expect from a Gnome app. Very bare bones in terms of features but whats there works well and is amazing to use on mobile screens. The reason it only ranks third place in my opinion is that it totally lacks any way to manage downloaded episodes and has no way to stream so as Pinephone user like me with 16GB of storage you can basically only wait till it deems the episode old and deletes it by itself (seems to be at three episodes in my experience). I also noticed that it doesn't remember where you where in the episode or even what you were listening to so that is another major downside in my opinion. I like the app and it's well made and everything but I just can't forgive those drawbacks for my personal usage.

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/bOPtC9xKwbtj/1DeEKVwuZQMtL8grWjnXLsJjr0cQX5MPOMpy9nh8.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/usZvkt7NZDzX/vTxdNASg3Ez5CNBWmwugqLhZ7xEMRAzaubT7AkkB.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/6d2rXzLly2GN/hDMnVrgUz0r6VX1M5ntjHWtUOh1Bi3MYXJztKwRu.png) |
|-------|-------|-------|
| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/1KoExBYpxySE/6ekENmQ8bt96qnNhDX6NhO6OyEKV2q17TV9v5hUl.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/sUtK3GXN3MGb/ehdafIX7wDLNDiy4j67OnSTB5IsW2NRvYt4V1B1T.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/Z7P2D73dMNLR/y6kgwVPPU1kUBDAZim9Wd9JtEyAEyv5XGVXw8G03.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.gnome.org/World/podcasts |
| AUR | gnome-podcasts (repo) gnome-podcasts-git |
| Flathub |  |
| Mobian |  |
| PostmarketOS | gnome-podcasts |

## Pyrocast:
Pyrocast is a Gnome Podcast fork made with GTK and written in Rust. Unlike most other apps on this list it streams episodes instead of Downloading them and that with a unfinished but really nice UI. Sadly it seems to be a dead WIP project which you totally can use if you dislike downloading each episode before listening to it but it's clearly unfinished and it doesn't seem like it ever will be :/

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/0tUAy7FsqQeY/DkaRrvF6IaUyCQDAzGcO4xVEn6LgySp6tJNba3tI.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/UJ1oh0wvA537/1Y38ygD3Dfit9zGizadZapeCIzUPkwRWyNooXyHq.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/sW3IhHfqWu6z/K7zUksJ2jz76gWGDJ8WDx5dQCznaApI3pS3y90Eo.png) |
|-------|-------|-------|
| ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/nwXOUx78FAIS/7ZBSPSj412njddqNbZKkzMYlcLj3cXLjSIYSQVDs.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/EYFFq4Om4ngn/w7Fphr0ROxZKrtfEl7GA4gQsSkIDgsziPbyFCMaG.png) | ![]() |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/jnetterf/pyrocast |
| AUR |  |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |
| Binary | https://linmob.uber.space/pyrocast |

## Pods:
Pods is a minimal Podcast client written in Rust. It's goal to me seems to be a GPodder like experience (No build in audio player or any of that fancy stuff) but it still lacks most features and the UI is clunky and just not nice to use yet. Most buttons have ages of delay before they trigger and you have to hold them down for a while or they wont do anything, additionally the top bar is still there and just gets moved off the screen which leaves a gap at the bottom and the overall layout just isn't intuitive in my opinion. I had a chat with the dev on Reddit and he tolled me that the UI is still in pre-alpha and that he currently learns how to do it properly so it is not a client I can recommend yet but I like the aim of the project and hope it continues!

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/dclHe92P1kkr/d7aHjz7JfZXWkt1znAvRsFaoG4qToRU3Zbs97VbH.png) | ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/Z094W6cXIBcJ/mV1SRXyufFbW11HQeEzXDWSBlL7cjlPCe0DB83Sr.png) |  ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/QmbyRyrHsby9/JTgrmStgDnwDwB0jDFJuAELNWNZaWCM4zsWrwX7U.png) |
|-------|-------|-------|


| Type: | Package: |
|-------|-------|
| Source | https://github.com/dskleingeld/pods |
| AUR |  |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |
| Binary | https://open.lbry.com/@GameySecond:2/pods-bin:6?r=D23fWA6ePDwmZpXPfaLBzkDVj5qWRWYW |

## PineCast:
Pinecast is another minimal and WIP podcast client written in c++. The UI is a bit odd if you are used to modern streamlined interfaces but already works really well and doesn't look bad ether. I ran into a few issues in my testing including no proper downloading capabilities yet, no sort of animations or loading indicator which makes the UI feel like it's lagging at times, issues with scrolling on mobile devices which in combination with the lack of a page per episode means random download triggers while scrolling, no way to cancel a ongoing download and just generally a lack of features I like even in a minimal app. All of that is to be expected with a heavy WIP app tho and PineCast to me seems like it's the right direction just a bit early for actual usage.

**Notes:**
- After compiling the app you have to create a folder called ``Podcasts`` in the same folder the binary (main.cpp) is in or subscriptions wont work.
- It uses a special library of curl for C++ called ``libcurlpp`` which is in the AUR but seems to be lacking from most repos.

| ![](https://pixelfed-prod.nyc3.cdn.digitaloceanspaces.com/public/m/_v2/245825453661753344/f98697a52-a34568/UIlXQVNAcHiF/nyVnNnOD7i25ViRDzKi0u1Ca91rtD7lySdkVGgeQ.png) | ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/obM7vsSULjzS/0nmJfuueYAY80cXl1tJxc747eEKlpYCNswkw3UTy.png) |  ![](https://pixelfed.social/storage/m/_v2/245825453661753344/f98697a52-a34568/7swdCBLFBzKl/Ffu8o5SKECdW4uBYlhluzpPw1cSS8PKQgmYG2CaM.png) |
|-------|-------|-------|

| Type: | Package: |
|-------|-------|
| Source | https://github.com/dskleingeld/pods |
| AUR |  |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |
| Binary | https://open.lbry.com/@GameySecond:2/pods-bin:6?r=D23fWA6ePDwmZpXPfaLBzkDVj5qWRWYW |

**Credits:**
- Big thanks to Peter who send me the binary for Pyrocast since I couldn't get it compiled on my own and maintains the fantastic [LinMobApps](https://linmobapps.frama.io/) that I rely on heavily for my Pinephone usage and content!
- Thanks to the two devs on Reddit who provided very useful information and special thanks to the PineCast dev who even helped me to compile his app in PMs!

**Mobile GNU/Linux podcasts:**
1. PineTalk: https://www.pine64.org/pinetalk/
2. PostmarketOS Podcast: https://cast.postmarketos.org/
3. If you know any I forgot make sure to comment down below and I will add them :D

**Extra Links:**
- Reddit thread: https://libredd.it/r/pinephone/comments/oz3dby/podcasts_on_the_pinephone/
- Pine64 forum: thread: https://forum.pine64.org/showthread.php?tid=14594
