+++
title = "Glazing tools, Part I: KDE & Kinoite"
description = "Sharing some love on tools that make me feel comfy"
date = 2026-07-26
draft = false

[taxonomies]
tags = ["glazing", "fedora", "kde"]
+++

I have been wanting to write some blog posts for a long time now, and I haven't been entirely sure what to write about. So I've decided to let happiness win for once and write about stuff I love in this series.

Turns out there are a lot of tools that I have replaced over the ~10 years I've spent in computer science, and that I don't think I could ever come back to, given how great their replacements are. Hence the "Part I": I just don't see myself finishing this article in my lifetime if I have to list all of them (especially since the list keeps moving as some parts get replaced).

I have decided that this first article would be about the software I am most fond of: Fedora Kinoite and KDE.

## What is a "good tool" anyway?
The easy answer would be that it's whatever works for you, so I'll just give you my list of criteria when I'm evaluating software.
- Is the software easy to install through package managers I already have on my machine (brew, dnf, flatpak)? If not, I am not using your project.
- Are the default settings sensible, or do I have to tweak your project for hours to make it work? This also includes configuration files. I like to have choice, but I want the choices you make for me to be good enough as well.
- Is my distro already shipping something similar? If so, you can be 99% sure it won't touch my system.
- Does it work well? It should be fast and not crash every day. If it doesn't, I'll probably find an alternative in a couple of weeks and yeet it off my computer.

Overall, I just don't like installing new stuff on my machine unless I actively encounter issues with what I'm using right now. I also like my routine, and I have a job, which means I don't want to spend hours learning something that I am not absolutely sure will make my life easier. This is what has kept me from investing my time in [Jujutsu](https://www.jj-vcs.dev/latest/) & [NixOS](https://nixos.org/).

## Distro-hopping

Having said that, I really like the software I use to be as up-to-date as possible. I experimented with a ton of different distros at the start of my computer journey, trying to find the right balance between stability and up-to-date packages.

