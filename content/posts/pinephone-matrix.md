+++
author = "Gamey"
title = "PINEPHONE: Matrix clients on Linux Phones!"
date = "2021-10-24"
description = "List of best avalable Matrix clients for Linux Phones. (E.g. Pinephone, Librem5, OnePlus)"
tags = [
    "Pinephone", "ArchLinux", "Matrix",
]

+++

I actually wrote two articles about this topic ages ago and there has been depressingly little development since then but there have been changes that make the future look a lot brighter. What I am referring to is Matrix support on Linux phones and with that push notifications which essentially don't exist in the current GNU/Linux ecosystem but are a essential component for a good Smartphone. I am probably not the only one who got frustrated by the current state more then once and possibly even lost hope altogether but there is a light at the end of a long tunnel and that's what I want to show you in this article! Even after all my research I am not able to find any good solutions and trust me I tried a lot but as I pointed out already there are clients that I have very high hopes in for the future and it is already possible to use some just in very limited capacity because of various issues, the main one being a total lack of push notifications.

The solution for push notifications will by the looks of it be Unified Push which is already in use in a few Android apps. I had a short chat with Vurpo who did some initial work on Unified push for Linux and and she tolled me that it's still very much work in progress and currently not usable but she already wrote specs, proof of concept implementations and implemented it for Nheko earlier this year, after that she sadly ran out of time so it's not complete yet but that's a great start. I am sure some project will pick his work back up and finish it because so many apps need push notifications and I'm looking forward to that!

## Fluffychat
A beautiful cross platform Matrix client made in Flutter and for mobile screens with encryption support, room discovery functionality and support for most Matrix features like "Spaces" or Markdown rendering. That seems to good to be true right? Well kinda, it's all true but the Flutter part causes issues like not specially amazing performance, a desktop like Gnome header bar I can't disable, no current background notification support and a extremely annoying bug with Wayland onscreen keyboards which after switching the window once causes the app to always jump back to the start of the text when you type and can only be fixed with a restart. Over all this is a absolutely awesome Matrix client for Linux Phones but Flutter really dose limit it's usability to a point where I sometimes feel like throwing my Pinephone out the window. Luckily Fluffychat has a awesome dev and community, while they can't do much about the Flutter issues they already work on a implementation for "unified push" which should enable push notifications for Linuxphone users.

**Note:**

- So far I only got it to work as Flatpak but there may be another way that I just don't know about.

