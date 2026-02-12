<div align="center">

# ⚙️ <span style="color: #2E86AB;">Q4OS Setup and Using</span>

### <span style="color: #6C757D;">Trinity Desktop User Manual</span>
*<span style="color: #A23B72;">Revision 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source of document: <a href="https://www.q4os.org/dqa007.html" style="color: #2E86AB;">https://www.q4os.org/dqa007.html</a>
</p>

</div>

---

## 📑 <span style="color: #2E86AB;">Table of Contents</span>

1. [Introduction](#1-introduction)
2. [Testing](#2-testing)
   - 2.1. [Live CD](#21-live-cd)
   - 2.2. [In Virtualbox](#22-in-virtualbox)
3. [Installation](#3-installation)
4. [Wireless network setup](#4-wireless-network-setup)
5. [Print and Scan](#5-print-and-scan)
   - 5.1. [Hewlett-Packard printers and scanners](#51-hewlett-packard-printers-and-scanners)
   - 5.2. [Other printers](#52-other-printers)
   - 5.3. [Scanners](#53-scanners)
6. [Power management](#6-power-management)
7. [Hardware sensors](#7-hardware-sensors)
8. [Touchpad device](#8-touchpad-device)
9. [Proprietary multimedia codecs](#9-proprietary-multimedia-codecs)
10. [Proprietary video drivers](#10-proprietary-video-drivers)
11. [Users and groups](#11-users-and-groups)
    - 11.1. [Adding a regular user](#111-adding-a-regular-user)
12. [Android interconnection](#12-android-interconnection)
13. [Security updates, software management](#13-security-updates-software-management)
    - 13.1. [Update manager](#131-update-manager)
14. [External software repositories](#14-external-software-repositories)
15. [Alternative desktop environments](#15-alternative-desktop-environments)
16. [Adding more languages](#16-adding-more-languages)
    - 16.1. [Add languages](#161-add-languages)
    - 16.2. [User setup](#162-user-setup)
    - 16.3. [Example](#163-example)
17. [Miscellaneous tips](#17-miscellaneous-tips)
    - 17.1. [Kickoff start menu](#171-kickoff-start-menu)
    - 17.2. [Single click icons](#172-single-click-icons)
    - 17.3. [Desktop effects](#173-desktop-effects)
    - 17.4. [Autologin](#174-autologin)
    - 17.5. [Screen scaling](#175-screen-scaling)
    - 17.6. [Timezone selection](#176-timezone-selection)
    - 17.7. [Root password](#177-root-password)

---

## <span style="color: #F77F00;">1. Introduction</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

This paper covers how to set up, configure and use Q4OS operating system.

Q4OS is recommended to be used on production machines, as it has been built on top of the rock stable, secured and reliable Debian system tested by lot of people around the World.

There is a huge stable software base sitting in the default repositories - you are free to use it and adjust the system to suit your needs.

</div>

---

## <span style="color: #06A77D;">2. Testing</span>

### <span style="color: #06A77D;">2.1. Live CD</span>

If you want to get a quick Q4OS experience or test it within a real hardware, you can safely boot a Q4OS live CD or USB.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Safe Testing:</strong> It will write nothing into your hard drive and will not affect your existing installation. It's possible to install Q4OS system directly from live media using the live installer.
</blockquote>

---

### <span style="color: #06A77D;">2.2. In Virtualbox</span>

We recommend to install Q4OS inside [Virtualbox](http://www.virtualbox.org/) for testing purposes.

**Configuration:**
- Operating system: **Linux**
- Version: **Debian (32/64-bit)**

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tip:</strong> It's appropriate to setup "Virtualbox guest additions" within the guest system to achieve the best performance. There is a convenient auto-installer in the Q4OS 'Software centre' available. Installer contains optimized drivers and is preferred to install from original Oracle's or other sources.
</blockquote>

---

## <span style="color: #D62828;">3. Installation</span>

Please read Fresh Q4OS installation [setup guide](https://www.q4os.org/dqa018.html).

---

## <span style="color: #7209B7;">4. Wireless network setup</span>

Q4OS fully supports wireless networks and includes a tool called **tdenetworkmanager** to manage wireless connections. You can find it in the system tray.

If you have issues connecting to a wireless network, please read [wifi connection troubleshooting post](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #F77F00;">5. Print and Scan</span>

### <span style="color: #F77F00;">5.1. Hewlett-Packard printers and scanners</span>

Install HP Linux printing and imaging system, satisfy dependencies and setup a printer in terminal:

```bash
$ sudo apt install hplip hplip-gui avahi-utils cups
$ sudo apt install libcupsimage2-dev libdbus-1-dev libssl-dev libusb-1.0.0-dev python-dev
$ sudo hp-setup
```

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Note:</strong> Some HP printers require a downloadable driver plug-in. The 'hp-setup' command will download and install the plug-in automatically.
</blockquote>

---

### <span style="color: #F77F00;">5.2. Other printers</span>

First list drivers and choose the proper one for your model:

```bash
$ apt-cache search printer-driver
```

Install a specific set of drivers, for example Samsung laser printers:

```bash
$ sudo apt install printer-driver-splix cups
```

Or you can install all of available printer drivers:

```bash
$ sudo apt install foomatic-db printer-driver-all cups
```

Next add and configure printers:

```
Start menu → Applications → Settings → Print system
```

You can find valuable additional information at the [Debian wiki](https://wiki.debian.org/SystemPrinting).

---

### <span style="color: #F77F00;">5.3. Scanners</span>

We recommend to use **Kooka** application for scanning. Install required software and add any users who need access to the 'scanner' group:

```bash
$ sudo apt install libsane sane sane-utils xsane kooka-trinity
$ sudo adduser your_user_name scanner
```

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Important:</strong> A user will need to log out and log back in to take effect of the new group.
</blockquote>

Check the scanner is now recognized:

```bash
$ scanimage -L
$ sane-find-scanner
```

If you want to configure a network scanning, see [Sane over network](https://wiki.debian.org/SaneOverNetwork).

---

## <span style="color: #06A77D;">6. Power management</span>

It is desirable to install power control application for laptops and mobile devices:

```bash
$ sudo apt update
$ sudo apt install rfkill tdepowersave-trinity
```

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 15px 0;">

Login again, nice power control application will be present in system tray.

**Features:**
- 🔋 Control CPU frequency
- 📊 View battery status
- 💤 Configure sleep and hibernate actions
- 🔘 Handle lid close events
- ⚡ Power button configuration

</div>

---

## <span style="color: #D62828;">7. Hardware sensors</span>

Most computers come with various sensors, which can be used to watch your hardware and prevent it from unexpected fault. This is where **ksensors** application comes in.

```bash
$ sudo apt install ksensors-trinity
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

You will find 'ksensors' monitoring application in the Start menu or in the system tray.

**Features:**
- 🌡️ Temperature monitoring
- ⚡ Voltage sensors
- 🌀 Fan speed monitoring
- 🔔 Alarms and thresholds
- ⚙️ Actions on limits exceeding

</div>

Q4OS should recognize available sensors automatically out of the box. If not, you have to detect needed kernel modules:

```bash
$ sudo sensors-detect
```

You will be asked at the end of scan process if you want what it finds to be added to '/etc/modules' file. Answer 'yes' and then reboot.

---

## <span style="color: #7209B7;">8. Touchpad device</span>

Q4OS uses **libinput** driver to control touchpad and related pointing devices by default.

Check for the complete list of 'libinput' configuration options:

```bash
$ man libinput
```

All the options could be applied in the `/etc/X11/xorg.conf.d/60-libinput.conf` file.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Alternative: Synaptics Driver**

You can make an older 'synaptics' driver take precedence over 'libinput':

```bash
$ sudo apt install xserver-xorg-input-synaptics
```

Use default 'synclient' command-line tool to configure Synaptics touchpads:

```bash
$ synclient
```

To see all available options:

```bash
$ man synaptics
```

Example - disable touchpad's 'tap to click':

```bash
$ synclient TapButton1=0 TapButton2=0
```

</div>

For more detailed info please read [Debian documentation](https://wiki.debian.org/SynapticsTouchpad).

---

## <span style="color: #F77F00;">9. Proprietary multimedia codecs</span>

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 15px 0;">

Many codecs are already available in default repositories. These include codecs for:
- 🎵 MP3
- 🎬 H264
- 🔊 AAC encoding and decoding

If you want to install extra collection of professional quality codecs, you can run easy to use installer from **Q4OS Software Centre**.

Media players such as VLC and Mplayer make use of these codecs in order to provide support for playback of files encoded through these many different codecs.

</div>

---

## <span style="color: #06A77D;">10. Proprietary video drivers</span>

Install proprietary drivers to improve video performance and get full 3D acceleration. See [graphics card Debian wiki](https://wiki.debian.org/GraphicsCard) page for detailed instructions.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
🎮 <strong>NVIDIA Users:</strong> If you have a NVIDIA graphics card, you can run installer from Q4OS Software Centre. It will probe the hardware for related available drivers and install them in a user friendly way.
</blockquote>

---

## <span style="color: #D62828;">11. Users and groups</span>

### <span style="color: #D62828;">11.1. Adding a regular user</span>

Open "Users and groups" window:

```
Control Panel → System Administration → Users and groups
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Steps:**

1. Click "Add" button
2. Specify new username and fill user details
3. Assign users to specific system groups to specify user rights

**Recommended groups for new users:**
- `cdrom` - CD/DVD access
- `audio` - Audio playback
- `video` - Video devices
- `plugdev` - Removable devices
- `netdev` - Network management
- `powerdev` - Power management
- `lpadmin` - Printer installation
- `sudo` - Administrator permissions

</div>

---

## <span style="color: #7209B7;">12. Android interconnection</span>

Use **gmtp** application - fast and well arranged graphical file manager that connects most of phones and other Android devices to PC via USB cable.

```bash
$ sudo apt install gmtp
```

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Usage:**

1. Attach your device via USB cable
2. Set it as MTP device
3. Run 'gmtp' file manager

You will be able to browse internal directory structure and copy, delete and manage files from your Android device.

</div>

---

## <span style="color: #F77F00;">13. Security updates, software management</span>

Q4OS uses **Apt** package management system and related tools to maintain system health and clean. There is automatic unattended upgrades mechanism to get security and software updates quietly.

If you need to update your system immediately manually, issue commands in terminal:

```bash
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
📚 <strong>More Info:</strong> If you want to know how to install additional software, please follow 'Available Q4OS Applications' user manual, available from <a href="https://www.q4os.org/documents.html" style="color: #2E86AB;">Documents</a> section of the Q4OS website.
</blockquote>

---

### <span style="color: #F77F00;">13.1. Update manager</span>

Update Manager notify users about available security and software updates and let them to upgrade system on request.

You can easily install Update Manager from the **Q4OS Software Centre**.

---

## <span style="color: #06A77D;">14. External software repositories</span>

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Power Users Only:</strong> This chapter is intended specifically for power users familiar to Debian package management system.
</blockquote>

The default Q4OS configuration offers the basic and dependable set of software repositories. If you want to add more external repositories, you are free to follow standard Debian procedures.

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Example: Installing Opera web browser**

List available predefined repositories:

```bash
$ sudo qrepoadd --gui
```

Select 'opera' repository from drop-down combobox and click 'Ok' button. Alternatively:

```bash
$ sudo qrepoadd opera
```

Install packages:

```bash
$ sudo apt update
$ sudo apt install opera-stable
```

**To uninstall and disable repository:**

```bash
$ sudo apt autoremove opera-stable
$ sudo qreporm opera
$ sudo apt update
```

</div>

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Warning:</strong> Adding external third-party repositories is low level system action, and it could deeply influence package database integrity and dependencies. Fortunately Apt package management system contains strong tools for administrators to fix broken dependencies.
</blockquote>

---

## <span style="color: #7209B7;">15. Alternative desktop environments</span>

Other desktop environments integration into the Q4OS system is supported. They could be installed alongside the default Trinity desktop, for example:
- KDE Plasma
- LXQt
- XFCE
- And others

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Installation:**

You can add a desktop environment using the Desktop Profiler tool:

```bash
$ swprofiler.exu
```

Click on the right top corner button ">" to select desktop environment and install it together with a desktop profile.

**Switching Desktops:**

After reboot, users will be able to choose which desktop environment to log into:

1. On the TDM login screen, click 'Menu' button
2. Go to 'Session Type'
3. Select desired desktop environment

</div>

---

## <span style="color: #F77F00;">16. Adding more languages</span>

It's possible to add multiple languages into Q4OS and set different national environments for different users.

### <span style="color: #F77F00;">16.1. Add languages</span>

Administrator installs separate localization packages and users will be able to switch between different languages.

Run new language wizard from terminal (repeat for multiple languages):

```bash
$ addlanguage
```

If you have installed some applications having separate localization packages, install them as well. **Libre Office example:**

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-xx
```

**Optional - change global system locale and timezone:**

```bash
$ sudo dpkg-reconfigure locales
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #F77F00;">16.2. User setup</span>

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Step 1:** Pickup and set a locale (prefer UTF8 locales):

```bash
$ chqloc --list
$ chqloc --setlocale xx_XX.utf8
```

**Step 2:** Select new user language

Open "Country/Region & Language" dialog:

```
Control Panel → Regional & Accessibility → Country/Region & Language
```

Choose your country clicking the country button. It will set up the user's language as well as various national conventions (date/time format, currency, etc.).

**Step 3:** Select a keyboard layout:

```
Control Panel → Regional & Accessibility → Keyboard Layout
```

Login again - you will see your profile translated into the chosen language!

</div>

---

### <span style="color: #F77F00;">16.3. Example</span>

<div style="background-color: #E3F2FD; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

**Scenario:** Fresh installation of Q4OS with Libre Office suite installed. We would like to set-up German language.

**Step 1:** Run new language wizard to select German language:

```bash
$ addlanguage
```

**Step 2:** Libre Office lang pack:

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-de
```

**Step 3:** Set user's German locale:

```bash
$ chqloc --list
$ chqloc --setlocale de_DE.utf8
```

**Step 4:** Open "Country/Region & Language" dialog:

```
Control Panel → Regional & Accessibility → Country/Region & Language
```

Click first button with country flag and choose "Europe, Central → Germany".

**Step 5:** Select German keyboard layout:

```
Control Panel → Regional & Accessibility → Keyboard Layout
```

**Step 6:** Login again - your profile is now in German! 🇩🇪

</div>

---

## <span style="color: #D62828;">17. Miscellaneous tips</span>

### <span style="color: #D62828;">17.1. Kickoff start menu</span>

Well arranged, modern style start menu offers search bar, favorites tab, history and more.

To switch to Kickoff menu, right mouse click on system panel:

```
Configure Panel → Menus → Start menu style → Kickoff
```

You can restore default start menu the same way.

---

### <span style="color: #D62828;">17.2. Single click icons</span>

Icon activation by mouse doubleclicking is default in Q4OS. It's easy to set single click activation:

```
Control Panel → Peripherals → Mouse → General tab → Single click to open files and folders
```

---

### <span style="color: #D62828;">17.3. Desktop effects</span>

Turn desktop smoothing and beautifying effects on.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Note:</strong> Desktop effects will work flawlessly on modern hardware only. It's not recommended to use it with legacy hardware.
</blockquote>

Enable desktop effects:

```bash
$ ctrl-compmgr --enable
```

Disable desktop effects:

```bash
$ ctrl-compmgr --disable
```

---

### <span style="color: #D62828;">17.4. Autologin</span>

It is possible to bypass login screen and login specified user automatically after system boot.

See all possible options:

```bash
$ sudo ctrl-autologin --help
```

Enable autologin:

```bash
$ sudo ctrl-autologin --enable username
```

---

### <span style="color: #D62828;">17.5. Screen scaling</span>

A fresh Q4OS installation should detect screen resolution automatically. However, you can force system to use a user defined DPI (dots per inch):

```
Control Panel → System Administration → Screen scaling
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tip:</strong> Increasing the DPI value will make fonts and icons bigger. A correct value for modern displays is ranging from 120 to 200 DPI depending on the screen type.
</blockquote>

---

### <span style="color: #D62828;">17.6. Timezone selection</span>

Run command in terminal to select system timezone:

```bash
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #D62828;">17.7. Root password</span>

Root superuser password is disabled by default in Q4OS. Use "sudo" to issue commands as root.

You can also manually enable and change the root password to be able to use root account directly:

```bash
$ sudo passwd
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Setup and Using</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Trinity desktop user manual, rev. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Official Q4OS Website</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Documentation</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Community Forum</a>
</p>

</div>
