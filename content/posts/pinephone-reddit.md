+++
author = "Gamey"
title = "PINEPHONE: Reddit clients for Linux Phones!"
date = "2021-10-10"
description = "List of best avalable Reddit clients for Linux Phones."
tags = [
    "Pinephone", "ArchLinux", "Reddit",
]

+++

Today I will focus on Reddit clients, yea I know Reddit is big tech but it can be incredibly useful and at least since I started to write articles like this one I wouldn't want to miss it. There are actually quite a few Reddit clients and some of them very nice to so I would say that in this aspect you are absolutely covered as Linux Phone user! As always all of my testing is done on my 2GB Pinephone running DanctNIX Arch Linux and Phosh as DE.

## Headlines
A relatively new and beautiful GTK4 Reddit client that's very much in the Spirit of Giara but seems to work better on low end devices. There are some annoyingly long loading screens on the Pinephone that I really hope are fixable but when something is loaded it's a really smooth experience with close to no lags. The client still seems to be in very active development and will probably change quite a bit in the future so certain things like issues requesting the Gnome keyring (required to access your login) will probably be patched soon if they aren't already. This is definitely my personal favorite after testing all the clients on this list and I will probably stick to it for now :D

**Note:** In it's current stage Headlines doesn't seem to unlock the Gnome keyring so I recommend Seahorse as a nice way to do it manually.

