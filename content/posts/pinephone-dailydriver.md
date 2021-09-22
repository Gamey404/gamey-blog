+++
author = "Gamey"
title = "My Pinephone Dailydriver setup (Outdated)"
date = "2021-04-12"
description = "A list of most current Browsers for the Pinephone."
tags = [
"Pinephone", "Linux Phone",
]

+++

Today I will talk a little about my personal Pinephone setup which I use as daily driver by now. Unlike on my testing setup where I just love DanctNIX Arch ARM in this case I chose PostmarketOS. The reason for that is it's minimalist approach which fits perfect for a Alpine base and even better for a low end device like the Pinephone. The main advantage of Arch is the AUR and it's always up to date packages which makes it perfect as a testing setup and for many of your probably also as daily driver but I tend to spend a lot of time for my daily driver setups to get them right once and then use them till I want to change something. I also took PostmarketOS edge since I think stable isn't quite there yet but as soon as I get along with stable I will switch to that. So to sum it up what I use as my current daily driver phone is PostmarketOS edge with my favorite mobile DE Phosh. I can't really say why but I just don't like Plasma mobile in it's current state it somehow feels cheap to me (personal taste). I though it could be useful to some to also include parts of the installation because of the sometimes annoying but awesome Pmbootstrap so this post will probably be a bit longer then my usual ones. As always everything is done on my 2GB RAM Pinephone and may be a tiny bit different on a 3GB version.
<!--more-->

## Installation:
PostmarketOS doesn't give you any really good images instead they have a tool for it (Pmbootstrap). It can be a bit annoying at times but over all it's actually really nice since you don't get years old software all the time. You can get Pmbootstrap over pip or like I did it just from [this]() Github.

1. Install Pmbootstrap on your Linux computer via pip or from the git repo. If you had it installed before make sure to run ``pmbootstrap status`` to check for updates and update in case there are any!
2. Start Pmbootstrap with the command ``pmbootstrap init`` and select what you want. I will go for the edge repo since the stable branch isn't quite there yet in my opinion and I will also enable none free firmware since it's currently kind of a must. As user interface I will go with Phosh since it's my current favorite and just generally the in my opinion most usable DE right now.
3. After init you have to continue with ``pmbootstrap install``. I think you can also install it directly but I will just go for a ISO image here. I also want fde (full disk encryption) so I will go for ``pmbootstrap install -fde`` which I would recommend to everyone. Oh and don't type a password in when it asks you for one since Phosh and Plasma mobile both currently only work with a pin so just make it numbers only. The encryption password in case you enabled it is a different case for that you should get creative to find a secure one!
4. In case you did it like me (aim for a ISO image) you have to use ``pmbootstrap export``. When it's done it should tell you that a image is in ``/tmp/postmarketOS-export`` and with that you are almost done.
5. The final step is to type ``pmbootstrap shutdown`` and continue by flashing the ISO it gave you with whatever tool you like. I just used Gnome Disks but Etcher and others work to and in case you prefer terminal tools that's a option as well. That's it you should have a working image of PostmarketOS flashed to your device now :D

## Apps I use:
A list of the Apps I actually use on my device which you can hopefully take as inspiration.

- **Angelfish:** The default Plasma mobile web browser which also works great  on PostmarketOS and is useful as backup browser next to Firefox.
- **Portfolio:** A minimal GTK mobile first file manager which still lacks a few features but works like a charm.
- **Audiotube:** A Youtube music player which is still extremely new but already works quite nice and is a must have if you sometimes listen to music that isn't on your device.
- **PostmarketOS Tweaks:** A Gnome tweaks inspired app for PostmarketOS Phosh which allows you to change some settings like animations and theme.
- **Gnome Disks:** If you are a Linux user you probably know this utility it's just useful to work with SD cards on the Pinephone.
- **Gnome Feeds:** My favorite GTK feed reader (made for local feeds).
- **Tootle:** A amazing GTK Mastodon client which works like a charm.
- **Foliate:** A feature rich GTK EBook reader which works very well on the Pinephone.
- **Calindori:** The Plasma mobile calendar app which is just amazing no matter your DE.
- **Gnome Weather:** Lately this one is broken for me (gets stuck in a loading loop on the second start and never recovers) but if it would work it would be a damn awesome app.
- **Fragments** I haven't had to use it yet but a nice torrent client is always nice to have.
- **Flatseal:** The best way to handle Flatpak permissions and in case you use Flathub with it's low security standards a absolute must have to make the sandbox a actual sandbox.
- **Hydrogen:** This one is technically more of a website then a app but it's still my favorite Matrix client for the Pinephone till the Chatty implementation is ready.
- **Eye of Gnome:** A very simple image viewer which works decent enough on the Pinephone.

## Cool Apps:
Just some apps I really like which I simply don't have a use for but you may so why not include them :D