| ![](/../screenshots/Fluffychat/fluffychat-1.png) | ![](/../screenshots/Fluffychat/fluffychat-2.png) |
|-------|-------|-------|
| ![](/../screenshots/Fluffychat/fluffychat-3.png) | ![](/../screenshots/Fluffychat/fluffychat-4.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.com/famedly/fluffychat/ |
| AUR | fluffychat fluffychat-git (Both seem broken) |
| Flathub | https://flathub.org/apps/details/im.fluffychat.Fluffychat |
| Mobian |  |
| PostmarketOS |  |

## Hydrogen
While this technically isn't a app it's a very nice web client optimized for low power devices and works fantastic on the Pinephone. It's very barebones with a ton of features like joining rooms, sorting rooms in any way, spaces, most settings and more just not implemented which seems to be the goal here actually. A nice way to read and write a bit on Matrix that works on basically any hardware and simply doesn't need to be a fully features client. It dose have some really nice features like E2E, multi account support and a handy setting to scale down images in case you internet is as bad as your hardware. When Firefox first removed all PWA functionality it initially broke but as far as I can tell it seems to work fine again and I definitely recommend if you have issues with Fluffychat and just as a backup in general.

**Note:**

- If you are on Plasma mobile just use Angelfish to use it as webapp but if you aren't I sadly don't have any solution I can recommend.

| ![](/../screenshots/Hydrogen/hydrogen-1.png) | ![](/../screenshots/Hydrogen/hydrogen-2.png) |
|-------|-------|
| ![](/../screenshots/Hydrogen/hydrogen-3.png) ||

| Type: | Package: |
|-------|-------|
| Source | https://github.com/vector-im/hydrogen-web |
| Universal | https://hydrogen.element.io |

## Nheko
A modern, feature rich native Matrix client designed for desktop devices but with some slight mobile optimizations. It's far from perfectly optimized but since Nheko doesn't use KDEs or Gnomes frameworks it's really cool that the dev still invested time for some manual optimization to make it usable on Linux phones. Issues include long starting times and often completely refusing to start, bad scrolling that sometimes triggers a chat, hard to hit buttons, often pre selected rooms that you then can't click on till you opened another one and go back and more small bugs like those. I actually used Nheko for a while and I'm thankful for all the work that people put into it but at the end of the day it's a desktop client, I think that's what it will continue to be and there is nothing wrong with that.

**Notes:**

- Nheko may need ``scale-to-fit nheko`` to fit the screen.
- Before you can use Nheko you also have to set ``mobile_mode=true`` in ``.config/nheko/nheko.conf`` or for Flatpak users ``.var/app/io.github.NhekoReborn.Nheko/config/nheko/nheko.conf``.

| ![](/../screenshots/Nheko/nheko-1.png) | ![](/../screenshots/Nheko/nheko-2.png) |
|-------|-------|

| Type: | Package: |
|-------|-------|
| Source | https://github.com/Nheko-Reborn/nheko |
| AUR | nheko nheko-git (broken) |
| Flathub | https://flathub.org/apps/details/io.github.NhekoReborn.Nheko |
| Mobian | nheko |
| PostmarketOS | nheko |

## Neochat
The main Matrix client for Plasma mobile which is incredibly well optimized for Linux phones with great performance, a good UI and a nice featurteset but unfortunately without E2E. They actively work on E2E and also expressed interest in a potential UnifiedPush implementation so they are headed in a really good direction but just not there yet. I will definitely keep a eye on this project and I am very excited to see it develop but in it's current state I can't recommend NeoChat over options like Fluffychat, Hydrogen and even Nheko because I really value encryption.

| ![](/../screenshots/NeoChat/neochat-1.png) | ![](/../screenshots/NeoChat/neochat-2.png) | ![](/../screenshots/NeoChat/neochat-3.png) |
|-------|-------|-------|
| ![](/../screenshots/NeoChat/neochat-4.png) | ![](/../screenshots/NeoChat/neochat-5.png) | ![](/../screenshots/NeoChat/neochat-6.png) |

| Type: | Package: |
|-------|-------|
| Source | https://invent.kde.org/network/neochat |
| AUR | neochat-git |
| Flathub | https://flathub.org/apps/details/org.kde.neochat |
| Mobian |  |
| PostmarketOS | neochat |

## Fractal
A Matrix client made with GTK3/Libhandy that could be awesome but lacks E2E and wont ever get it. The project is still maintained but most of the work has shifted to the fractal-next branch which is a full rewrite using the new Matrix Rust SDK and GTK4/Libadwaita so I wouldn't expect any big new features. It also has some issues accessing the Gnome keyring which means you have to unlock it manually before starting Fractal (E.g. with Seahorse). If you are still interested in using the client [here](https://gamey.tech/posts/fractal-on-the-pinephone/) is a old article of mine that shows how to do so with Seahorse and Pantalaimon to add E2E support but I would recommend you to wait. With the very promising rewrite on the horizon which will have E2E, even better mobile support, better performance and more it's definitely a project to look out for and who would have guessed, they also plan to implement UnifiedPush.

| ![](/../screenshots/Fractal/fractal-1.png) | ![](/../screenshots/Fractal/fractal-2.png) |
|-------|-------|
| ![](/../screenshots/Fractal/fractal-3.png) | ![](/../screenshots/Fractal/fractal-4.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.gnome.org/GNOME/fractal |
| AUR | fractal (repo) fractal-git |
| Flathub | https://flathub.org/apps/details/org.gnome.Fractal |
| Mobian |  |
| PostmarketOS | fractal |

## Chatty
As you may know Phosh's default SMS app Chatty was supposed to ship with Matrix support right from the beginning but they ran into issues with *Libpurple and ultimately decided to ditch it so everything took a lot longer then expected. Luckily they made some serious progress in that direction and even ship a experimental implementation with the app now. It doesn't seem to have device verification yet, currently spams your SMS with all your Matrix rooms and is probably rightfully still hidden behind the experimental setting. There however is E2E support, the interface works really well for 1o1 conversations and probably also private groups and it's right there in your SMS app that runs basically whenever your screen is on which obviously isn't a replacement for push notifications but better then nothing. The development of Matrix support for Chatty has had it's ups and downs and I can't even really guess to when it maight be ready for daily use but they have the hardest parts figured out now so I am optimistic.

**Notes:**

- To enable the experimental features of Chatty (Matrix and MMS) you have to use ``gsettings set sm.puri.Chatty experimental-features true``.
- Chatty is preinstalled on any distro using Phosh since it's the default SMS app there and I don't think it makes sense to install it using other DEs so I skipped the package list in this case.
- I disabled experimental features immediately after catching it use over 800MB of ram in the background instead of the usual 25-30 but I didn't do any debugging.
- *Libpurple is a library that aims to support all kinds of chats in a single client (E.g. Matrix, Discord and much much more) but apparently with a lot of flaws, from what I gathered specially in the Documentation and regarding hard coded parts in a few libraries that bind it to the main client Pidgin which definitely shouldn't be a thing.

| ![](/../screenshots/Chatty-Matrix/chatty-1.png) | ![](/../screenshots/Chatty-Matrix/chatty-2.png) | ![](/../screenshots/Chatty-Matrix/chatty-3.png) |
|-------|-------|-------|
| ![](/../screenshots/Chatty-Matrix/chatty-4.png) | ![](/../screenshots/Chatty-Matrix/chatty-5.png) | ![](/../screenshots/Chatty-Matrix/chatty-6.png) |

## Others
Just a few clients that didn't make it in the main list for various reasons. There are also a few more ether desktop specific or terminal clients which I didn't bother to mention here because the scope of this article already increased like stupid and I want to publish it at some point but you can find them on https://matrix.org/discover/ .

- **Kazv:** A WIP client made with Kirigami but I couldn't get it's library (libkazv) to actually build on my Pinephone.

- **Quaternion:** A Desktop client with zero mobile optimizations so while it technically works like any Linux app the UI is unusable.

- **Spectral:** Another Desktop only client, see text about Quaternion.

- **Gomuks:** A terminal based client that I actually used for a little while but terminal apps honetly just aren't great to use on mobile devices.

- **Mirage:** Mirage is a desktop only Matrix client and thanks to it's gesture based interface it was the first client I am aware of that supported proper E2E on Linux phones. I used it for a while and I am thankful for that but it's a awful experience with start up times of literal minutes, A extremely confusing interface, barely functional touchscreen scrolling and more because after all this is clearly a desktop client.

- **Syphon:** I had a very short chat with the dev and I think he will take a look at Fluffychats way of getting the desktop version to work on the Pinephone and possibly try to replicate that.

- **Cinny:** One of the best looking Matrix clients I have ever seen which is currently desktop only but mobile support using PWAs is apparently planned.

## More

**Mentioned Clients:**

- Fluffychat: https://gitlab.com/famedly/fluffychat
- Hydrogen: https://github.com/vector-im/hydrogen-web/
- Nheko: https://github.com/Nheko-Reborn/nheko
- NeoChat: https://invent.kde.org/network/neochat
- Fractal: https://gitlab.gnome.org/GNOME/fractal
- Chatty: https://source.puri.sm/Librem5/chatty
- Kazv: https://lily.kazv.moe/kazv/kazv
- Quaternion: https://github.com/quotient-im/Quaternion
- Spectral: https://gitlab.com/spectral-im/spectral
- Gomuks: https://github.com/tulir/gomuks
- Mirage: https://github.com/mirukana/mirage
- Syphon: https://github.com/syphon-org/syphon/
- Cinny: https://github.com/ajbura/cinny

**Other:**

- UnifiedPush: https://unifiedpush.org/
- Fractal UnifiedPush: https://gitlab.gnome.org/GNOME/fractal/-/issues/675
- Splitting Fractal: https://blogs.gnome.org/tbernard/2018/05/16/banquets-and-barbecues/

