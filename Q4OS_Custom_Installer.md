<div align="center">

# 📦 <span style="color: #2E86AB;">Easy way to create custom application installer</span>

### <span style="color: #6C757D;">Developer Manual</span>
*<span style="color: #A23B72;">Revision 09/2024</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source of document: <a href="https://www.q4os.org/dqa009.html" style="color: #2E86AB;">https://www.q4os.org/dqa009.html</a>
</p>

</div>

---

## 📑 <span style="color: #2E86AB;">Table of Contents</span>

### <span style="color: #F77F00;">1. [Introduction](#1-introduction)</span>
### <span style="color: #06A77D;">2. [Example Applications](#2-example-applications)</span>
- 2a. [Apt installer](#2a-apt-installer)
- 2b. [Flatpak installer](#2b-flatpak-installer)
- 2c. [Deb integration](#2c-deb-integration)
- 2d. [Advanced installers](#2d-advanced-installers)

### <span style="color: #D62828;">3. [Extracting Installers](#3-extracting-installers)</span>

---

## <span style="color: #F77F00;">1. Introduction</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

This document describes how to create Q4OS self-extracting convenient installer for your own applications, files and directory structure.

### 🎯 What You'll Create

This procedure will create both:

1. **`.deb` package** - for installation with `apt` command
2. **`.qsi` installer** - fully automated, convenient installer

The installer will flawlessly install and deliver the application to Q4OS users.

</div>

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
⚙️ <strong>Prerequisites:</strong> Before we can proceed creating an application, you need to install Q4OS Development Pack from repositories:
</blockquote>

```bash
$ sudo apt install q4os-devpack-base
```

---

## <span style="color: #06A77D;">2. Example Applications</span>

### <span style="color: #06A77D;">2a. Apt installer</span>

In this example we create the most simple installer for single application from Apt repositories.

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Step 1:** Get installer configuration from template:

```bash
$ cp -r /opt/program_files/q4os-devpack/examples/00_qinstaller/basic $HOME/example
```

**Step 2:** Build the installer:

```bash
$ cd $HOME/example
$ build-qinstaller qinstaller1
```

**Step 3:** Find the created installer in `$HOME/example1/setup`

</div>

---

### <span style="color: #06A77D;">2b. Flatpak installer</span>

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tip:</strong> Go the same as for example 2a above, only replace "qinstaller1" template with "qinstaller2"
</blockquote>

---

### <span style="color: #06A77D;">2c. Deb integration</span>

We will create installer with a `.deb` file integrated. Get a simple sample application from development pack template - it will represent an application.

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #F77F00;">

**Step 1:** Copy the template

Run commands in terminal (you can use cut and paste):

```bash
$ cp -r /opt/program_files/q4os-devpack/examples/00_qinstaller/sample_app $HOME/my_sample_app
```

The directory structure in `$HOME/my_sample_app/` represents our application.

**Step 2:** Build the installer

```bash
$ cd $HOME/my_sample_app
$ dpkg-buildpackage -b -uc -us -tc
```

Comfortable `.qsi` installer will be generated in your `$HOME` directory along with the regular Debian `.deb` package.

**Step 3:** Test installation

You can now proceed testing installation of your application by double-clicking `setup_sample-app_*.qsi` file.

</div>

<div align="center" style="margin: 20px 0;">

![Comfortable installer will be generated](./Easy%20way%20to%20create%20custom%20application%20installer_files/dqa009_01.png)
![You can now proceed testing installation](./Easy%20way%20to%20create%20custom%20application%20installer_files/dqa009_02.png)

</div>

**Step 4:** Run the application from terminal:

```bash
$ sample-app.sh
```

<div align="center" style="margin: 20px 0;">

![Run the sample application](./Easy%20way%20to%20create%20custom%20application%20installer_files/dqa009_03.png)

</div>

**Step 5:** To remove the installed application:

```bash
$ sudo apt remove sample-app
```

---

### <span style="color: #06A77D;">2d. Advanced installers</span>

<div style="background-color: #F3E5F5; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #7209B7;">

🚀 **For Advanced Users:**

Choose any of our official open source installers from [Q4OS Github account](https://github.com/q4os-installers) as a template.

**Steps:**
1. Clone the installer
2. Customize all the desired options

</div>

---

## <span style="color: #D62828;">3. Extracting Installers</span>

<div style="background-color: #FFEBEE; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

Extracting and looking into a compiled `.qsi` installer is easy.

**Steps:**

1. Copy the installer file into some working directory
2. Run to extract its content in this directory:

```bash
$ xqtrsetup
```

</div>

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Easy way to create custom application installer</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Developer manual, rev. 09/2024</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Official Q4OS Website</a> | 
💻 <a href="https://github.com/q4os-installers" style="color: #FFD700; text-decoration: none;">Q4OS GitHub</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Documentation</a>
</p>

</div>
