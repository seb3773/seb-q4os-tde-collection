<div align="center">

# ⚙️ <span style="color: #2E86AB;">Q4OS Einrichtung und Verwendung</span>

### <span style="color: #6C757D;">Trinity Desktop Benutzerhandbuch</span>
*<span style="color: #A23B72;">Revision 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Quelle des Dokuments: <a href="https://www.q4os.org/dqa007.html" style="color: #2E86AB;">https://www.q4os.org/dqa007.html</a>
</p>

### 🌐 In Ihrer Sprache lesen:
[🇬🇧 English](Q4OS_Setup_and_Using.md) | [🇫🇷 Français](Q4OS_Setup_and_Using.fr.md) | [🇩🇪 Deutsch](Q4OS_Setup_and_Using.de.md) | [🇪🇸 Español](Q4OS_Setup_and_Using.es.md)

</div>

---

## 📑 <span style="color: #2E86AB;">Inhaltsverzeichnis</span>

1. [Einleitung](#1-einleitung)
2. [Testen](#2-testen)
   - 2.1. [Live CD](#21-live-cd)
   - 2.2. [In Virtualbox](#22-in-virtualbox)
3. [Installation](#3-installation)
4. [WLAN-Netzwerk einrichten](#4-wlan-netzwerk-einrichten)
5. [Drucken und Scannen](#5-drucken-und-scannen)
   - 5.1. [Hewlett-Packard Drucker und Scanner](#51-hewlett-packard-drucker-und-scanner)
   - 5.2. [Andere Drucker](#52-andere-drucker)
   - 5.3. [Scanner](#53-scanner)
6. [Energieverwaltung](#6-energieverwaltung)
7. [Hardwaresensoren](#7-hardwaresensoren)
8. [Touchpad-Gerät](#8-touchpad-gerät)
9. [Proprietäre Multimedia-Codecs](#9-proprietary-multimedia-codecs)
10. [Proprietäre Videotreiber](#10-proprietary-video-drivers)
11. [Benutzer und Gruppen](#11-users-and-groups)
    - 11.1. [Einen regulären Benutzer hinzufügen](#111-adding-a-regular-user)
12. [Android-Verbindung](#12-android-interconnection)
13. [Sicherheitsupdates, Softwareverwaltung](#13-security-updates-software-management)
    - 13.1. [Update-Manager](#131-update-manager)
14. [Externe Software-Repositories](#14-external-software-repositories)
15. [Alternative Desktop-Umgebungen](#15-alternative-desktop-environments)
16. [Weitere Sprachen hinzufügen](#16-adding-more-languages)
    - 16.1. [Sprachen hinzufügen](#161-add-languages)
    - 16.2. [Benutzereinrichtung](#162-user-setup)
    - 16.3. [Beispiel](#163-example)
17. [Verschiedene Tipps](#17-miscellaneous-tips)
    - 17.1. [Kickoff Startmenü](#171-kickoff-start-menu)
    - 17.2. [Ein-Klick-Symbole](#172-single-click-icons)
    - 17.3. [Desktop-Effekte](#173-desktop-effects)
    - 17.4. [Automatische Anmeldung](#174-autologin)
    - 17.5. [Bildschirmskalierung](#175-screen-scaling)
    - 17.6. [Zeitzonenauswahl](#176-timezone-selection)
    - 17.7. [Root-Passwort](#177-root-password)

---

## <span style="color: #F77F00;">1. Einleitung</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

Dieses Dokument behandelt die Einrichtung, Konfiguration und Verwendung des Q4OS-Betriebssystems.

Q4OS wird für den Einsatz auf Produktionsmaschinen empfohlen, da es auf dem äußerst stabilen, sicheren und zuverlässigen Debian-System aufgebaut ist, das von vielen Menschen weltweit getestet wurde.

Es gibt eine riesige stabile Softwarebasis in den Standard-Repositories - Sie können sie frei nutzen und das System an Ihre Bedürfnisse anpassen.

</div>

---

## <span style="color: #06A77D;">2. Testen</span>

### <span style="color: #06A77D;">2.1. Live CD</span>

Wenn Sie eine schnelle Q4OS-Erfahrung erhalten oder es auf echter Hardware testen möchten, können Sie sicher eine Q4OS Live-CD oder USB starten.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Sicheres Testen:</strong> Es wird nichts auf Ihre Festplatte geschrieben und Ihre bestehende Installation nicht beeinträchtigt. Es ist möglich, das Q4OS-System direkt vom Live-Medium mit dem Live-Installer zu installieren.
</blockquote>

---

### <span style="color: #06A77D;">2.2. In Virtualbox</span>

Wir empfehlen, Q4OS zu Testzwecken in [Virtualbox](http://www.virtualbox.org/) zu installieren.

**Konfiguration:**
- Betriebssystem: **Linux**
- Version: **Debian (32/64-bit)**

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tipp:</strong> Es ist angebracht, "Virtualbox Guest Additions" im Gastsystem zu installieren, um die beste Leistung zu erzielen. Im Q4OS 'Software Center' ist ein praktischer Auto-Installer verfügbar. Der Installer enthält optimierte Treiber und sollte gegenüber Originalen von Oracle oder anderen Quellen bevorzugt werden.
</blockquote>

---

## <span style="color: #D62828;">3. Installation</span>

Bitte lesen Sie den [Einrichtungsleitfaden](https://www.q4os.org/dqa018.html) für eine frische Q4OS-Installation.

---

## <span style="color: #7209B7;">4. WLAN-Netzwerk einrichten</span>

Q4OS unterstützt drahtlose Netzwerke vollständig und enthält ein Tool namens **tdenetworkmanager** zur Verwaltung drahtloser Verbindungen. Sie finden es in der Systemleiste.

Wenn Sie Probleme beim Verbinden mit einem drahtlosen Netzwerk haben, lesen Sie bitte den [Beitrag zur WLAN-Fehlerbehebung](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #F77F00;">5. Drucken und Scannen</span>

### <span style="color: #F77F00;">5.1. Hewlett-Packard Drucker und Scanner</span>

Installieren Sie das HP Linux Printing and Imaging System, erfüllen Sie Abhängigkeiten und richten Sie einen Drucker im Terminal ein:

```bash
$ sudo apt install hplip hplip-gui avahi-utils cups
$ sudo apt install libcupsimage2-dev libdbus-1-dev libssl-dev libusb-1.0.0-dev python-dev
$ sudo hp-setup
```

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Hinweis:</strong> Einige HP-Drucker erfordern einen herunterladbaren Treiber-Plugin. Der Befehl 'hp-setup' lädt und installiert das Plugin automatisch.
</blockquote>

---

### <span style="color: #F77F00;">5.2. Andere Drucker</span>

Listen Sie zuerst Treiber auf und wählen Sie den passenden für Ihr Modell:

```bash
$ apt-cache search printer-driver
```

Installieren Sie ein bestimmtes Treiberpaket, zum Beispiel für Samsung Laserdrucker:

```bash
$ sudo apt install printer-driver-splix cups
```

Oder Sie können alle verfügbaren Druckertreiber installieren:

```bash
$ sudo apt install foomatic-db printer-driver-all cups
```

Fügen Sie als Nächstes Drucker hinzu und konfigurieren Sie diese:

```
Startmenü → Anwendungen → Einstellungen → Drucksystem
```

Sie finden wertvolle zusätzliche Informationen im [Debian Wiki](https://wiki.debian.org/SystemPrinting).

---

### <span style="color: #F77F00;">5.3. Scanner</span>

Wir empfehlen die Verwendung der Anwendung **Kooka** zum Scannen. Installieren Sie die erforderliche Software und fügen Sie alle Benutzer hinzu, die Zugriff auf die Gruppe 'scanner' benötigen:

```bash
$ sudo apt install libsane sane sane-utils xsane kooka-trinity
$ sudo adduser ihr_benutzername scanner
```

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Wichtig:</strong> Ein Benutzer muss sich ab- und wieder anmelden, damit die neue Gruppe wirksam wird.
</blockquote>

Überprüfen Sie, ob der Scanner jetzt erkannt wird:

```bash
$ scanimage -L
$ sane-find-scanner
```

Wenn Sie ein Netzwerk-Scanning konfigurieren möchten, lesen Sie [Sane über Netzwerk](https://wiki.debian.org/SaneOverNetwork).

---

## <span style="color: #06A77D;">6. Energieverwaltung</span>

Es ist wünschenswert, eine Energieverwaltungsanwendung für Laptops und mobile Geräte zu installieren:

```bash
$ sudo apt update
$ sudo apt install rfkill tdepowersave-trinity
```

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 15px 0;">

Melden Sie sich erneut an, eine schöne Energieverwaltungsanwendung wird in der Systemleiste vorhanden sein.

**Funktionen:**
- 🔋 CPU-Frequenz steuern
- 📊 Batteriestatus anzeigen
- 💤 Ruhezustands- und Hibernate-Aktionen konfigurieren
- 🔘 Deckel-Schließereignisse verwalten
- ⚡ Netzschalter-Konfiguration

</div>

---

## <span style="color: #D62828;">7. Hardwaresensoren</span>

Die meisten Computer verfügen über verschiedene Sensoren, die zur Überwachung Ihrer Hardware verwendet werden können, um unerwartete Ausfälle zu vermeiden. Hier kommt die Anwendung **ksensors** ins Spiel.

```bash
$ sudo apt install ksensors-trinity
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

Sie finden die Überwachungsanwendung 'ksensors' im Startmenü oder in der Systemleiste.

**Funktionen:**
- 🌡️ Temperaturüberwachung
- ⚡ Spannungssensoren
- 🌀 Lüftergeschwindigkeitsüberwachung
- 🔔 Alarme und Schwellenwerte
- ⚙️ Aktionen bei Grenzwertüberschreitungen

</div>

Q4OS sollte verfügbare Sensoren automatisch out-of-the-box erkennen. Wenn nicht, müssen Sie benötigte Kernel-Module erkennen:

```bash
$ sudo sensors-detect
```

Am Ende des Scan-Prozesses werden Sie gefragt, ob Sie hinzufügen möchten, was gefunden wurde, zur Datei '/etc/modules'. Antworten Sie 'ja' und starten Sie neu.

---

## <span style="color: #7209B7;">8. Touchpad-Gerät</span>

Q4OS verwendet standardmäßig den **libinput**-Treiber zur Steuerung des Touchpads und verwandter Zeigegeräte.

Überprüfen Sie die vollständige Liste der 'libinput'-Konfigurationsoptionen:

```bash
$ man libinput
```

Alle Optionen können in der Datei `/etc/X11/xorg.conf.d/60-libinput.conf` angewendet werden.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Alternative: Synaptics-Treiber**

Sie können einen älteren 'synaptics'-Treiber Vorrang vor 'libinput' geben lassen:

```bash
$ sudo apt install xserver-xorg-input-synaptics
```

Verwenden Sie das Standard-'synclient'-Befehlszeilentool zur Konfiguration von Synaptics-Touchpads:

```bash
$ synclient
```

Um alle verfügbaren Optionen anzuzeigen:

```bash
$ man synaptics
```

Beispiel - Deaktivieren des 'Tap to Click' des Touchpads:

```bash
$ synclient TapButton1=0 TapButton2=0
```

</div>

Für detailliertere Informationen lesen Sie bitte die [Debian-Dokumentation](https://wiki.debian.org/SynapticsTouchpad).

---

## <span style="color: #F77F00;">9. Proprietäre Multimedia-Codecs</span>

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 15px 0;">

Viele Codecs sind bereits in den Standard-Repositories verfügbar. Dazu gehören Codecs für:
- 🎵 MP3
- 🎬 H264
- 🔊 AAC-Encoding und Decoding

Wenn Sie eine zusätzliche Sammlung professioneller Qualitätscodecs installieren möchten, können Sie einen benutzerfreundlichen Installer aus dem **Q4OS Software Center** ausführen.

Medienplayer wie VLC und Mplayer verwenden diese Codecs, um die Wiedergabe von Dateien zu unterstützen, die mit diesen verschiedenen Codecs kodiert wurden.

</div>

---

## <span style="color: #06A77D;">10. Proprietäre Videotreiber</span>

Installieren Sie proprietäre Treiber, um die Videoleistung zu verbessern und vollständige 3D-Beschleunigung zu erhalten. Detaillierte Anweisungen finden Sie auf der [Grafikkarte Debian Wiki](https://wiki.debian.org/GraphicsCard) Seite.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
🎮 <strong>Für NVIDIA-Benutzer:</strong> Wenn Sie eine NVIDIA-Grafikkarte haben, können Sie den Installer aus dem Q4OS Software Center ausführen. Er sondiert die Hardware nach verfügbaren Treibern und installiert sie benutzerfreundlich.
</blockquote>

---

## <span style="color: #D62828;">11. Benutzer und Gruppen</span>

### <span style="color: #D62828;">11.1. Einen regulären Benutzer hinzufügen</span>

Öffnen Sie das Fenster "Benutzer und Gruppen":

```
Control Panel → System Administration → Users and groups
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Schritte:**

1. Klicken Sie auf die Schaltfläche "Hinzufügen"
2. Geben Sie den neuen Benutzernamen an und füllen Sie die Benutzerdetails aus
3. Weisen Sie Benutzer bestimmten Systemgruppen zu, um Benutzerrechte festzulegen

**Empfohlene Gruppen für neue Benutzer:**
- `cdrom` - CD/DVD-Zugriff
- `audio` - Audiowiedergabe
- `video` - Videogeräte
- `plugdev` - Wechselbare Geräte
- `netdev` - Netzwerkverwaltung
- `powerdev` - Energieverwaltung
- `lpadmin` - Druckerinstallation
- `sudo` - Administratorberechtigungen

</div>

---

## <span style="color: #7209B7;">12. Android-Verbindung</span>

Verwenden Sie die Anwendung **gmtp** - einen schnellen und gut organisierten grafischen Dateimanager, der die meisten Telefone und andere Android-Geräte über USB-Kabel mit dem PC verbindet.

```bash
$ sudo apt install gmtp
```

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Verwendung:**

1. Schließen Sie Ihr Gerät über USB-Kabel an
2. Stellen Sie es als MTP-Gerät ein
3. Starten Sie den Dateimanager 'gmtp'

Sie können die interne Verzeichnisstruktur durchsuchen und Dateien von Ihrem Android-Gerät kopieren, löschen und verwalten.

</div>

---

## <span style="color: #F77F00;">13. Sicherheitsupdates, Softwareverwaltung</span>

Q4OS verwendet das Paketverwaltungssystem **Apt** und verwandte Tools zur Aufrechterhaltung der Systemgesundheit und Sauberkeit. Es gibt einen automatischen Mechanismus für unbeaufsichtigte Upgrades, um Sicherheits- und Softwareupdates leise zu erhalten.

Wenn Sie Ihr System sofort manuell aktualisieren müssen, geben Sie Befehle im Terminal ein:

```bash
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
📚 <strong>Weitere Informationen:</strong> Wenn Sie wissen möchten, wie Sie zusätzliche Software installieren, folgen Sie bitte dem Benutzerhandbuch 'Verfügbare Q4OS-Anwendungen', verfügbar im Abschnitt <a href="https://www.q4os.org/documents.html" style="color: #2E86AB;">Dokumente</a> der Q4OS-Website.
</blockquote>

---

### <span style="color: #F77F00;">13.1. Update-Manager</span>

Der Update-Manager benachrichtigt Benutzer über verfügbare Sicherheits- und Softwareupdates und ermöglicht ihnen, das System auf Anfrage zu aktualisieren.

Sie können den Update-Manager einfach aus dem **Q4OS Software Center** installieren.

---

## <span style="color: #06A77D;">14. Externe Software-Repositories</span>

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Nur für Power-User:</strong> Dieses Kapitel richtet sich speziell an Power-User, die mit dem Debian-Paketverwaltungssystem vertraut sind.
</blockquote>

Die Standard-Q4OS-Konfiguration bietet das grundlegende und zuverlässige Set an Software-Repositories. Wenn Sie weitere externe Repositories hinzufügen möchten, können Sie den Standard-Debian-Prozeduren folgen.

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Beispiel: Installation des Opera Web-Browsers**

Listen Sie verfügbare vordefinierte Repositories auf:

```bash
$ sudo qrepoadd --gui
```

Wählen Sie das 'opera'-Repository aus der Dropdown-Liste und klicken Sie auf 'Ok'. Alternativ:

```bash
$ sudo qrepoadd opera
```

Installieren Sie Pakete:

```bash
$ sudo apt update
$ sudo apt install opera-stable
```

**Zum Deinstallieren und Deaktivieren des Repositorys:**

```bash
$ sudo apt autoremove opera-stable
$ sudo qreporm opera
$ sudo apt update
```

</div>

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Warnung:</strong> Das Hinzufügen externer Drittanbieter-Repositories ist eine Low-Level-Systemaktion und könnte die Integrität und Abhängigkeiten der Paketdatenbank tiefgreifend beeinflussen. Glücklicherweise enthält das Apt-Paketverwaltungssystem starke Tools für Administratoren, um defekte Abhängigkeiten zu reparieren.
</blockquote>

---

## <span style="color: #7209B7;">15. Alternative Desktop-Umgebungen</span>

Die Integration anderer Desktop-Umgebungen in das Q4OS-System wird unterstützt. Sie können neben dem Standard-Trinity-Desktop installiert werden, zum Beispiel:
- KDE Plasma
- LXQt
- XFCE
- Und andere

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Installation:**

Sie können eine Desktop-Umgebung mit dem Desktop Profiler-Tool hinzufügen:

```bash
$ swprofiler.exu
```

Klicken Sie auf die Schaltfläche ">" in der oberen rechten Ecke, um eine Desktop-Umgebung auszuwählen und sie zusammen mit einem Desktop-Profil zu installieren.

**Desktop wechseln:**

Nach dem Neustart können Benutzer auswählen, in welche Desktop-Umgebung sie sich anmelden möchten:

1. Klicken Sie auf dem TDM-Anmeldebildschirm auf die Schaltfläche 'Menü'
2. Gehen Sie zu 'Sitzungstyp'
3. Wählen Sie die gewünschte Desktop-Umgebung

</div>

---

## <span style="color: #F77F00;">16. Weitere Sprachen hinzufügen</span>

Es ist möglich, mehrere Sprachen zu Q4OS hinzuzufügen und verschiedene nationale Umgebungen für verschiedene Benutzer einzustellen.

### <span style="color: #F77F00;">16.1. Sprachen hinzufügen</span>

Der Administrator installiert separate Lokalisierungspakete und Benutzer können zwischen verschiedenen Sprachen wechseln.

Starten Sie den neuen Sprachassistenten im Terminal (wiederholen Sie für mehrere Sprachen):

```bash
$ addlanguage
```

Wenn Sie einige Anwendungen mit separaten Lokalisierungspaketen installiert haben, installieren Sie diese ebenfalls. **Libre Office Beispiel:**

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-xx
```

**Optional - Globale System-Locale und Zeitzone ändern:**

```bash
$ sudo dpkg-reconfigure locales
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #F77F00;">16.2. Benutzereinrichtung</span>

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Schritt 1:** Locale auswählen und festlegen (UTF8-Locales bevorzugen):

```bash
$ chqloc --list
$ chqloc --setlocale xx_XX.utf8
```

**Schritt 2:** Neue Benutzersprache auswählen

Öffnen Sie den Dialog "Land/Region und Sprache":

```
Control Panel → Regional & Accessibility → Country/Region & Language
```

Wählen Sie Ihr Land, indem Sie auf die Landschaltfläche klicken. Dadurch wird die Benutzersprache sowie verschiedene nationale Konventionen (Datums-/Uhrzeitformat, Währung usw.) festgelegt.

**Schritt 3:** Eine Tastaturlayout auswählen:

```
Control Panel → Regional & Accessibility → Keyboard Layout
```

Melden Sie sich erneut an - Sie sehen Ihr Profil in der gewählten Sprache übersetzt!

</div>

---

### <span style="color: #F77F00;">16.3. Beispiel</span>

<div style="background-color: #E3F2FD; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

**Szenario:** Frische Installation von Q4OS mit installierter Libre Office Suite. Wir möchten die deutsche Sprache einrichten.

**Schritt 1:** Starten Sie den neuen Sprachassistenten, um Deutsch auszuwählen:

```bash
$ addlanguage
```

**Schritt 2:** Libre Office Sprachpaket:

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-de
```

**Schritt 3:** Deutsche Benutzer-Locale festlegen:

```bash
$ chqloc --list
$ chqloc --setlocale de_DE.utf8
```

**Schritt 4:** Öffnen Sie den Dialog "Land/Region und Sprache":

```
Control Panel → Regional & Accessibility → Country/Region & Language
```

Klicken Sie auf die erste Schaltfläche mit der Landesflagge und wählen Sie "Europa, Mitteleuropa → Deutschland".

**Schritt 5:** Deutsche Tastaturlayout auswählen:

```
Control Panel → Regional & Accessibility → Keyboard Layout
```

**Schritt 6:** Melden Sie sich erneut an - Ihr Profil ist jetzt auf Deutsch! 🇩🇪

</div>

---

## <span style="color: #D62828;">17. Verschiedene Tipps</span>

### <span style="color: #D62828;">17.1. Kickoff Startmenü</span>

Ein gut organisiertes Startmenü im modernen Stil bietet Suchleiste, Favoriten-Reiter, Verlauf und mehr.

Um zum Kickoff-Menü zu wechseln, Rechtsklick auf das Systempanel:

```
Configure Panel → Menus → Start menu style → Kickoff
```

Sie können das Standard-Startmenü auf die gleiche Weise wiederherstellen.

---

### <span style="color: #D62828;">17.2. Ein-Klick-Symbole</span>

Die Symbolaktivierung per Mausklick ist standardmäßig in Q4OS. Es ist einfach, Ein-Klick-Aktivierung einzustellen:

```
Control Panel → Peripherals → Mouse → General tab → Single click to open files and folders
```

---

### <span style="color: #D62828;">17.3. Desktop-Effekte</span>

Aktivieren Sie Glättungs- und Verschönerungseffekte für den Desktop.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Hinweis:</strong> Desktop-Effekte funktionieren nur auf moderner Hardware einwandfrei. Es wird nicht empfohlen, sie mit alter Hardware zu verwenden.
</blockquote>

Desktop-Effekte aktivieren:

```bash
$ ctrl-compmgr --enable
```

Desktop-Effekte deaktivieren:

```bash
$ ctrl-compmgr --disable
```

---

### <span style="color: #D62828;">17.4. Automatische Anmeldung</span>

Es ist möglich, den Anmeldebildschirm zu umgehen und einen angegebenen Benutzer automatisch nach dem Systemstart anzumelden.

Alle möglichen Optionen anzeigen:

```bash
$ sudo ctrl-autologin --help
```

Automatische Anmeldung aktivieren:

```bash
$ sudo ctrl-autologin --enable username
```

---

### <span style="color: #D62828;">17.5. Bildschirmskalierung</span>

Eine frische Q4OS-Installation sollte die Bildschirmauflösung automatisch erkennen. Sie können das System jedoch zwingen, einen benutzerdefinierten DPI-Wert (Punkte pro Zoll) zu verwenden:

```
Control Panel → System Administration → Screen scaling
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tipp:</strong> Eine Erhöhung des DPI-Werts macht Schriftarten und Symbole größer. Ein korrekter Wert für moderne Displays liegt je nach Bildschirmtyp zwischen 120 und 200 DPI.
</blockquote>

---

### <span style="color: #D62828;">17.6. Zeitzonenauswahl</span>

Führen Sie den Befehl im Terminal aus, um die Systemzeitzone auszuwählen:

```bash
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #D62828;">17.7. Root-Passwort</span>

Das Root-Superuser-Passwort ist in Q4OS standardmäßig deaktiviert. Verwenden Sie "sudo", um Befehle als Root auszuführen.

Sie können das Root-Passwort auch manuell aktivieren und ändern, um das Root-Konto direkt verwenden zu können:

```bash
$ sudo passwd
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Einrichtung und Verwendung</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Trinity Desktop Benutzerhandbuch, Rev. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Offizielle Q4OS Website</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Dokumentation</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Community Forum</a>
</p>

</div>