| ![](/../screenshots/Headlines/headlines-10.png) | ![](/../screenshots/Headlines/headlines-9.png) | ![](/../screenshots/Headlines/headlines-8.png) |
|-------|-------|-------|
| ![](/../screenshots/Headlines/headlines-7.png) | ![](/../screenshots/Headlines/headlines-6.png) | ![](/../screenshots/Headlines/headlines-5.png) |
| ![](/../screenshots/Headlines/headlines-4.png) | ![](/../screenshots/Headlines/headlines-3.png) | ![](/../screenshots/Headlines/headlines-2.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.com/caveman250/Headlines |
| AUR | headlines |
| Flathub | https://flathub.org/apps/details/io.gitlab.caveman250.headlines |
| Mobian |  |
| PostmarketOS |  |

## Giara
Another beautiful GTK4 Reddit client that has been around far longer then Headlines and is a main contender for desktop users but also well mobile optimized. My favorite Giara feature is for sure the build in Invidious and Nitter support which I think all clients should have but annoyingly it lacks browsing without a account. I can't specially recommend it to Pinephone users since it appears to be more demanding then the others which beside of a really hot phone also causes some lags but for people with a more powerful device like the OpnePlus6 or Librem5 it could certainly be a great choice!

| ![](/../screenshots/Giara/giara-1.png) | ![](/../screenshots/Giara/giara-2.png) | ![](/../screenshots/Giara/giara-3.png) |
|-------|-------|-------|
| ![](/../screenshots/Giara/giara-4.png) | ![](/../screenshots/Giara/giara-5.png) | ![](/../screenshots/Giara/giara-6.png) |
| ![](/../screenshots/Giara/giara-7.png) | ![](/../screenshots/Giara/giara-8.png) | ![](/../screenshots/Giara/giara-9.png) |

| Type: | Package: |
|-------|-------|
| Source | https://gitlab.com/gabmus/giara |
| AUR | giara-git |
| Flathub | https://flathub.org/apps/details/org.gabmus.giara |
| Mobian |  |
| PostmarketOS | giara |

## Quickddit
A mobile first Reddit client that works on Ubuntu Touch, SailfishOS and more desktop like distros. My article will only focus on the more desktop like distros (E.g. DanctNIX Arch, PostmarketOS and Mobian) since that's what I use but the great cross distro support is still really cool! Aesthetically it fails to bring over the full beauty of Ubuntu Touch in my opinion but functionally it's a absolute blast. Often little things like the option to switch the top bar to the bottom for one handed use can really impact usability and other nice features like surfing Reddit without a account or multi account functionality aren't missing here ether, so while originally designed for Ubuntu Touch this is definitely a feature rich and nice to use app for multiple Linux Phone distros and DEs. I only really use Phosh but I would love to hear from you Plasma mobile and specially SXMO users!

**Note:** Since it is a Ubuntu Touch app building Quickddit is a little different then most other GNU/Linux apps. Peter from Linmob made a old but great article [here](https://linmob.net/reddit-clients-for-mobile-linux/) where he goes over it!

| ![](/../screenshots/Quickddit/quickddit-1.png) | ![](/../screenshots/Quickddit/quickddit-2.png) | ![](/../screenshots/Quickddit/quickddit-3.png) |
|-------|-------|-------|
| ![](/../screenshots/Quickddit/quickddit-4.png) | ![](/../screenshots/Quickddit/quickddit-5.png) | ![](/../screenshots/Quickddit/quickddit-6.png) |
| ![](/../screenshots/Quickddit/quickddit-7.png) | ![](/../screenshots/Quickddit/quickddit-8.png) | ![](/../screenshots/Quickddit/quickddit-9.png) |

| Type: | Package: |
|-------|-------|
| Source | https://github.com/accumulator/Quickddit |
| AUR | quickddit |
| Flathub |  |
| Mobian |  |
| PostmarketOS |  |

## Others:
Just a few unmaintained projects that I still want to mention.

- **tuir:** A Terminal client for Reddit that seems to have most features except subscribing to Subreddits (you can still view them as far as I can tell) but I couldn't get the login to actually work and while it scales just fine keybinding based navigation can be a bit annoying on a mobile device. It was recommended to me on Reddit by xxxx a SXMO user and I think xxxx was able to log in to but I wont use it so I am not going to figure out what went wrong ether. If you want a Terminal client while unmaintained Tuir looks really nice even on mobile screens and definitely could be worth a try and if you use it already I would love to hear some feedback.

- **Something for Reddit:** You may need a microscope but with scale to fit this old GTK Reddit client actually works. It's not specially usable and had no updates in over three years so I have fairly low hopes for future mobile support but it's still a client I guess.
https://github.com/samdroid-apps/something-for-reddit

- **Reddit client GTK:** I couldn't get it to build yet (needs cross compiling) and since it's a abandoned WIP Rust learning project I am just not going to bother. I don't think it's worth checking out ether but it exists so I may as well mention it.
https://github.com/johan-bjareholt/reddit-client-gtk

- **Baconer:** Seems like this one was abandoned in very early development and probably with barely any mobile support even tho it looks like it was supposed to target mobile devices. It lags really bad, the UI is very ugly and hard to navigate, it seems to straight up just load websites for stuff like videos which make the scaling issues even more obvious and just generally is unusable. There also wasn't any activity on the repo for over nine months so unless the Plasma mobile team picks it back up I don't have specially high hopes for Baconers future. It's one of those many many small Kirigami apps with no description and using qmake, most of which seem to have targeted Android (E.g. blabber).
https://github.com/TomBebb/Baconer

## Related:
- My posts on Reddit about this article [r/pinephone](https://www.reddit.com/r/pinephone/comments/py5rz1/reddit_clients_on_the_pinephone/) [r/PinePhoneOfficial](https://www.reddit.com/r/PinePhoneOfficial/comments/py5t1q/reddit_clients_on_the_pinephne/)
- My post on the Pine64 forum about this article [here](https://forum.pine64.org/showthread.php?tid=14990)
- Peters old article about the topic [here](https://linmob.net/reddit-clients-for-mobile-linux/)
- LinMobApps [here](https://linmobapps.frama.io)
- My articles about Linux Phone apps [1](/posts/pinephone-5-amazing-linux-phone-apps) [2](/posts/pinephone-5-amazing-linux-phone-apps-part-2) [3](/posts/pinephone-5-amazing-linux-phone-apps-part-3)
