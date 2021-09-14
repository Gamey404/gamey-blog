+++
author = "Gamey"
title = "Fractal on the Pinephone."
date = "2021-01-23"
description = "A short guide to using the matrix client Fractal with encryption on the Pinephone."
tags = [
    "Pinephone", "ArchLinux", "fractal",
]

+++

# Fractal Encryption and Keyring fix on the Pinephone
Today I want to take a look at a fantastic Matrix client on the Pinephone and show you workarounds for it's main two issues. Fractal is a awesome Matrix client for Gnome and Phosh but it currently lacks support for encryption and on Phosh it can't open the Gnome Keyring (safe your login). Luckily there are workarounds for those two issues and those are what this post will focus on. If you want to know more about all current options to use Matrix on the Pinephone I made a post about them a while ago which is linked down below.

## [Pantalaimon](https://github.com/matrix-org/pantalaimon/) for Encryption
Pantalaimon is a E2EE aware deamon proxy for Matrix messengers. You can use it to enable E2EE in clients that actually don't have encryption implemented yet. You probably guessed it, I will show you how to use Pantalaimon for Fractal now so you can use it for secure chats.

1. Before you can install Pantalaimon you need libolm (The matrix encryption library). If your distro provides a package for it use that and if not you can find instructions [here](https://gitlab.matrix.org/matrix-org/olm/blob/master/README.md).
2. To install Pantalaimon I will use [the source code](https://github.com/matrix-org/pantalaimon) because the part of Pantalaimon that handles session verifying (panctl) broke a while ago and we need the latest version to fix that. Well I couldn't get it to work with thenewest version ether but probably my fault or something.
3. Now you need a configuration file for Pantalaimon which should be placed in ``~/.config/pantalaimon/pantalaimon.conf`` (You have to create the folder first). I will only make a minimal one but you can find more details on the configuration options [here](https://github.com/matrix-org/pantalaimon/blob/master/docs/man/pantalaimon.5.md). A minimal config file for Pantalaimon looks like this:
```
[local-matrix]
Homeserver = https://yourhomeserver.xyz
ListenAddress = localhost
ListenPort = 8010
```
4. Now you can start the Pantalaimon deamon by simply typing ``pantalaimon`` in a Terminal (setting up auto start is probably a good idea but thats to distro specific for this post).
5. Now you can start Fractal and where your Homeserver would go you simply put http://localhost:8010 (I think it failed for me so I had to get the exact local address from the Pantalaimon deamon).
6. You could just stop here but there are a few optional steps left to verify your Pantalaimon session. To do so you will need a tool called panctl which should be included in Pantalaimon and a verified device. Sadly it refused to list the servers for me so ether I have been lied to about the fix in the latest version or I fucked up somewhere.

## [Seahorse](https://wiki.gnome.org/Apps/Seahorse) as workaround
The Gnome Wiki describes Seahorse as "a GNOME application for managing encryption keys and passwords in the GNOME Keyring." The main point for us is that it unlocks the Gnome Keyring and since Fractal only has issues doing that we can use Seahorse as workaround.

1. Install seahorse and fractal (should both be in all repos).
2. Start Fractal and log in like you usually would.
3. Now use ``scale-to-fit seahorse`` and check if it worked.
4. From now on you can always just unlock the "Default keyring" with Seahorse before starting Fractal!

## More:
- I made a post about the different options to use Matrix on the Pinephone which you can find [here]().
- A detailed description of Pantalaimon can be found [here](https://github.com/matrix-org/pantalaimon/blob/master/docs/man/pantalaimon.8.md).
- [This](https://www.cogitri.dev/posts/10-pantalaimon-setup/) amazing blog post helped me a lot. It's a tutorial that shows how to install Pantalaimon for Fractal.

### Screenshots:
Here are a few screenshots of Fractal and Seahorse.

| ![](https://gateway.pinata.cloud/ipfs/QmXKD8BAG5r2CAxtSWYs37L6UwpypoL77iiZCzxFKzK7Pt/20201017_04h05m22s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXKD8BAG5r2CAxtSWYs37L6UwpypoL77iiZCzxFKzK7Pt/20201218_12h50m36s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXKD8BAG5r2CAxtSWYs37L6UwpypoL77iiZCzxFKzK7Pt/20201017_04h09m00s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmXKD8BAG5r2CAxtSWYs37L6UwpypoL77iiZCzxFKzK7Pt/20201017_04h05m22s_grim.png) |
|-------|-------|-------|---|
| ![](https://gateway.pinata.cloud/ipfs/QmTZukJAcsvxGJKDGJdppjm6fQMcrVCasaX2Xh8vusUqLN/20210123_15h51m23s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmTZukJAcsvxGJKDGJdppjm6fQMcrVCasaX2Xh8vusUqLN/20210123_15h51m39s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmTZukJAcsvxGJKDGJdppjm6fQMcrVCasaX2Xh8vusUqLN/20210123_15h52m47s_grim.png) | ![](https://gateway.pinata.cloud/ipfs/QmTZukJAcsvxGJKDGJdppjm6fQMcrVCasaX2Xh8vusUqLN/20210123_15h53m15s_grim.png) |


### Thanks to:
- @jason123santa:matrix.org for telling me about Seahorse!
