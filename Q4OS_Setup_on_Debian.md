<div align="center">

# 🐧 <span style="color: #2E86AB;">Setup Q4OS on top of a Debian based distribution</span>

### <span style="color: #6C757D;">Administrator Manual</span>
*<span style="color: #A23B72;">Revision 12/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source of document: <a href="https://www.q4os.org/dqa017.html" style="color: #2E86AB;">https://www.q4os.org/dqa017.html</a>
</p>

</div>

---

## 📑 <span style="color: #2E86AB;">Table of Contents</span>

### <span style="color: #F77F00;">1. [Introduction](#1-introduction)</span>
### <span style="color: #06A77D;">2. [Q4OS Setup](#2-q4os-setup)</span>
### <span style="color: #D62828;">3. [After Install Steps](#3-after-install-steps)</span>

---

## <span style="color: #F77F00;">1. Introduction</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

The procedure consists of couple different steps:

1. **First**, you need to install one of the Debian-based Linux distributions on your device. This includes:
   - **Debian** itself
   - **Devuan** for x86_64bit
   - **Armbian** or **Raspberry Pi OS** for the Arm64 architecture

2. **Then**, you download and run the Q4OS installation script, which will set up and fully configure fresh Q4OS desktop on your computer.

The script will:
- ✅ Check for compatibility
- ✅ Add Q4OS repositories
- ✅ Modify the underlying system in a Q4OS way
- ✅ Enable Q4OS tools and features on the host operating system

</div>

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 15px; margin: 15px 0; border-radius: 5px;">
💡 <strong>ARM Support:</strong> As Q4OS supports ARM 64bit hardware architecture, this method is also very convenient for setting up Q4OS on ARM devices.
</blockquote>

---

## <span style="color: #06A77D;">2. Q4OS Setup</span>

As introduced in the first chapter, perform a Debian based OS installation first, configure it accordingly.

There is an interactive Q4OS installation script available from Q4OS downloads repository. It supports various Debian based operating systems.

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #F77F00;">

### 📥 Installation Steps

Simply download and run this script in terminal as **root**:

```bash
$ wget q4os.org/downloads/q4os-setup.sh
$ su
# sh q4os-setup.sh
```

The script will add Q4OS repositories and guide you throughout Q4OS setup process. Please follow on-screen instructions.

</div>

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
⏱️ <strong>Note:</strong> The setup process takes a while. Once completed, reboot and login into the fresh and clean Q4OS Desktop.
</blockquote>

---

## <span style="color: #D62828;">3. After Install Steps</span>

<div style="background-color: #F3E5F5; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #7209B7;">

Now, it's the right time to install desired applications!

### 🎯 Recommended Approach

The best and recommended way is to use:

- **Q4OS Desktop Profiler**
- **Software Center**

Please read Q4OS [documentation](https://www.q4os.org/documents.html) for detailed instructions.

</div>

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 15px; margin: 15px 0; border-radius: 5px;">
🎉 <strong>Welcome to Q4OS!</strong> Enjoy your new desktop and don't forget to involve yourself in the Q4OS <a href="https://www.q4os.org/forum/" style="color: #2E86AB;">community</a>.
</blockquote>

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Setup Q4OS on top of a Debian based distribution</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Administrator manual, rev. 12/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Official Q4OS Website</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Documentation</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Community Forum</a>
</p>

</div>