Here are the ones I can remember running:
- [Debian](https://www.debian.org/)
- [Ubuntu & almost all variants](https://ubuntu.com/desktop/flavors)
- [ChaletOS](https://archiveos.org/chaletos/)
- [Zorin](https://zorin.com/os/)
- [Linux Mint](https://www.linuxmint.com/)
- [Manjaro](https://manjaro.org/)
- [MX Linux](https://mxlinux.org/)
- [Pop!_OS](https://system76.com/pop)
- [SliTaz](https://www.slitaz.org)

I was getting burnt out from distro-hopping every other week and couldn't find anything that really satisfied me. For some reason, I had never touched [Fedora](https://fedoraproject.org/) — I thought it was some kind of niche distro, especially since it was backed by Red Hat. I finally decided to give it a try anyway.

## 🎩 Fedora my beloved

Fedora has been the only distro I have installed on my machines for around 4 years now. The up-to-date packages (especially the DE), the polish on the system, the easy updates (Ubuntu used to explode whenever I tried to run `sudo do-release-upgrade`) — it's all been super great.

I first gave [Fedora Silverblue](https://fedoraproject.org/atomic-desktops/silverblue/) a try around 2023, which was inconclusive as I had trouble wrapping my head around how to properly install my packages and all that. I decided to give it another go around a year ago — this time using `brew` for CLI tools — and given that I had grown tired of GNOME for a ton of different reasons, I started using [Kinoite](https://fedoraproject.org/atomic-desktops/kinoite/) instead.

It works like a charm. I can roll back my kernel and **all of my packages** if something goes wrong — it <u>never</u> has — and most importantly, it forces me to manage my packages *the right way*: Flatpak for GUI apps, brew for everything else.

My `dnf` packages are the ones shipped with my distro. I don't touch them at all, I don't risk hitting dependency hell, and I will simply *never* run into conflicts. Some might say it takes a bit more disk space to run all that — that installing my `brew` and `flatpak` packages through DNF on a regular Fedora install would use less — but I couldn't care less. I have a 1TB SSD inside my laptop, and I will never use more than half of it, even after several years.

Also, it means if a `brew` package exists on my Mac I can almost certainly install it on Kinoite too, and use it for my personal projects.

> Just to drive this point home: I do not have to hunt for a `.deb` or a `.rpm` file anymore. Like, it hasn't happened to me in a year and a half since I started using immutable Fedora installs. This is such a relief I cannot overstate it.

If I need a mutable system, or some kind of sandbox (which I do when I run Kali for pentesting), I use [Distrobox](https://distrobox.it/), which works without hiccups. I understand the concepts behind dev containers, but old habits die hard, so besides the Kali container, I run everything on my bare OS.

Bottom line: it's super stable, it's up-to-date, and it ships with nearly everything I need.

## Moving away from GNOME

I have tried quite a lot of DEs over the years — even though I have always been repulsed by tiling window managers, since I have a mouse and might as well use it — and they all had issues:
- no support for Wayland (which means some GUI apps have weird bugs)
- low maintainer count, which means there aren't a ton of new features and bugs take a long time to get fixed
- old design that makes me feel like I'm on a 2006 computer running Windows XP (and not in a good way)
- bad integration of themes across the whole UX: half-themed taskbar icons, missing animations, few customization options

> I do use Windows and macOS pretty much daily. I work on macOS during my day job, and I run Windows to play games. Even though those systems have flaws that sometimes create friction, they also bring stuff that I now just expect from any serious project — and almost all DEs miss the mark.

For years I used GNOME, especially when I was still a student: the gestures and the fact that there was pretty much nothing on the screen besides the small top bar meant I could have as much free screen space as possible to display my content. And on a setup where I only had my laptop screen to work with, GNOME was the most efficient way of navigating my windows when I was in class, which made it my go-to DE for around 3 years.

But now things have changed. I work remotely, and almost never use my laptop without peripherals. I don't really *need* the gestures. Now that I have a proper mouse and keyboard I'd rather have a DE that is actually feature-complete.

{{ figure(src="/photos/kde/desk-setup.avif", alt="My desk setup", caption="My desk setup — fucking awesome.") }}

I grew tired of having to install plugins for every basic task, especially since they pretty much all broke whenever I updated Fedora (which I never understood — every version has a preview for several weeks). Like, come on, I need a plugin for the taskbar to show up without me pressing the Super key?

## KDE

So the only DE that was left for me to use was KDE. And it has been so much better overall, oh my god. It's like the Windows 7 feeling, but modern and complete. I get a ton of customization options (I don't use many, but I like to change some stuff) and most importantly it is **complete, out of the box**. I don't need *any* plugin, and I don't have any. Everything I need is already available, and more! Here is a non-exhaustive list of stuff that, in my opinion, is unmatched anywhere else.

### KDE Apps

[Konsole](https://apps.kde.org/konsole/) ships with KDE, works out of the box, and is highly customizable (with a UI and not a config file, looking at you [Ghostty](https://ghostty.org/)). I can split panes, open tabs, it looks good, and I can replicate my input across panes if needed, which has saved me so much time during production outages in my past job.

[Okular](https://apps.kde.org/okular/), [Skanpage](https://apps.kde.org/skanpage/) & [KWrite](https://apps.kde.org/kwrite/) do exactly what I expect from a PDF viewer, scanner interface, and notepad. They each do one thing, and they do it well.

[Gwenview](https://apps.kde.org/gwenview/) allows me to crop an image, rotate it... Basically what I have been able to do on my phone for ages to edit photos, I can do directly from there. The rest of the time, if I just want to open an image, it stays out of my way. I know there's software to do that on other OSes, Linux included, but it's packaged by default on my system!

> It's not a shitty image viewer with no tools at all, one that would force me to look for an alternative, install it, and then leave it sitting on my computer for ages until I need it again in 3 months.

[Plasma System Monitor](https://apps.kde.org/plasma-systemmonitor/) allows me to add panes and customize it as I need if I want more data — but with sensible defaults. This is crazy, but before I used KDE I couldn't even imagine it would be possible (let alone an improvement) to customize a system monitor.

### The little details that add up

Taskbar customizations: I don't change a ton of settings there, but I have a simple media player integration and a per-core CPU graph. I can get rid of system icons I don't want and just tuck them in a foldable menu. It does exactly what I want. When I plug in a wireless controller, it shows the remaining battery (crazy to me that Windows hasn't added that yet).
{{ figure(src="/photos/kde/kde1.png", alt="KDE audio panel showing per-device and per-app volume controls", caption="Device and app volume control in the same panel? You can even test your mic in there!") }}

The settings app: everything is in there, I love it. It's just one app that has all of my system settings in one place. Given how many dialogs I have to go through to do basic stuff on pretty much every other system (except macOS, which just... locks you out of tons of options) it's a breath of fresh air to have the Settings app actually allow me to change my settings.
{{ figure(src="/photos/kde/ksettings.png", alt="The KDE System Settings app on its Quick Settings page, showing theme, animation speed and click behaviour options, with every settings category listed in the sidebar", caption="How hard was it to do the same, Microsoft? smh my head") }}

KInfoCenter: I can actually get details on every component of my system right from a single app. Do you know how many times I've had to run obscure software on my friends' computers to get a somewhat complete list of the hardware they have? This is a lifesaver as well. When I troubleshoot my friend's grandpa's computer, I can just open this bad boy up and check which hardware they have before ordering a replacement.
{{ figure(src="/photos/kde/kinfocenter.png", alt="KInfoCenter's Memory page, listing each RAM module in full: type, size, speed, voltage, manufacturer and part number", caption="Look at all the info I can get on my RAM, I never saw so much with any other GUI tool. It's so efficient.") }}

## Conclusion

Overall, those are all the things that make my computer feel comfy. I don't need to install a lot of external tools; pretty much all of the features I want are already packed in — until new ones I didn't even realize I needed are added by the KDE team.

I hope my article has convinced you to give Kinoite — or at least KDE — a try, especially if you don't play games that require kernel-level anticheat. If you do, installing any distro on your gaming computer is not a good idea. 

> Also, you should know some of those anticheats have [already been abused in the past](https://www.trendmicro.com/en_us/research/22/h/ransomware-actor-abuses-genshin-impact-anti-cheat-driver-to-kill-antivirus.html) to push malware on your beloved war machine.

If you're not one of the unfortunate people stuck on Summoner's Rift or Genshin Impact, I want to tell you that the people I know who moved away from Windows to Kinoite have never felt better using their computers. You could be feeling just like them if you give Linux a try!

And if you're already using KDE and are enjoying it as much as I am, consider [making a donation](https://kde.org/donate/).

*See you next time, and in the meantime, take care* ( >؂•̀ )

Téo 💖