- **Quickddit** A fantastic Reddit client which I would go for if I used Reddit more.
- **Cawbird** A nice GTK Twitter client which works decent but I only tried it with a tempmail account so my knowledge is limited here.
- **Goodvibes:** In case you want a internet radio client for whatever reason this one looks amazing to me.
- **Onionshare:** It doesn't scale that well but it's usable so in case you have to upload any files that should stay anonymous you can use it.
- **Gnome Password Safe:** I really have to update my KeePass db so I can use this app better. Bitwarden is nice and all but it really starts to annoy me with that bloated web interface that can't scale for mobile screens at all.
- **Gnome Podcasts:** I usually don't listen to podcasts so this app lands here but it's actually fantastic and I may try the Pine64 podcast and see if I like the media format after all.
- **Spot:** I don't use Spotify but in case you do and have a premium account this client looks really damn nice to me.
- **Telegram:** I simply don't use Telegram and would choose Matrix, XMPP and even Signal or Wire over it every time but in case you like it the desktop client works nice on the Pinephone. Just keep in mind that you won't have any encryption and I will leave it at that before I start to rage.
- **Gnome Authendicator:** I should really start to use 2factor more but currently I got the app installed and never used it.
- **Briar GTK:** Last time I tried it I had to build this damn Java/Python mess from the AUR which takes ages and it kept breaking from time to time but if you use Briar you may have more patience then me.
- **Castor:** A adaptive GTK Gemini browser so in case you use Gemini this is probably your best pick on the Pinephone.
- **Hackgregator:** A GTK Hackernews reader that works nicely on the Pinephone.
- **Index:** A more feature rich file manager which you can use in case Portfolio lacks something you need.
- **Pika Backup:** I currently don't have any backup since I use all my SD cards to play around but this seems like a nice option in case you want one.

## General usability:
So now let's talk a bit about the general usability aka Calls, SMS, Battery life, performance and so on.

- **Battery:** This was a huge issue when I received my device (PostmarketOS CE) but it got a LOT better since then. With a SIM card in the device and WLAN disabled I can use it for a day but if I use the screen to much it sometimes dies a bit early. So in short still not perfect but usable enough for me.
-  **Calls:** Till lately I had issues with calls but currently it seems to work just fine. I can recieve calls and my device wakes up basically instantly and in terms of signal strength I never ran into any issues. Keep in mind tho that the Pinephone doesn't support all providers that well so you could potentially run into issues.
-   **SMS:** These work perfectly for me for a while now but I am not that sure about MMS. I never write long texts over SMS and would never ever even think about sending pictures over it so I can't really tell you how well they work. I still wait damn hard for the Matrix implementation to Chatty and seriously hope they also get calls working because I prefer it over the old unsecure methods of communication.
-   **Performance:** Now that's a bit more tricky to answer then the other ones specially in a blog post. I would recommend you to watch videos from Linmob or Martijn if you want to actually see it but I will do my best to describe it here to. My PostmarketOS Phosh install on the internal storage runs surprisingly well in my experience. Almost all of the big lags are gone and the device feels decent for the most part. Scrolling can still feel a bit shitty and sometimes you have minor lags but the system and system apps with the exception of Gnome Software and Megapixels tend to run absolutely acceptable in my opinion. Some apps and heavy websites obviously make issues but that's not really the fault of PostmarketOS or the Pinephone and probably won't change much any time soon. WebkitGTK still sucks and makes many Gnome apps that make use of web technologies run very poorly but in most cases you can just disable Javascript to make it usable. In case the a bit more sluggish experience isn't something for you you should probably not buy a Pinephone or wait another year. Obviously the Pinephone will never be able to keep up with your Android or iOS flagship because the hardware just isn't there but so far every release of Phosh and Phoc improves performance a lot and so far I can't see much of a slowdown so we will have to wait and see how far people manage to push the Pinephones hardware software side :D
-   **Camera:** The camera works and it does so surprisingly well for the mostly FOSS software behind it but there is no comparison to a modern Phone camera. I am not a expert but as far as I know that has two origins because while modern Phone cameras are also better hardware then the Pinephones you also have to keep in mind that the only reason phone pictures look that good is software. A modern phone camera probably relies more on software then the actual hardware and if you look closely you can see it to. In short I wouldn't use the Pinephone to capture a moment because the basically total lack of color accuracy prevents me from doing so but it's enough to take a quick picture of something and look at it later.
-   **Screen:** I will start this point with you will probably disagree with me. I am a defender of 1080p screens for everything that isn't a huge TV covering up half your wall and see no reason to go beyond 720p on a phone. Yes you will probably see the difference if you put a 720p and a 1080p display side by side but let's be honest it's a damn phone and as long as it's not under 720p this will have absolutely no effect on the usability or experience. Generally the Pinephone screen is a bit dark in direct sunlight but beside of that just good and idk why I would want a different one.
-   **Alarm Clock/Reminder:** This one may sound odd to you but because of deep sleep it's a actual issue. A few weeks ago the demo app Alarm Mobile came out but it relies on SystemD and from how it currently looks I expect the Gnome Clock implementation to work the same. That means the SystemD free PostmarketOS will need a custom implementation and that sucks specially for something so essential. I always use my Phone to wake up and even to set reminders when I cook and stuff like that so I really hope that PostmarketOS will also get a solution for that soon.

| ![](https://gateway.pinata.cloud/ipfs/QmXbrKBb94Rt7fHAT9vV7xgaCwASBVN62EiyS5naaqCbuH/20210411_16h37m27s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXbrKBb94Rt7fHAT9vV7xgaCwASBVN62EiyS5naaqCbuH/20210411_16h37m41s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXbrKBb94Rt7fHAT9vV7xgaCwASBVN62EiyS5naaqCbuH/20210411_16h36m34s_grim.png) |
|-------|-------|-------|
