# Archived Article

**Original URL:** https://www.theregister.com/2023/11/02/trinity_desktop_q4os/  
**Source:** The Register  
**Date:** Thu 2 Nov 2023 // 10:15 UTC  
**Archived:** February 2025

---

# Trinity Desktop's Latest Release Snaps into Action on Q4OS 5.3

**Author:** Liam Proven  
**Date:** Thu 2 Nov 2023 // 10:15 UTC  
**Source:** The Register

---

A new version of the Trinity desktop is out, with a new window-snapping feature. And that's not the only way it's snappy.

The Trinity Desktop Environment (latest release 14.1.1), or TDE for short, is a fork and continuation of KDE version 3.5, the last release of KDE 3. It's loosely comparable to MATE, which is a continuation of GNOME 2 after the developers moved on to the radically different GNOME 3. KDE 4 wasn't as radical a change, but it introduced a significantly different design based around customizable widgets called "plasmoids." In 2010, The Reg described the change thus:

> Something strange happened to KDE in the last decade. Ten years ago it was a robust, decidedly unglamourous desktop. The design was very German. It worked. They took pride in that, and not being like the flakey and fancy Gnome kids.
>
> Then they went mad. They went 4.0.

When we mentioned the release of TDE 14.0.11 and TDE 14.0.12, we linked to some other folk similarly disenchanted with KDE 4, including Linus Torvalds himself. Enough people preferred the relatively simple design of the older KDE that they have kept it alive, modernizing it just enough to run on current distributions. Like MATE, development is active, with minor new features and things appearing occasionally, but not sweeping changes – which is what you'd expect from teams who liked things the way they were enough to keep older versions alive.

The most visible new feature in this release is window snapping, which the release notes compare to Windows' Aero Snap. This is a love-it-or-hate-it sort of feature, and The Reg FOSS desk is in the fan faction; we find it useful, and a welcome addition.

TDE is available in most of the usual suspects: Debian, Ubuntu, Arch, Fedora, and so on. As you might expect, it's supported in several distros which are or were KDE-centric, including openSUSE, Mageia and PCLinuxOS.

It's also the default desktop of a couple of distros, including the Devonian Exe GNU/Linux, based on Devuan, and Q4OS, based on Debian itself.

## Q4OS Overview

Q4OS is simple and pleasantly plain, but not to the degree of Windows 95-level austerity. The Reg took a look at Q4OS 2.4 almost exactly six years back, but that's long enough ago we decided on another look. Q4OS 5.3 came out about two weeks ago, although the project's website doesn't seem to have been updated to indicate this yet. There are three different editions of the distro: two 64-bit versions, with either TDE or KDE Plasma 5, and a 32-bit edition which only offers TDE.

It offers modern niceties such as a Software Centre, and you can switch the Start menu layout, themes and so on.

Q4OS is a combination of existing parts, so we won't go into exhaustive (and exhausting) depth. It's based on Debian 12 "Bookworm" with kernel 6.1. The 64-bit edition boots into a live environment, while the 32-bit one booted into the text-based Debian installer just with fewer questions. If you choose to install, it runs the Calamares installer used in multiple other distros from OpenMandriva to siduction, which is friendly and simple.

## Testing

We tried the 64-bit edition in the latest VirtualBox, and on the metal on an old Thinkpad W500: a Core 2 Duo with 8 GB of RAM and an old, small SSD. We tried the 32-bit edition on the lowest-end PC in the FOSS desk test fleet, a Sony Vaio P, an Atom with 2 GB of RAM, and although installation was much slower on this machine, it worked fine on all of them. It has VirtualBox graphics drivers pre-loaded, so the VM was resizable and ran smoothly. On the metal, it's a midweight distro rather than super-lightweight, but it's commendably easy.

The new tiling functionality in TDE R14.1.1 is very handy, for example in the common situation of copy-pasting commands.

Q4OS idles at about 600 MB of RAM in use, which isn't bad – it's rather more than Reg lightweight fave the Raspberry Pi Desktop, the x86 PC version, which takes about a third as much RAM. On the other hand, TDE is a much richer desktop than LXDE, and offers better customizability. It uses about 6.5 GB of disk space, which isn't too punitive for 2023.

The OS connects to Wi-Fi during installation and updates itself, so once installed, no updates were pending and we found we had the latest TDE 14.1.1. On all our test devices, it correctly configured all the hardware, and plays a startup sound to show it's working.

This vulture isn't the greatest fan of KDE, and even back when KDE 3 was current, we felt it was cluttered with options to tweak. For instance, connecting to Wi-Fi took us three goes, because we didn't notice that there were two separate buttons for "Next" and "Continue," only one of which prompts for a network password. There are two web browsers provided, Chromium and KDE's own Konqueror file manager, which is also a browser, and three different start menu layouts available. This sort of duplication feels redundant, but like Perl, "there's more than one way to do it" seems to be the KDE way.

## Verdict

Saying that, though, TDE works well, even on the very slow Poulsbo graphics of the Vaio P. We are quite impressed by Q4OS: it's easier to install than Debian itself, lighter and quicker, and easy to work with. It eschews modern shiny for traditional functionality, which is a very welcome change.

Back in the days of KDE 2, our favorite version was the customized edition provided with Xandros – you can see some screenshots in The Reg's 2004 review. We were recently surprised to discover that Linspire, later owned by Xandros, is still going. If Linspire has access to Xandros's customized KDE, these teams could work together and make something amazing. But even so, it's pretty good as it is. ®

---

**Tags:** Debian, Linux, Open Source
