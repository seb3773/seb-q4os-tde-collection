<div align="center">

# 🛠️ <span style="color: #2E86AB;">Build an application for Trinity desktop</span>

### <span style="color: #6C757D;">General recommendations - Developer Manual</span>
*<span style="color: #A23B72;">Revision 08/2024</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source of document: <a href="https://www.q4os.org/dqa002.html" style="color: #2E86AB;">https://www.q4os.org/dqa002.html</a>
</p>

</div>

---

## 📑 <span style="color: #2E86AB;">Table of Contents</span>

1. [Introduction](#1-introduction)
2. [Basic installation rules in short](#2-basic-installation-rules-in-short)
3. [Installer](#3-installer)
   - 3.1. [Standard setup using Apt](#31-standard-setup-using-apt)
   - 3.2. [Simple setup mode](#32-simple-setup-mode)
   - 3.3. [User setup mode](#33-user-setup-mode)
4. [Directory tree](#4-directory-tree)
5. [Desktop icons](#5-desktop-icons)
6. [Menu entries](#6-menu-entries)
7. [Configuration files](#7-configuration-files)
8. [Registration](#8-registration)
9. [Internet repository](#9-internet-repository)
10. [Update mechanism](#10-update-mechanism)
11. [Porting existing applications](#11-porting-existing-applications)
12. [Windows applications](#12-windows-applications)

---

## <span style="color: #F77F00;">1. Introduction</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

This developer manual generally describes important rules for building a Unix-like application for Q4OS Trinity operating system, alongside clarifies essential build steps and also help you to understand Q4OS basics and design.

### 🎯 About Q4OS

Q4OS is desktop operating system designed to offer:
- 🖥️ Compact and clean user interface
- 🔧 Simple accessories
- 🏗️ Stable foundation for running complex third-party applications

Since Q4OS is a Debian/Linux based OS, it uses **Apt** package management system and related tools to maintain system health and clean.

</div>

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 15px; margin: 15px 0; border-radius: 5px;">
💡 <strong>Recommendation:</strong> We advise you to use QT libraries API to compile your applications. If Application requires some library or other software, which is not part of base Q4OS installation, the easiest way is pick it and install as a system shared from official Q4OS repository.
</blockquote>

---

## <span style="color: #D62828;">2. Basic installation rules in short</span>

<div style="background-color: #FFEBEE; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

### 📋 Essential Rules

- ❌ Any Application file may not affect other system files or directory structure!
- 📦 Install Applications using "Apt" package management system (two exceptions: "simple setup mode" and "user setup mode")
- 📁 All Application files are located in `/program_files/appname` directory
- 🍔 System menu entries in `/usr/share/apps/q4os_system/q4os_menus_applications_merged/`
- 🔗 System menu links in `/usr/share/applications/`
- 🖼️ System desktop icons in `/opt/trinity/share/apps/kdesktop/Desktop/`
- ⚙️ System configuration files in `/program_files/appname/` or `/etc/appname/`
- 📝 Registration via `/usr/share/apps/q4os_system/q4_regs/appname.qrg` file is necessary
- 👤 User menu entries and links in `$HOME/.q4data/applnk/Programs/`
- 🖥️ User desktop icons in `$HOME/Desktop/`
- 🔧 User configuration files in `$HOME/.appname/`
- 📂 Placing some files somewhere in user's `$HOME/` directories structure is possible
- 🗑️ Using `/tmp/` for temporary operations is recommended
- ⚠️ Placing file to other than specified location is allowed only in absolutely necessary cases
- 🔓 Q4OS allows you to install application bypassing "Apt" system using "simple setup mode"
- 👥 It is possible to install user specific application in "user setup mode"

</div>

---

## <span style="color: #06A77D;">3. Installer</span>

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0;">

Install job should be automated by user comfortable installer to let user to:
- ❓ Answer questions
- ✅ Take some more installation steps like environment checks
- 🔄 Pre/post-install actions
- ➕ Another optional steps
- 📥 Finally install the software

Packages can be packed together and joined to installer creating single self-extracting executable.

</div>

---

### <span style="color: #06A77D;">3.1. Standard setup using Apt</span>

The preferred way to distribute your application is to create Apt `*.deb` packages (or single package) installable using `apt` or `dpkg` commands, which are part of basic system installation.

<div style="background-color: #E3F2FD; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Key Features:**

If Application requires some external library, which is included in official Q4OS repository, you can set it as dependency and installer automatically takes care about proper setup.

Installer can install/remove packages from official repositories standard "Apt" way using command-line tools as `dpkg` or `apt`. Any administrative operations need to be executed via `sudo` command.

</div>

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
📚 <strong>Resources:</strong> For detailed resource on "Apt" package management system look at <a href="http://www.debian.org/doc/debian-policy" style="color: #F77F00;">http://www.debian.org/doc/debian-policy</a>
</blockquote>

You can take and modify simple installer skeleton from "Q4OS Development Pack" software now. We plan to release official Q4OS installer in the future.

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #06A77D;">

### ✨ Advantages of using "Apt" package management system:

- ✅ Control over any Application file
- 📦 Take care about installation of dependent software
- 🔗 Close integration to system, keeping it clean
- 🔍 Watch dependencies, avoid package conflicts
- 🗑️ Easy uninstall process
- 🔄 Easy update mechanism
- 🌐 Possibility to create your own Internet repository
- 🏪 Possibility to order your app into Q4OS software centre

</div>

**Notes about installer actions:**

Application installer has to process at minimum the following operations:

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Required Operations:**
- 📁 Create `program_files/appname` directory
- 📋 Copy application files and directory structure into `program_files/appname`
- 🍔 Create menu and desktop entries
- 📝 Register application to the system

**Optional Operations:**
- ⚙️ Create configuration files
- 👥 Adding some system users and groups
- ➕ Other operations

</div>

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 15px; margin: 15px 0; border-radius: 5px;">
⚠️ <strong>Important restrictions!</strong><br>
• Application may not affect any Q4OS system files and structure<br>
• All files should be installed into permitted folders only
</blockquote>

---

### <span style="color: #06A77D;">3.2. Simple setup mode</span>

Q4OS allows installer to only copy application files into `/program_files/appname` tree without packaging and installing with "Apt", but you loose some noted advantages in this case.

<div style="background-color: #FFF3E0; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #F77F00;">

**Basic rules must be kept:**

- 📁 All files belonging to application must be located in `program_files/appname` and/or user's `$HOME/.program_files/appname` directory
- 📝 Register application into the system using `/usr/share/apps/q4os_system/q4_regs/appname.qrg` file
- 🍔 Menu entries located in `$HOME/.q4data/applnk/Programs` directory
- 🖼️ Desktop icons located in `$HOME/Desktop`
- 📂 Other application files can be stored somewhere in user's `$HOME/` directory structure
- ❌ Any other file locations and other exceptions are strictly forbidden in "simple setup mode"

</div>

---

### <span style="color: #06A77D;">3.3. User setup mode</span>

<div style="background-color: #F3E5F5; padding: 20px; border-radius: 8px; margin: 15px 0;">

Non-privileged users will use this mode for installations. All Application files are located strictly in user's `$HOME/` directory structure.

**Recommendation:** It is recommended to use `$HOME/.program_files/appname` folder as much as possible.

</div>

---

## <span style="color: #7209B7;">4. Directory tree</span>

<div style="background-color: #F3E5F5; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #7209B7;">

According to basic Q4OS rules, any file (executables, libraries, data, ...) belonging to an application has to be located in application specific folder `/program_files/appname` with rare exceptions (menu and desktop entries, configuration) all described in this document.

**Purpose:** `/program_files` folder is intended to be independent on operating system files and structure.

### 📂 Installation Steps

One necessary step for installer is to:
1. Create folder `/program_files/appname`
2. Copy all application data into it

Subtree structure is optional. For example, properly ported Unix applications will contain standard subdirectories like `bin, share, var, etc, ...`

</div>

---

## <span style="color: #F77F00;">5. Desktop icons</span>

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0;">

### 🌐 Desktop icons folder - global:

```
/opt/trinity/share/apps/kdesktop/Desktop/
```

Directory contains `*.desktop` files - links to desktop icons.

📚 For more info see: [Desktop Entry Specification](http://standards.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html)

### 👤 Desktop icons folder - user:

```
$HOME/Desktop/
```

Directory contains `*.desktop` files - links to desktop icons.

</div>

---

## <span style="color: #06A77D;">6. Menu entries</span>

Installer should create some "Start menu" shortcuts. Any entry can be global (for all users) or user specific.

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #06A77D;">

### 🌐 Menu entries - global:

```
/usr/share/apps/q4os_system/q4os_menus_applications_merged/
```

Directory contains xml file `appname.menu`.

📚 For more info see: [Menu Specification](http://standards.freedesktop.org/menu-spec/menu-spec-latest.html)

### 🔗 Menu links - global:

```
/usr/share/applications/
```

Directory contains `*.desktop` files - links to menu items.

📚 For more info see: [Desktop Entry Specification](http://standards.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html)

### 👤 Menu entries - user:

```
$HOME/.q4data/applnk/Programs
```

Directory contains user menu items, organized into real subdirectory structure. Any directory can contain:
- 📁 Subdirectory (submenu)
- 📄 `*.desktop` file (menu item)

Users are allowed to add, remove or change menu items modifying this directory structure and files contained.

</div>

---

## <span style="color: #D62828;">7. Configuration files</span>

<div style="background-color: #FFEBEE; padding: 20px; border-radius: 8px; margin: 15px 0;">

### ⚙️ Configuration Storage

**System configuration:**
- `/program_files/appname/`
- or `/etc/appname/` directory structure

**User specific configuration:**
- `$HOME/.appname/`

</div>

---

## <span style="color: #7209B7;">8. Registration</span>

<div style="background-color: #F3E5F5; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #7209B7;">

Applications have to be registered by describing `appname.qrg` file in `/usr/share/apps/q4os_system/q4_regs/q4apps` directory.

### 📝 Registration Process

Installer creates new file `/usr/share/apps/q4os_system/q4_regs/appname.qrg` by:
1. Copying skeleton file `app.qrg.template`
2. Substitute all fields properly

**Importance:** This step is important to maintain proper information about your application. `*.qrg` file is a simple, but important interface between your application and Q4OS.

</div>

---

## <span style="color: #F77F00;">9. Internet repository</span>

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0;">

You can have your own Internet repository for:
- 🔄 Easy application updates
- 🏪 Order your app in the Q4OS software centre

📚 To learn how create your own GPG signed Internet software repository start here: [How To Setup A Debian Repository](http://wiki.debian.org/HowToSetupADebianRepository)

</div>

---

## <span style="color: #06A77D;">10. Update mechanism</span>

<div style="background-color: #E3F2FD; padding: 20px; border-radius: 8px; margin: 15px 0;">

There is no recommended way how to solve this quite complicated task.

**Options:**
- 📦 Use custom software repository and package management system to simplify developer's life
- 🔧 If you need some specific functions, you have to code custom updater

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Important:</strong> Doing any update action, it is important to ensure keeping Apt package system in clean consistent state.
</blockquote>

</div>

---

## <span style="color: #D62828;">11. Porting existing applications</span>

<div style="background-color: #FFEBEE; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

Q4OS handles typical Unix filesystem structure. Any native Linux executable can be run without modification, so porting Unix applications is fairly easy.

### 🔄 Porting Process

**Quick (but not clean) way:**
- Simply run `make install`
- However, you have to take care about Q4OS installation rules above

**Recommended approach:**

At minimal, you should:
1. ✏️ Modify Makefile to add menu and desktop entries for Q4OS
2. 📝 Take care of registration to the system
3. 📁 Locating installed files in `program_files/appname` folder is strongly recommended (although not necessary)
4. 📦 Installing with user comfortable [installer](#3-installer) improve user's comfort and make distribution easier

</div>

---

## <span style="color: #7209B7;">12. Windows applications</span>

<div style="background-color: #F3E5F5; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #7209B7;">

It is possible to run Windows applications within Q4OS using [Wine](http://www.winehq.org/) compatibility layer.

### 🍷 Wine Integration

**Available Resources:**
- Wine installer available at Q4OS website
- Development utilities installable from basic Q4OS repositories

**Development Tools:**
- 🔧 Great Wine debug tools
- 📚 [WineLib](http://wiki.winehq.org/Winelib) to adapt and compile Windows applications for Q4OS
- 📖 See [Wine Developer's Guide](http://www.winehq.org/docs/winedev-guide/index) - detailed resource for development with Wine

**Current Status:**
At the moment we are working at Wine optimization and close integration into the Q4OS system.

</div>

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Build an application for Trinity desktop</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>General recommendations, developer manual, rev. 08/2024</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Official Q4OS Website</a> | 
💻 <a href="http://www.trinitydesktop.org/" style="color: #FFD700; text-decoration: none;">Trinity Desktop</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Documentation</a>
</p>

</div>
