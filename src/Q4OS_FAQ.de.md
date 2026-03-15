<div align="center">

# 🖥️ <span style="color: #2E86AB;">Q4OS Häufig gestellte Fragen</span>

### <span style="color: #6C757D;">Trinity Desktop Benutzerhandbuch</span>
*<span style="color: #A23B72;">Revision 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Quelle des Dokuments: <a href="https://www.q4os.org/dqa011.html" style="color: #2E86AB;">https://www.q4os.org/dqa011.html</a>
</p>

### 🌐 In Ihrer Sprache lesen:
[🇬🇧 English](Q4OS_FAQ.md) | [🇫🇷 Français](Q4OS_FAQ.fr.md) | [🇩🇪 Deutsch](Q4OS_FAQ.de.md) | [🇪🇸 Español](Q4OS_FAQ.es.md)

</div>

---

## 📑 <span style="color: #2E86AB;">Inhaltsverzeichnis</span>

### <span style="color: #F77F00;">1. [Einleitung](#1-einleitung)</span>

### <span style="color: #06A77D;">2. [Installation](#2-installation)</span>
- 2.1. [Wie erstelle ich eine bootfähige Q4OS Installations-USB-Festplatte?](#21-wie-erstelle-ich-eine-bootfähige-q4os-installations-usb-festplatte)
- 2.2. [Gibt es eine Möglichkeit, Q4OS zusammen mit Windows im Dual-Boot zu betreiben?](#22-gibt-es-eine-möglichkeit-q4os-zusammen-mit-windows-im-dual-boot-zu-betreiben)
- 2.3. [Ich habe nach der Installation keinen Ton, was soll ich tun?](#23-ich-habe-nach-der-installation-keinen-ton-was-soll-ich-tun)
- 2.4. [Keine Verbindung zum drahtlosen Netzwerk möglich, was tun?](#24-keine-verbindung-zum-drahtlosen-netzwerk-möglich-was-tun)

### <span style="color: #D62828;">3. [System](#3-system)</span>
- 3.1. [Es gibt defekte Paketabhängigkeiten in meinem System. Wie kann ich sie reparieren?](#31-es-gibt-defekte-paketabhängigkeiten-in-meinem-system-wie-kann-ich-sie-reparieren)
- 3.2. [Einige Buchstaben werden falsch eingegeben ('L' wird als '3' angezeigt, 'J' als '1')](#32-einige-buchstaben-werden-falsch-eingegeben-l-wird-als-3-angezeigt-j-als-1)
- 3.3. [Schriftarten und Symbole sind auf meinem hiDPI-Bildschirm zu klein, kann ich sie vergrößern?](#33-schriftarten-und-symbole-sind-auf-meinem-hidpi-bildschirm-zu-klein-kann-ich-sie-vergrößern)
- 3.4. [Wie kann ich die aktuelle CPU-Temperatur im Systempanel anzeigen?](#34-wie-kann-ich-die-aktuelle-cpu-temperatur-im-systempanel-anzeigen)
- 3.5. [Ich bin hinter einem Proxy, Paketmanager-basierte Anwendungen funktionieren nicht](#35-ich-bin-hinter-einem-proxy-paketmanager-basierte-anwendungen-funktionieren-nicht)
- 3.6. [Ich möchte einen aktuellen Linux-Kernel verwenden, ist das möglich?](#36-ich-möchte-einen-aktuellen-linux-kernel-verwenden-ist-das-möglich)

### <span style="color: #7209B7;">4. [Desktop](#4-desktop)</span>
- 4.1. [Wie richte ich mehrere virtuelle Desktops in Q4OS ein?](#41-wie-richte-ich-mehrere-virtuelle-desktops-in-q4os-ein)
- 4.2. [Ich kann einige Symbole auf meinem Desktop nicht umbenennen oder bearbeiten](#42-ich-kann-einige-symbole-auf-meinem-desktop-nicht-umbenennen-oder-bearbeiten)
- 4.3. [Wie kann ich das Startmenü bearbeiten?](#43-wie-kann-ich-das-startmenü-bearbeiten)
- 4.4. [Kann ich die Ansicht und Verknüpfungen im rechten Panel des standardmäßigen Q4OS 'Bourbon' Startmenüs anpassen?](#44-kann-ich-die-ansicht-und-verknüpfungen-im-rechten-panel-des-standardmäßigen-q4os-bourbon-startmenüs-anpassen)
- 4.5. [Ich möchte, dass der Eintrag des Willkommensbildschirms im Startmenü angezeigt wird](#45-ich-möchte-dass-der-eintrag-des-willkommensbildschirms-im-startmenü-angezeigt-wird)
- 4.6. [Wie kann ich eine Anwendung automatisch starten?](#46-wie-kann-ich-eine-anwendung-automatisch-starten)
- 4.7. [Ich habe meinen Desktop durcheinander gebracht, wie kann ich Standardfarben, Schriftarten, Thema und andere Desktop-Einstellungen zurücksetzen?](#47-ich-habe-meinen-desktop-durcheinander-gebracht-wie-kann-ich-standardfarben-schriftarten-thema-und-andere-desktop-einstellungen-zurücksetzen)
- 4.8. [Wie kann ich Einfach-Klick-Symbole statt Doppelklick einstellen?](#48-wie-kann-ich-einfach-klick-symbole-statt-doppelklick-einstellen)
- 4.9. [Nennen Sie mir den einfachsten Weg, einen Screenshot zu erstellen](#49-nennen-sie-mir-den-einfachsten-weg-einen-screenshot-zu-erstellen)
- 4.10. [Ist es möglich, das Symbolthema zu ändern?](#410-ist-es-möglich-das-symbolthema-zu-ändern)
- 4.11. [Ich habe Tastenkürzel im Control Panel definiert, aber sie funktionieren nicht](#411-ich-habe-tastenkürzel-im-control-panel-definiert-aber-sie-funktionieren-nicht)
- 4.12. [Ich habe bemerkt, dass der 'Programme'-Eintrag aus dem Startmenü verschwunden ist](#412-ich-habe-bemerkt-dass-der-programme-eintrag-aus-dem-startmenü-verschwunden-ist)
- 4.13. [Tastenkürzel funktioniert nicht zum Wechseln zwischen nicht-lateinischen Tastaturlayouts](#413-tastenkürzel-funktioniert-nicht-zum-wechseln-zwischen-nicht-lateinischen-tastaturlayouts)
- 4.14. [Ich muss die Displayhelligkeit anpassen](#414-ich-muss-die-displayhelligkeit-anpassen)

### <span style="color: #F77F00;">5. [Anwendungen](#5-anwendungen)</span>
- 5.1. [Wie kann ich 'Conky' Transparenz einrichten?](#51-wie-kann-ich-conky-transparenz-einrichten)

---

## <span style="color: #F77F00;">1. Einleitung</span>

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
📢 Melden Sie uns alle Fehler, die Sie finden, Vorschläge sind willkommen. Senden Sie uns möglichst, was Ihrer Meinung nach eine klarere Lösung wäre. Sie können sich sicher an die <a href="http://www.trinitydesktop.org/faq/index.php" style="color: #2E86AB;">Trinity Desktop Environment FAQ</a> halten.
</blockquote>

---

## <span style="color: #06A77D;">2. Installation</span>

### <span style="color: #06A77D;">2.1. Wie erstelle ich eine bootfähige Q4OS Installations-USB-Festplatte?</span>

Der einfachste Weg unter Linux ist, Ihr USB-Gerät anzuschließen, nicht einzuhängen und im Terminal auszuführen:

```bash
$ sudo cp bootable.iso /dev/sdx
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Hinweis:</strong><br>
• <code>sdx</code> ist das Ziel-USB-Laufwerk, zum Beispiel <code>sdb</code><br>
• <code>bootable.iso</code> ist das bootfähige Q4OS Installations-CD-Image, Sie können es von der Q4OS Website herunterladen
</blockquote>

Alternativ können Sie die plattformübergreifende Software **UNetbootin** oder **Rufus** verwenden, um bootfähige USB-Festplatten zu erstellen. Siehe [So erstellen Sie ein Live-Medium](https://www.q4os.org/dqa018.html#creat).

---

### <span style="color: #06A77D;">2.2. Gibt es eine Möglichkeit, Q4OS zusammen mit Windows im Dual-Boot zu betreiben?</span>

Klar! Der bevorzugte Weg ist die Installation von einer 'Live' CD, da dies Ihnen die Option zur Installation des Bootloaders gibt. Wenn Sie den Installer den Grub-Bootloader installieren lassen, erkennt er automatisch verfügbare Betriebssysteme einschließlich Windows und bietet sie bei jedem Start an.

Wenn Sie den Windows-Bootloader behalten möchten, vergessen Sie nicht, das entsprechende Kontrollkästchen während der Installation zu deaktivieren.

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Wichtig:</strong> Wir empfehlen dringend, vorher alle Ihre Daten zu sichern. Bitte lesen Sie die <a href="https://www.q4os.org/dqa018.html" style="color: #D62828;">Installationsanweisungen</a>.
</blockquote>

---

### <span style="color: #06A77D;">2.3. Ich habe nach der Installation keinen Ton, was soll ich tun?</span>

Wir empfehlen Ihnen, zuerst den Pipewire-Soundserver zu installieren:

```bash
$ sudo apt install pipewire pavucontrol-qt
```

Starten Sie Ihren Computer neu. Befolgen Sie dann diese Schritte:

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Konfigurationsschritte:**

1. Rechtsklick auf das 'Mixer'-Symbol in der Systemleiste → 'Masterkanal auswählen...'
2. Stellen Sie 'Aktueller Mixer' in der oberen rechten Dropdown-Liste auf 'PipeWire'
3. Klicken Sie auf 'Ok', um den Dialog zu schließen
4. Starten Sie die Anwendung 'Lautstärkeregelung' über das Startmenü
5. Konfigurieren Sie die Ausgangsmixereinstellungen im Reiter 'Ausgabegeräte'
6. Überprüfen Sie, ob die Ausgangskanäle nicht stummgeschaltet sind

</div>

Das Audiosystem sollte jetzt funktionieren. Wenn nicht, fahren Sie fort, die folgenden Schritte zu befolgen.

**Zusätzliche Diagnose:**

Linksklick auf das 'Mixer'-Symbol in der Systemleiste und klicken Sie auf die Schaltfläche 'Mixer', um die Audio-Mixer-Pegel zu überprüfen und zu aktualisieren. Stellen Sie sicher, dass die Soundkarte 'PipeWire' in der oberen rechten Ecke des 'kmix' Mixer-Fensters ausgewählt ist.

Führen Sie dann den Befehl im Terminal aus und überprüfen Sie die Debug-Ausgabe:

```bash
$ artsplay /opt/trinity/share/sounds/KDE_Startup.wav
```

Wenn es immer noch keinen Ton gibt, beenden Sie vorübergehend den Trinity-Soundserver und versuchen Sie, Audio mit einem unabhängigen alsa-Player abzuspielen:

```bash
$ artsshell terminate
$ aplay /opt/trinity/share/sounds/KDE_Startup.wav
```

Überprüfen Sie erneut die Debug-Ausgabe. Wenn Ihr Audiosystem immer noch nicht funktioniert, fahren Sie mit der [Fehlerbehebung bei Soundproblemen](http://www.trinitydesktop.org/faq/sound.php) in der Trinity FAQ fort.

---

### <span style="color: #06A77D;">2.4. Keine Verbindung zum drahtlosen Netzwerk möglich, was tun?</span>

Q4OS unterstützt drahtlose Netzwerke vollständig und enthält ein Tool namens **tdenetworkmanager** zur Verwaltung drahtloser Verbindungen. Sie finden es in der Systemleiste.

Wenn Sie Probleme beim Verbinden mit einem drahtlosen Netzwerk haben, lesen Sie bitte den [Beitrag zur WLAN-Fehlerbehebung](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #D62828;">3. System</span>

### <span style="color: #D62828;">3.1. Es gibt defekte Paketabhängigkeiten in meinem System. Wie kann ich sie reparieren?</span>

Wir haben ein praktisches Tool zur automatischen Reparatur defekter Abhängigkeiten in Q4OS, führen Sie einfach im Terminal aus:

```bash
$ sudo sh /usr/share/apps/q4os_system/bin/qapt_fix.sh
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Erinnerung:</strong> Wir empfehlen dringend, Software nur aus zuverlässigen und Debian-kompatiblen Quellen zu installieren, um eine Beschädigung des Paketsystems zu verhindern.
</blockquote>

---

### <span style="color: #D62828;">3.2. Einige Buchstaben werden falsch eingegeben ('L' wird als '3' angezeigt, 'J' als '1')</span>

Eine häufige Störung, die auf Netbooks mit kleiner Tastatur auftritt. Die Tastatur ist durch NumLock blockiert, Sie könnten versuchen, NumLock auszuschalten.

Starten Sie das Control Panel:

```
Control Panel → Peripheriegeräte → Tastatur → NumLock bei KDE-Start → auf Aus stellen
```

Melden Sie sich erneut an und testen Sie die Tastatur.

---

### <span style="color: #D62828;">3.3. Schriftarten und Symbole sind auf meinem hiDPI-Bildschirm zu klein, kann ich sie vergrößern?</span>

Ja, Q4OS kann die Bildschirmauflösung skalieren. Bitte lesen Sie das Kapitel [Bildschirmauflösung](https://www.q4os.org/dqa007.html#tips.6).

---

### <span style="color: #D62828;">3.4. Wie kann ich die aktuelle CPU-Temperatur im Systempanel anzeigen?</span>

Starten Sie die Anwendung **ksensors** von:

```
Startmenü → Programme → Zubehör → System → KSensors
```

Wenn **ksensors** noch nicht installiert ist, folgen Sie dem Kapitel [Hardwaresensoren](https://www.q4os.org/dqa007.html#hwsens), um es zu installieren.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0; border-left: 5px solid #7209B7;">

**Konfiguration:**

1. Rechtsklick auf das 'ksensors'-Symbol in der Systemleiste → Konfigurieren
2. Wählen Sie die betreffende HW-Sensoren-Gruppe
3. Wählen Sie den gewünschten Sensor aus der Liste
4. Dock-Reiter → Haken Sie das Kontrollkästchen 'Sichtbar'
5. Sie können optional Farben, Alarme, Schwellenwerte, Aktionen bei Grenzwertüberschreitungen und andere Optionen einstellen
6. Klicken Sie auf die Schaltfläche 'Anwenden' und schließen Sie den Dialog

</div>

---

### <span style="color: #D62828;">3.5. Ich bin hinter einem Proxy, Paketmanager-basierte Anwendungen funktionieren nicht</span>

Sie müssen systemweite Umgebungsvariablen festlegen. Öffnen Sie die Datei `/etc/environment` mit Ihrem bevorzugten Editor und fügen Sie die folgenden Zeilen hinzu (entsprechend anpassen):

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
📝 <strong>Hinweis:</strong> Sie müssen sowohl in Groß- als auch in Kleinbuchstaben duplizieren, da einige Programme nur nach dem einen oder anderen suchen.
</blockquote>

Das APT-Paketverwaltungssystem wird den Umgebungsvariablen nicht gehorchen, wenn es normal mit sudo verwendet wird. Konfigurieren Sie sie also separat; erstellen Sie eine Datei namens `95proxies` in `/etc/apt/apt.conf.d/`, und fügen Sie Folgendes ein:

```bash
Acquire::http::proxy "http://myproxy.server.com:8080/";
Acquire::ftp::proxy "ftp://myproxy.server.com:8080/";
Acquire::https::proxy "https://myproxy.server.com:8080/";
```

Starten Sie schließlich neu, um sicherzustellen, dass die Änderungen wirksam werden.

---

### <span style="color: #D62828;">3.6. Ich möchte einen aktuellen Linux-Kernel verwenden, ist das möglich?</span>

Wir empfehlen die Verwendung des zuverlässigen und tiefgreifend bewährten standardmäßigen Q4OS/Debian-Kernels. Es gibt nicht allzu viele Gründe für gewöhnliche Benutzer, einen neueren Kernel zu verwenden.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Warnung:</strong> Die neuesten Kernel sind nicht so sicher wie der felsfeste und erschöpfend getestete standardmäßige Debian-Kernel, sie können jedoch Verbesserungen und neuere Gerätetreiber und Unterstützung bringen.
</blockquote>

Wenn Sie aus irgendeinem Grund den neuesten Linux-Kernel bevorzugen, führen Sie das Auto-Installation-Skript im Terminal aus, um ihn einfach aus dem Backports-Repository zu installieren:

```bash
$ qinst-kernel-bpo
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Gut zu wissen:</strong> Der alte gute Standard-Kernel wird nicht deinstalliert, sodass Sie ihn jederzeit aus dem Grub-Bootmenü auswählen und starten können, falls Sie in Probleme geraten.
</blockquote>

---

## <span style="color: #7209B7;">4. Desktop</span>

### <span style="color: #7209B7;">4.1. Wie richte ich mehrere virtuelle Desktops in Q4OS ein?</span>

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Schritt 1:** Starten Sie das Control Panel und gehen Sie zu:

```
Desktop → Mehrere Desktops
```

Wählen Sie, wie viele virtuelle Desktops Sie haben möchten.

**Schritt 2a:** Fügen Sie ein Desktop-Umschalt-Applet zu Ihrer Taskleiste hinzu:

1. Rechtsklick auf die Taskleiste
2. Wählen Sie 'Applet zum Panel hinzufügen' (wenn die Taskleiste gesperrt ist, entsperren Sie sie zuerst)
3. Wählen Sie im Popup-Fenster 'Desktop Pager / Switcher'
4. Klicken Sie auf 'Zum Panel hinzufügen'

**Schritt 3a:** Konfigurieren Sie ein Tastenkürzel:

1. Starten Sie das Control Panel
2. Gehen Sie zu: `Regional & Zugänglichkeit → Tastenkürzel`
3. Scrollen Sie im Reiter 'Globale Kürzel' nach unten und finden Sie 'Zum nächsten Desktop wechseln' unter 'Desktop-Umschaltung'
4. Klicken Sie auf die Schaltfläche neben der Option 'Benutzerdefiniert'
5. Weisen Sie die Tastenkombination zu, die Sie verwenden möchten
6. Klicken Sie auf 'OK', um zu speichern

</div>

---

### <span style="color: #7209B7;">4.2. Ich kann einige Symbole auf meinem Desktop nicht umbenennen oder bearbeiten</span>

Es könnten drei logische Typen von Symbolen auf Ihrem Desktop vorhanden sein:

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 10px 0;">

**1. Systemsymbole** 🔒
- 'Mein Computer', 'Meine Dokumente', 'Meine Netzwerkorte', 'Papierkorb', 'Webbrowser', 'Drucker'
- Gehören root
- Von einem Benutzer nicht direkt bearbeitbar
- Können vom Desktop entfernt werden

**2. Globale Symbole** 🌐
- Normalerweise von Anwendungsinstallern erstellt
- Gehören root und werden von allen Benutzern gemeinsam genutzt
- Benutzer können sie ausblenden, aber nicht bearbeiten oder umbenennen

**3. Benutzersymbole** 👤
- Von einem einzelnen Benutzer erstellt
- Vollständige Kontrolle: löschen, umbenennen, Eigenschaften bearbeiten (Rechtsklick → Eigenschaften)

</div>

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Tipp:</strong> Wenn Sie ein globales oder Systemsymbol bearbeiten möchten, empfehlen wir, es vom Desktop zu entfernen und ein entsprechendes Benutzersymbol mithilfe von Drag&Drop → Kopieren aus dem Startmenü zu erstellen. Es gehört dem Benutzer und ist vollständig bearbeitbar.
</blockquote>

---

### <span style="color: #7209B7;">4.3. Wie kann ich das Startmenü bearbeiten?</span>

1. Öffnen Sie das Startmenü
2. Rechtsklick auf einen beliebigen Eintrag unter 'Programme'
3. Wählen Sie 'Menü bearbeiten'
4. Das Menüeditor-Fenster erscheint

Sie können neue benutzerdefinierte Untermenüs/Ordnerstrukturen erstellen und sie mit gewünschten Menüeinträgen füllen. Sie können neue Verknüpfungen mit der rechten Maustaste erstellen oder Symbole vom Startmenü oder Desktop in das Menüeditor-Fenster ziehen.

Neu erstellte Elemente erscheinen im Startmenü nach dem Schließen des Menüeditor-Fensters.

**Bonus:** Sie können auch umschalten, ob Startmenüeinträge nach Kategorien oder nach Anwendungen organisiert sind:

```bash
$ sh /usr/share/apps/q4os_system/bin/kmenu_struct.sh --help
```

---

### <span style="color: #7209B7;">4.4. Kann ich die Ansicht und Verknüpfungen im rechten Panel des standardmäßigen Q4OS 'Bourbon' Startmenüs anpassen?</span>

Ja! Bearbeiten Sie die Datei `$HOME/.trinity/share/config/kickerrc` in Ihrem Home-Verzeichnis.

Es gibt mehrere Konfigurationsoptionen, die mit 'Bourbon' beginnen und standardmäßig auskommentiert sind. Sie müssen:

1. Die Zeile `BourbonSysViewCustomItems` auskommentieren
2. `.desktop` Verknüpfungen angeben, die im rechten Menüpanel angezeigt werden sollen
3. Komma `,` als Trennzeichen verwenden

**Zusätzliche Optionen:**

- Standardverknüpfungen ausblenden:
  - `BourbonShowSysViewFolders=false`
  - `BourbonShowSysViewApps=false`

---

### <span style="color: #7209B7;">4.5. Ich möchte, dass der Eintrag des Willkommensbildschirms im Startmenü angezeigt wird</span>

Führen Sie den Befehl aus, um die Willkommensbildschirm-Verknüpfung im Terminal zu aktualisieren:

```bash
$ sudo kwriteconfig --file '/usr/share/applications/q4os-welcome-screen.desktop' --group 'Desktop Entry' --key 'NoDisplay' 'false'
```

Alternativ können Sie die Datei `/usr/share/applications/q4os-welcome-screen.desktop` manuell bearbeiten.

Das Willkommensbildschirm-Symbol erscheint unter:

```
Startmenü → Programme → Zubehör → System
```

---

### <span style="color: #7209B7;">4.6. Wie kann ich eine Anwendung automatisch starten?</span>

Sie müssen eine Anwendungsverknüpfung (`.desktop` Datei) in den Autostart-Ordner hinzufügen:

- `$HOME/.trinity/Autostart`
- oder `$HOME/.q4data/Programs/Startup`

Die Anwendung wird unmittelbar nach der Benutzeranmeldung gestartet.

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Methoden:**

1. Ziehen Sie eine beliebige Anwendungsverknüpfung aus dem Startmenü oder Desktop und legen Sie sie im Autostart-Ordner ab
2. Es ist auch möglich, ein Shell-Skript oder eine ausführbare Datei in den Autostart-Ordner zu platzieren

</div>

---

### <span style="color: #7209B7;">4.7. Ich habe meinen Desktop durcheinander gebracht, wie kann ich Standardfarben, Schriftarten, Thema und andere Desktop-Einstellungen zurücksetzen?</span>

Einfach im Terminal ausführen:

```bash
$ sh /usr/share/apps/q4os_system/bin/default_desktop_settings.sh
```

---

### <span style="color: #7209B7;">4.8. Wie kann ich Einfach-Klick-Symbole statt Doppelklick einstellen?</span>

Symbolaktivierung durch Mausklick ist standardmäßig in Q4OS. Es ist einfach, Einfach-Klick-Aktivierung, Hover-Effekt und mehr im Control Panel einzustellen:

```
Control Panel → Peripheriegeräte → Maus → Reiter Allgemein → Dateien und Ordner mit Einfachklick öffnen
```

---

### <span style="color: #7209B7;">4.9. Nennen Sie mir den einfachsten Weg, einen Screenshot zu erstellen</span>

Sie können dies ohne zusätzliche Pakete tun:

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Schnelle Methode:**

1. Drücken Sie die `PrtScr` Taste
2. Rechtsklick auf den Desktop
3. Wählen Sie 'Inhalt der Zwischenablage einfügen'
4. Ein Dialog erscheint, in dem Sie den Dateinamen und Bildtyp eingeben können
5. Die Datei wird auf dem Desktop gespeichert

Sie können auch Konqueror öffnen, um zum bevorzugten Ordner zu navigieren, rechtsklicken und 'Inhalt der Zwischenablage einfügen' auswählen, um die Datei am bevorzugten Speicherort zu speichern.

</div>

**Dedizierte Anwendung:**

Es gibt eine leichte und leistungsstarke Anwendung **ksnapshot-trinity**, die in der Lage ist, den gesamten Bildschirm, eine Region, ein Fenster oder nur einen Fensterteil zu erfassen.

Installation:

```bash
$ sudo apt install ksnapshot-trinity
```

---

### <span style="color: #7209B7;">4.10. Ist es möglich, das Symbolthema zu ändern?</span>

Ja! Sie müssen erweiterte Control Panel Optionen im Terminal entsperren:

```bash
$ sudo kcmodules --unlock
```

Gehen Sie dann zu:

```
Control Panel → Erscheinungsbild & Themen → Symbole
```

Richten Sie das gewünschte Thema ein.

---

### <span style="color: #7209B7;">4.11. Ich habe Tastenkürzel im Control Panel definiert, aber sie funktionieren nicht</span>

Sie müssen nur den khotkeys-Dienst aktivieren, damit er bei der Sitzungsanmeldung ausgeführt wird.

Gehen Sie zum Control Panel:

```
Control Panel → Regional & Zugänglichkeit → Eingabeaktionen → Reiter Allgemeine Einstellungen → Haken Sie das Kontrollkästchen 'KHotKeys deaktivieren' heraus
```

---

### <span style="color: #7209B7;">4.12. Ich habe bemerkt, dass der 'Programme'-Eintrag aus dem Startmenü verschwunden ist</span>

Dies geschieht selten auf einigen speziell konfigurierten Systemen. Die Problemumgehung, die es beheben sollte, ist das erneute Umschalten von klassisch - kicker - klassisch.

Sie könnten es als neuen Fehler in unserem [Bug Tracker](https://sourceforge.net/p/q4os/tickets) melden und eine Beschreibung hinzufügen, wenn Sie Zusammenhänge finden.

---

### <span style="color: #7209B7;">4.13. Tastenkürzel funktioniert nicht zum Wechseln zwischen nicht-lateinischen Tastaturlayouts</span>

Das Tastaturwechsel-Kürzel ist standardmäßig `Alt+Leertaste` oder `Ctrl+Alt+K`. Es funktioniert einwandfrei, wenn Sie nur lateinische Tastaturlayouts installiert haben.

Um nicht-lateinische Tastaturen frei wechseln zu können, müssen Sie zu jeder verwendeten Tastatur ein 'lateinischen Layout' hinzufügen.

Führen Sie das Control Panel aus:

```
Control Panel → Regional & Zugänglichkeit → Tastaturlayout → wählen Sie ein nicht-lateinisches Tastaturlayout → Haken Sie das Kontrollkästchen 'Lateinisches Layout einschließen'
```

---

### <span style="color: #7209B7;">4.14. Ich muss die Displayhelligkeit anpassen</span>

Fahren Sie einfach mit der Maus über das **tdepowersave** Symbol in der Systemleiste und verwenden Sie das Mausrad, um die Helligkeit nach oben oder unten anzupassen.

Wenn das Symbol in der Systemleiste nicht verfügbar ist, müssen Sie das Paket `tdepowersave-trinity` installieren und sich erneut bei der Trinity-Desktopsitzung anmelden.

**Alternative:**

Sie können das Paket `klcddimmer-trinity` installieren und ein Applet im Systempanel hinzufügen. Sie müssen es jedoch so konfigurieren, dass es ein Helligkeitssteuerungs-Backend verwendet, zum Beispiel `xbacklight`.

---

## <span style="color: #F77F00;">5. Anwendungen</span>

### <span style="color: #F77F00;">5.1. Wie kann ich 'Conky' Transparenz einrichten?</span>

Sie müssen Q4OS/Trinity Desktop-Effekte aktiviert haben. Dies kann über den Willkommensbildschirm oder das Control Panel eingerichtet werden.

Bearbeiten Sie die Datei `/etc/conky/conky.conf` und fügen Sie Zeilen hinzu:

```bash
own_window yes
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
own_window_argb_visual
own_window_argb_value 0
```

Kommentieren Sie die Zeile:

```bash
#own_window_type desktop
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Häufig gestellte Fragen</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Trinity Desktop Benutzerhandbuch, Rev. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Offizielle Q4OS Website</a> | 
🐛 <a href="https://sourceforge.net/p/q4os/tickets" style="color: #FFD700; text-decoration: none;">Bug Tracker</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Forum</a>
</p>

</div>
