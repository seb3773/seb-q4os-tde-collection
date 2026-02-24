<div align="center">

# 🖥️ <span style="color: #2E86AB;">Q4OS Frequently Asked Questions</span>

### <span style="color: #6C757D;">Trinity Desktop User Manual</span>
*<span style="color: #A23B72;">Revision 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source of document: <a href="https://www.q4os.org/dqa011.html" style="color: #2E86AB;">https://www.q4os.org/dqa011.html</a>
</p>

</div>

---

## 📑 <span style="color: #2E86AB;">Table of Contents</span>

### <span style="color: #F77F00;">1. [Introduction](#1-introduction)</span>

### <span style="color: #06A77D;">2. [Installation](#2-installation)</span>
- 2.1. [How can I create bootable Q4OS installation USB disk?](#21-how-can-i-create-bootable-q4os-installation-usb-disk)
- 2.2. [Is there a way to dual boot Q4OS alongside Windows?](#22-is-there-a-way-to-dual-boot-q4os-alongside-windows)
- 2.3. [I have no sound after installation, what should I do?](#23-i-have-no-sound-after-installation-what-should-i-do)
- 2.4. [Unable to connect to wireless network, what to do?](#24-unable-to-connect-to-wireless-network-what-to-do)

### <span style="color: #D62828;">3. [System](#3-system)</span>
- 3.1. [There are broken packages dependencies in my system. How can I fix it?](#31-there-are-broken-packages-dependencies-in-my-system-how-can-i-fix-it)
- 3.2. [Some letters being mis-typed ('L' shows up as '3', 'J' as '1')](#32-some-letters-being-mis-typed-l-shows-up-as-3-j-as-1)
- 3.3. [Fonts and icons are too small on my hiDPI screen, can I make them larger?](#33-fonts-and-icons-are-too-small-on-my-hidpi-screen-can-i-make-them-larger)
- 3.4. [How can I display current CPU temperature in the system panel?](#34-how-can-i-display-current-cpu-temperature-in-the-system-panel)
- 3.5. [I am behind a proxy, package manager based applications don't work](#35-i-am-behind-a-proxy-package-manager-based-applications-dont-work)
- 3.6. [I want to use recent Linux kernel, is it possible?](#36-i-want-to-use-recent-linux-kernel-is-it-possible)

### <span style="color: #7209B7;">4. [Desktop](#4-desktop)</span>
- 4.1. [How to set up multiple virtual desktops in Q4OS?](#41-how-to-set-up-multiple-virtual-desktops-in-q4os)
- 4.2. [I am not able to rename or edit some icons on my Desktop](#42-i-am-not-able-to-rename-or-edit-some-icons-on-my-desktop)
- 4.3. [How can I edit Start menu?](#43-how-can-i-edit-start-menu)
- 4.4. [Can I customize view and shortcuts on the right panel of the default Q4OS 'Bourbon' Start menu?](#44-can-i-customize-view-and-shortcuts-on-the-right-panel-of-the-default-q4os-bourbon-start-menu)
- 4.5. [I want Welcome screen entry to be shown in the Start menu](#45-i-want-welcome-screen-entry-to-be-shown-in-the-start-menu)
- 4.6. [How can I autostart an application?](#46-how-can-i-autostart-an-application)
- 4.7. [I have messed my desktop, how can I revert default colors, fonts, theme and other desktop settings?](#47-i-have-messed-my-desktop-how-can-i-revert-default-colors-fonts-theme-and-other-desktop-settings)
- 4.8. [How can I set single-click icons instead of double-click?](#48-how-can-i-set-single-click-icons-instead-of-double-click)
- 4.9. [Tell me the most easy way to get a screenshot](#49-tell-me-the-most-easy-way-to-get-a-screenshot)
- 4.10. [Is it possible to change icon theme?](#410-is-it-possible-to-change-icon-theme)
- 4.11. [I have defined keyboard shortcuts in the Control Panel, but they don't work](#411-i-have-defined-keyboard-shortcuts-in-the-control-panel-but-they-dont-work)
- 4.12. [I have noticed the 'Programs' entry have vanished from the Start menu](#412-i-have-noticed-the-programs-entry-have-vanished-from-the-start-menu)
- 4.13. [Keyboard shortcut doesn't work to switch between non-latin keyboard layouts](#413-keyboard-shortcut-doesnt-work-to-switch-between-non-latin-keyboard-layouts)
- 4.14. [I need to adjust display brightness](#414-i-need-to-adjust-display-brightness)

### <span style="color: #F77F00;">5. [Applications](#5-applications)</span>
- 5.1. [How can I setup 'Conky' transparency?](#51-how-can-i-setup-conky-transparency)

---

## <span style="color: #F77F00;">1. Introduction</span>

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
📢 Notify us about any errors you find, suggestions are appreciated. When possible send us what you think would be a clearer solution. You can safely stick to <a href="http://www.trinitydesktop.org/faq/index.php" style="color: #2E86AB;">Trinity desktop environment FAQ</a>.
</blockquote>

---

## <span style="color: #06A77D;">2. Installation</span>

### <span style="color: #06A77D;">2.1. How can I create bootable Q4OS installation USB disk?</span>

The easiest way in Linux is to plug your usb in, do not mount it, and run in terminal:

```bash
$ sudo cp bootable.iso /dev/sdx
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Note:</strong><br>
• <code>sdx</code> is the target usb drive, for example <code>sdb</code><br>
• <code>bootable.iso</code> is bootable Q4OS installation CD image, you can download it from Q4OS website
</blockquote>

Alternatively, you can use multiplatform **UNetbootin** or **Rufus** software to create bootable USB disks. See [how to create a live media](https://www.q4os.org/dqa018.html#creat).

---

### <span style="color: #06A77D;">2.2. Is there a way to dual boot Q4OS alongside Windows?</span>

Sure! The preferred way is to proceed installation from 'Live' CD, as it gives you bootloader install option. If you let installer to install Grub bootloader, it will autodetect available operating systems including Windows and offer them all on every boot.

If you want to keep Windows bootloader, don't forget to uncheck the related checkbox during installation.

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Important:</strong> We strongly recommend to backup all your data before. Please read <a href="https://www.q4os.org/dqa018.html" style="color: #D62828;">installation instructions</a>.
</blockquote>

---

### <span style="color: #06A77D;">2.3. I have no sound after installation, what should I do?</span>

We recommend you to install the Pipewire sound server first:

```bash
$ sudo apt install pipewire pavucontrol-qt
```

Reboot your computer. Then follow these steps:

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Configuration Steps:**

1. Right-click to 'mixer' icon in system tray → 'Select Master Channel...'
2. Set 'Current Mixer' to 'PipeWire' in the top right listbox
3. Click 'Ok' to close the dialog
4. Run 'Volume Control' application from the Start menu
5. Configure output mixer settings on the 'Output Devices' tab
6. Check if output channels are not muted

</div>

The audio system should work now. If not, continue following the steps below.

**Additional Diagnostics:**

Left-click to 'mixer' icon in the system tray, and click to 'Mixer' button to check and update audio mixer levels. Make sure there is the 'PipeWire' sound card selected in the top right corner of the 'kmix' mixer window.

Then run command in terminal and check debug output:

```bash
$ artsplay /opt/trinity/share/sounds/KDE_Startup.wav
```

If there is still no sound, terminate temporarily Trinity sound server and try to play audio with independent alsa player:

```bash
$ artsshell terminate
$ aplay /opt/trinity/share/sounds/KDE_Startup.wav
```

Again, check debug output. If your audio system still doesn't work, continue [Troubleshooting sound problems](http://www.trinitydesktop.org/faq/sound.php) at Trinity FAQ.

---

### <span style="color: #06A77D;">2.4. Unable to connect to wireless network, what to do?</span>

Q4OS fully supports wireless networks and includes a tool called **tdenetworkmanager** to manage wireless connections. You can find it in the system tray.

If you have issues connecting to a wireless network, please read [wifi connection troubleshooting post](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #D62828;">3. System</span>

### <span style="color: #D62828;">3.1. There are broken packages dependencies in my system. How can I fix it?</span>

We have a handy tool to autofix broken dependencies in Q4OS, just run in terminal:

```bash
$ sudo sh /usr/share/apps/q4os_system/bin/qapt_fix.sh
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Reminder:</strong> We strongly recommend to install software from reliable and Debian compatible sources only to prevent package system from being corrupted.
</blockquote>

---

### <span style="color: #D62828;">3.2. Some letters being mis-typed ('L' shows up as '3', 'J' as '1')</span>

A common glitch that occurs on Netbooks with a small keyboard. Keyboard is blocked by NumLock, you could try to switch NumLock off.

Launch Control Panel:

```
Control Panel → Peripherals → Keyboard → NumLock on KDE startup → set Off
```

Login again and try the keyboard.

---

### <span style="color: #D62828;">3.3. Fonts and icons are too small on my hiDPI screen, can I make them larger?</span>

Yes, Q4OS can scale the screen resolution. Please read [screen resolution](https://www.q4os.org/dqa007.html#tips.6) chapter.

---

### <span style="color: #D62828;">3.4. How can I display current CPU temperature in the system panel?</span>

Run **ksensors** application from:

```
Start menu → Programs → Accessories → System → KSensors
```

If **ksensors** is not installed yet, follow the [hardware sensors](https://www.q4os.org/dqa007.html#hwsens) chapter to install it.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0; border-left: 5px solid #7209B7;">

**Configuration:**

1. Right-click to 'ksensors' icon in system tray → Configure
2. Select related HW sensors group
3. Select desired sensor from the list
4. Dock tab → check 'Visible' checkbox

You can optionally set colors, alarms, thresholds, actions on limits exceeding and other options. Click 'Apply' button and close the dialog.

</div>

---

### <span style="color: #D62828;">3.5. I am behind a proxy, package manager based applications don't work</span>

You need to set system wide environment variables. Open the `/etc/environment` file with your favorite editor and add the following lines (modifying appropriately):

```bash
http_proxy="http://myproxy.server.com:8080/"
https_proxy="http://myproxy.server.com:8080/"
ftp_proxy="http://myproxy.server.com:8080/"
no_proxy="localhost,127.0.0.1,localaddress,.localdomain.com"
HTTP_PROXY="http://myproxy.server.com:8080/"
HTTPS_PROXY="http://myproxy.server.com:8080/"
FTP_PROXY="http://myproxy.server.com:8080/"
NO_PROXY="localhost,127.0.0.1,localaddress,.localdomain.com"
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Note:</strong> You must duplicate in both upper-case and lower-case because some programs only look for one or the other.
</blockquote>

APT package management system will not obey the environment variables when used normally with sudo. So separately configure them; create a file called `95proxies` in `/etc/apt/apt.conf.d/`, and include the following:

```bash
Acquire::http::proxy "http://myproxy.server.com:8080/";
Acquire::ftp::proxy "ftp://myproxy.server.com:8080/";
Acquire::https::proxy "https://myproxy.server.com:8080/";
```

Finally, reboot to make sure the changes take effect.

---

### <span style="color: #D62828;">3.6. I want to use recent Linux kernel, is it possible?</span>

We recommend to use reliable and deeply proven default Q4OS/Debian kernel. There isn't too much reasons for ordinary users to use newer kernel.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Warning:</strong> The latest kernels are not so secure as the rock stable and exhaustively tested default Debian kernel, however it could bring improvements and newer device drivers and support.
</blockquote>

If you prefer for some reasons the latest linux kernel, run the auto-installation script in terminal to easily install it from backports repository:

```bash
$ qinst-kernel-bpo
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Good to know:</strong> The old good default kernel will not be uninstalled, so you can anytime choose and boot it from the grub boot menu, if you will fall into any issues.
</blockquote>

---

## <span style="color: #7209B7;">4. Desktop</span>

### <span style="color: #7209B7;">4.1. How to set up multiple virtual desktops in Q4OS?</span>

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Step 1:** Launch the Control Panel and go to:

```
Desktop → Multiple Desktops
```

Select how many virtual desktops you wish to have.

**Step 2a:** Add a desktop switch applet to your taskbar:

1. Right-mouse clicking on the taskbar
2. Select 'Add Applet to Panel' (if the taskbar is locked, un-lock it first)
3. In the pop-up window, select 'Desktop Pager / Switcher'
4. Click 'Add To Panel'

**Step 3a:** Configure a keyboard shortcut:

1. Launch the Control Panel
2. Go to: `Regional & Accessibility → Keyboard Shortcuts`
3. Under 'Global Shortcuts' tab, scroll down and find 'Switch To Next Desktop' under 'Desktop Switching'
4. Click the button next to 'Custom' option
5. Assign the keyboard combination you wish to use
6. Click 'OK' to save

</div>

---

### <span style="color: #7209B7;">4.2. I am not able to rename or edit some icons on my Desktop</span>

There could be three logical types of icons present on your desktop:

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 10px 0;">

**1. System Icons** 🔒
- 'My Computer', 'My Documents', 'My Network Places', 'Trash', 'Web Browser', 'Printers'
- Owned by root
- Not directly editable by a user
- Can be removed from desktop

**2. Global Icons** 🌐
- Usually created by application installers
- Owned by root and shared by all users
- Users can hide them but not edit or rename

**3. User Icons** 👤
- Created by a single user
- Full control: delete, rename, edit properties (right-click → Properties)

</div>

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tip:</strong> If you want to edit global or system icon, we recommend to remove it from the desktop and create matching user's icon using Drag&drop → Copy from the Start menu. It will be owned by user and fully editable.
</blockquote>

---

### <span style="color: #7209B7;">4.3. How can I edit Start menu?</span>

1. Open the Start menu
2. Right-click on any item under the 'Programs' entry
3. Select 'Edit menu'
4. The menueditor window appears

You will be able to create new custom submenus/folders structure and fill it with desired menu items. You can create new shortcuts using right mouse click, or drag&drop icons from the Start menu or Desktop into the menueditor window.

Newly created items will appear in the Start menu after closing the menueditor window.

**Bonus:** You can also switch Start menu items to be organized by Categories or by Applications:

```bash
$ sh /usr/share/apps/q4os_system/bin/kmenu_struct.sh --help
```

---

### <span style="color: #7209B7;">4.4. Can I customize view and shortcuts on the right panel of the default Q4OS 'Bourbon' Start menu?</span>

Yes! Edit file `$HOME/.trinity/share/config/kickerrc` in your home directory.

There are several configuration options beginning 'Bourbon' commented out by default. You need to:

1. Uncomment `BourbonSysViewCustomItems` line
2. Specify `.desktop` links you wish to be displayed on the right menu panel
3. Use comma `,` as a delimiter

**Additional options:**

- Hide default shortcuts:
  - `BourbonShowSysViewFolders=false`
  - `BourbonShowSysViewApps=false`

---

### <span style="color: #7209B7;">4.5. I want Welcome screen entry to be shown in the Start menu</span>

Run command to update Welcome screen shortcut in terminal:

```bash
$ sudo kwriteconfig --file '/usr/share/applications/q4os-welcome-screen.desktop' --group 'Desktop Entry' --key 'NoDisplay' 'false'
```

Alternatively, you can edit `/usr/share/applications/q4os-welcome-screen.desktop` file manually.

Welcome screen icon will appear under:

```
Start menu → Programs → Accessories → System
```

---

### <span style="color: #7209B7;">4.6. How can I autostart an application?</span>

You need to add an application shortcut (`.desktop` file) into the autostart folder:

- `$HOME/.trinity/Autostart`
- or `$HOME/.q4data/Programs/Startup`

The application will be launched immediately after the user login.

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Methods:**

1. Drag any application shortcut from the Start menu or Desktop and drop it into the autostart folder
2. It's also possible to place a shell script or executable into the autostart folder

</div>

---

### <span style="color: #7209B7;">4.7. I have messed my desktop, how can I revert default colors, fonts, theme and other desktop settings?</span>

Simply run in terminal:

```bash
$ sh /usr/share/apps/q4os_system/bin/default_desktop_settings.sh
```

---

### <span style="color: #7209B7;">4.8. How can I set single-click icons instead of double-click?</span>

Icon activation by mouse doubleclicking is default in Q4OS. It's easy to set single click activation, hover effect and more in Control Panel:

```
Control Panel → Peripherals → Mouse → General tab → Single click to open files and folders
```

---

### <span style="color: #7209B7;">4.9. Tell me the most easy way to get a screenshot</span>

You can do this without any other packages:

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Quick Method:**

1. Press `PrtScr` key
2. Right-click on the desktop
3. Select 'Paste clipboard contents'
4. A dialog appears where you can enter the filename and image type
5. The file will be saved to the desktop

You can also open Konqueror to browse to preferred folder, right-click and select 'Paste clipboard contents' to save file to preferred location.

</div>

**Dedicated Application:**

There is a lightweight and powerful application **ksnapshot-trinity**, capable to grab full screen, region, a window or window part only.

Installation:

```bash
$ sudo apt install ksnapshot-trinity
```

---

### <span style="color: #7209B7;">4.10. Is it possible to change icon theme?</span>

Yes! You have to unlock advanced Control Panel options in terminal:

```bash
$ sudo kcmodules --unlock
```

Then go to:

```
Control Panel → Appearance & Themes → Icons
```

Setup theme you prefer.

---

### <span style="color: #7209B7;">4.11. I have defined keyboard shortcuts in the Control Panel, but they don't work</span>

You only need to enable khotkeys service to be ran on session login.

Go to Control Panel:

```
Control Panel → Regional & Accessibility → Input Actions → General Settings tab → uncheck Disable KHotKeys checkbox
```

---

### <span style="color: #7209B7;">4.12. I have noticed the 'Programs' entry have vanished from the Start menu</span>

It happens rarely on some specifically configured systems. The workaround that should fix it is to re-switch from classic - kicker - classic menu.

You could report it as a new bug in our [Bug tracker](https://sourceforge.net/p/q4os/tickets), and add some description if you will find any connections.

---

### <span style="color: #7209B7;">4.13. Keyboard shortcut doesn't work to switch between non-latin keyboard layouts</span>

Keyboard switching shortcut defaults to `Alt+Space` or `Ctrl+Alt+K`. It works flawlessly if you have installed latin keyboard layouts only.

To be able to switch non-latin keyboard freely, you need to add 'latin layout' to each keyboard layout you use.

Run Control Panel:

```
Control Panel → Regional & Accessibility → Keyboard layout → select a non-latin keyboard layout → check 'Include latin layout' checkbox
```

---

### <span style="color: #7209B7;">4.14. I need to adjust display brightness</span>

Simply hover your mouse over the **tdepowersave** icon in the system tray, and use mouse scroll wheel to adjust brightness up or down.

If the icon is not available in the system tray, you need to install `tdepowersave-trinity` package and login to the Trinity desktop session again.

**Alternative:**

You can install `klcddimmer-trinity` package and add applet in the system panel. However, you will need to configure it to use a brightness control backend, for example `xbacklight`.

---

## <span style="color: #F77F00;">5. Applications</span>

### <span style="color: #F77F00;">5.1. How can I setup 'Conky' transparency?</span>

You have to have Q4OS/Trinity desktop effects enabled. It can be setup via Welcome screen or Control Panel.

Edit the `/etc/conky/conky.conf` file and add lines:

```bash
own_window yes
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
own_window_argb_visual
own_window_argb_value 0
```

Comment out line:

```bash
#own_window_type desktop
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Frequently Asked Questions</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Trinity desktop user manual, rev. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Official Q4OS Website</a> | 
🐛 <a href="https://sourceforge.net/p/q4os/tickets" style="color: #FFD700; text-decoration: none;">Bug Tracker</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Forum</a>
</p>

</div>
