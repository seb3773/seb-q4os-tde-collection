# Archived Article

**Original URL:** https://all-things-linux.blogspot.com/2014/11/q4os-debian-stable-with-trinity-desktop.html  
**Source:** All Things Linux Blog  
**Author:** Anonymous  
**Date:** Thursday, 27 November 2014  
**Archived:** February 2025

---

# Q4OS: Debian Stable with the Trinity Desktop Environment

**Author:** Anonymous  
**Date:** Thursday, 27 November 2014

---

Q4OS is like Exe GNU/Linux a distribution using the Trinity desktop and based on Debian Stable. In fact I could have picked Exe as well for review but Q4OS just had a new release and it looks cleaner from the start. It was simply the novelty factor that pulled me towards it and it's got a few nice touches of its own as we shall see. Version 0.5.20 was just released on 11/11/2014 and is available both for the mainstream 32 (i386) and 64-bit architectures. The images are a modest 314MB and 337MB respectively which makes for a speedy download and will definitely fit on your CD or even older USB sticks.

Hardware requirements are quoted as equivalent to a 300MHz Pentium, 128 MB Ram and 3GB of hard drive space minimum. Nice one, that should cover almost every PC still out there. The word lightweight may be overused these days but the above seems very light indeed, and the old KDE3/TDE clone runs like a champ on more modern hardware with a few cores at the 2GHz level. You might be forgiven to think it's Xfce or Openbox performance-wise. The distributed ISO's are installation media only and do not offer a live session.

Once booted up, the only option is to proceed with the old ncurses based Debian installer, a graphical install environment is not provided. That may sound a bit offputting to novice users, but bear in mind that this custom distribution is aimed at businesses that want a traditional, sane desktop environment for their workers (who probably have used a former iteration of KDE for a long time) and have IT staff to install. Also, veterans should not have any problems if they've ever installed Debian or Redhat in the days before graphical installers. If you're a relative newbie, no need to panic. The graphical installer in Debian is essentially the same, using similar steps so this should feel very familiar. That means LVM is supported as well. There's also the option of an automated install which takes care of everything and just leaves us with the task of rebooting and logging in to our new system. Very handy. Unfortunately if you go down this route neither a separate home partition nor a user is created and you'll have to add one later on yourself. At the end of the install you're prompted to create a root password though which we will use to log in the first time and an 'adminq' account is created with sudo rights. The initial install is around 1.9GB. My suggestion would be to add a step to the automatic install that calculates available space for a home partition based on percentage of the size of the drive, but that may be more trouble than it's worth and will not suit everybody either.

Once you've logged in you get a welcome screen like above and are presented with a very clean and tidy desktop reminiscent of Windows 2000 Professional and KDE 3. So yes, we're going back a long time but this is what people who do actual office work are comfortable with quite often and do not necessarily want to change. In the interest of efficiency and production, this is good. I remember when my organisation moved over from Windows 3.11 to NT and everybody, from heads of departments to secretaries, was trained for three days in groups of five. That's a lot of time and money to retrain in an organisation of 1200 people. Time that these people are not available to do their jobs.

In addition, Q4OS prides itself in long-term stability and in offering "a strong foundation for complex third-party applications". That probably refers to the stability of the Debian 7 foundation which should still be supported for a few good years if reaching LTS status as is to be expected. There are very good reasons for this assumption but that's another story. Even without, the current Debian Stable will still be supported for at least 1 year and a half. Commercial support, customizations and core level API programming can be purchased from Q4OS the company and presumably they will keep supporting this release even after Debian 7 is officially retired. That makes it very attractive for business. Due to the long-term support and its small footprint it is also marketed as an ideal virtual host. Under the hood is the default stable 3.2 kernel.

The OS detected immediately that it was running in VirtualBox and offered to download and install the guest additions, which it did. It was a nice touch not to have to hunt for and mount the guest additions iso myself and the whole process of compiling kernel modules completed without errors on my Debian Stable host. After that I had full screen 1366x786 resolution on my laptop. Q4OS asks for permissions before downloading and installing in a dialog again somewhat reminiscent of the Windows installers. As the system only comes with Konqueror as the default browser I opted to install Google-Chrome as well and after granting permissions the application installer set up the necessary repositories behind the scenes. It all finished smoothly and without a hitch.

A few supported applications are listed on the project's download page and I noticed that Chrome received its own submenu with an uninstall entry in the programs section, as well as being listed in Accessories/Internet. Bit strange to have applications listed as accessories but hey, not really a problem. Apart from that the menu is quite barren and basically what you get is a slim and trimmed down Trinity Desktop Environment with not much else than a browse, console/terminal program and admin tools in the Control Panel, with network connections and such. Cups is installed as the default printing system. You also get a nicely laid out, clean menu, Krusader for two-pane file management, the Kwrite text editor, Htop for process viewing and few other small utilities like Klipper, Kuser for managing accounts and wpagui for wireless. All the KDE 3 wallpapers and a few specific to Q4OS are included. Apparently there's also a script included that allows to easily add KDE 4, pulling in the whole software compilation as a meta-task, but I can't help feeling this would be counterproductive to the good experience so far. There are other distributions for that.

That's it. It's a good base to build your own if you like stability and the classic desktop TDE offers, a small footprint, low resource usage but still with a lot of functionality at your finger tips as the desktop environment can be extended with additional plugins to the control centre and all the old KDE programs like a messenger, Ktorrent for torrenting, a PIM etc. Give this a try if GNOME Shell and KDE 4 make you despair, Xfce does not cut it and window managers are far too basic for your needs.

**Addendum:** In response to questions, TDE is very stable and well integrated into the underlying Debian system in comparison to when added to other systems like RHEL 6 retrospectively. No crashes or bugs were experienced.

The project has just released an update to 0.5.21.

---

**Labels:** debian, desktop, kde3, linux light, TDE, trinity
