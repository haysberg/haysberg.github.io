+++
title = "Praising tools (Part I) : Unoriginal list"
description = "In which I praise my OS"
date = 2026-07-25
draft = true

[taxonomies]
tags = ["tools", "linux"]
+++

I have been wanting to write some blog posts for a long time now, and I was not entirely sure what to write about. So I've decided to let happiness win for once and write about stuff I love.

Turns out there are a lot of tools that I have replaced over the short years I've spent in the industry, and that I don't think I could ever come back to, given how great their replacements are. Hence the "Part I" : I just don't see myself finishing this article in my lifetime if I have to list all of them (especially since the list keeps moving as some parts get replaced).

I have decided that this first article would be for the non-moving parts of the list, and those have to be immutable Fedora, KDE, Flatpak and Zed.

# What is a "good tool" anyway ?
The easy answer would be that it's whatever works for you, so I'll just give you my list of criteria when I'm evaluating software.
- Is the software easy to install through package managers I already have on my machine (brew, dnf, flatpak) ? If not, I am not using your project.
- Are the default settings sensible, or do I have to tweak your project for hours to make it work ? This also includes configuration files. I like to have choice, but I want the choices you make for me to be good enough as well.
- Is my distro already shipping something similar ? If so, you can be 99% sure it won't touch my system.
- Does it work well ? It should be both fast and not crash every day. If it doesn't, I'll probably find an alternative in a couple of weeks and yeet it off my computer.

Overall, I just don't like installing new stuff on my machine unless I actively encounter issues with what I'm using right now. I also like my routine, and I have a job, which means I don't want to spend hours learning something that I am not absolutely sure will make my life easier. This is what has kept me from investing my time in [Jujutsu](https://www.jj-vcs.dev/latest/) & [NixOS](https://nixos.org/).

## Kinoite and immutable Fedora variants
Having said this, I really like the software I use to be as up-to-date as possible. I experimented with a ton of different distros at the start of my computer journey, trying to find the right balance between stability and up-to-date packages.

After trying out a shit ton of Ubuntu variants, then testing Arch, Manjaro and Debian, I was getting burnt out distro-hopping every other week, until I finally decided to try out [Fedora](https://fedoraproject.org/).

Fedora has been the only distro I have installed on my machines for around 4 years now. The up-to-date packages (especially the DE), the polish on the system, the easy updates where Ubuntu used to explode whenever I tried to run `sudo do-release-upgrade` — it's been super great.

I first gave [Fedora Silverblue](https://fedoraproject.org/atomic-desktops/silverblue/) a try around 2023, which was inconclusive as I had trouble wrapping my head around how to properly install my packages and all that. I decided to give it another go around a year ago — this time using `brew` for CLI tools — and given that I had grown tired of GNOME for a ton of different reasons, I started using [Kinoite](https://fedoraproject.org/atomic-desktops/kinoite/) instead.

It works like a charm, I can roll back if something goes wrong (it <u>never</u> did), and most importantly, it forces me to manage my packages *the right way* : Flatpak for GUI apps, brew for everything else.

If I need a mutable system, or some kind of sandbox (which I do when I run Kali for pentesting), I use [Distrobox](https://distrobox.it/), which works without hiccups. I understand the concepts behind dev containers, but old habits die hard, so besides the Kali container, I run everything on my bare OS.

Bottom line : it's super stable, it's up-to-date, and it packages nearly everything I need directly on install.

I wanted to add a section praising the whole uBlue / bootc ecosystem, but I will keep that for a dedicated article, as this is somewhat linked to stuff I do for work as well.

## KDE

## Flatpak

## Zed

The first real code editor I have used in my programming courses (around 2016) was [Atom](https://atom-editor.cc/). At the time, I really enjoyed moving my editor panes around, the way it was so pretty compared to its competition —not counting Jetbrains IDEs, as those are paid software—, the automatic highlighting, the complete settings...

After two years of loving relationship however, I grew tired of it. It was getting slow, and the minimalistic UI was not giving me enough under my fingers. So I jumped off the Atom train and moved to what stuck as close as possible to the philosophy I described at the start of this article at the time, [Visual Studio Code](https://code.visualstudio.com/).

At first, it was awesome, and this time I stuck to it for around 4 years. It was faster, with more features, a thriving plugin ecosystem to handle a ton of different tools, I found it better in every way. 

But after some years, I started to see it feel less and less snappy, and I had to fight with quite a lot of plugins just to handle my everyday work. Growing more and more concerned about my privacy, and not being able to sync my settings between instances when using VSCodium meant I stayed Microsoft's hostage for around a year, where my IDE was working, but not as good as I wished.

Fast forward to 2023, and I stumble upon a Rust-based, GPU accelerated IDE that looks like VSCode and Jetbrains IDEA had a baby. Basically all I have ever wanted... I couldn't believe it !

Turns out, the Zed IDE on paper was everything I had ever wanted, but it was in very early stages and just couldn't do the job properly. So I stayed on VSCode again, relunctantly, until I put my hands on Zed once again around a year and a half ago, and oh my god, there's been so much work on this project. Everything I need works. It's so snappy I literally couldn't believe it at first.

I can :
- completely disable AI features in a single click (I'm not against using AI code, I just don't want any of it inside my IDE)
- sync my config accross multiple machines by logging in my GitHub account
- install extensions in a single click when opening an unsupported file type (even though most of them are)

And the UI is so... so efficient. Blocky but modern, with the right amount of contrast (I use the default light mode theme), buttons that feel that they belong where they are in the window... I just don't see what could make me drop this absolute gem.
