<div align="center">

# ⚙️ <span style="color: #2E86AB;">Q4OS Configuration et Utilisation</span>

### <span style="color: #6C757D;">Manuel Utilisateur Trinity Desktop</span>
*<span style="color: #A23B72;">Révision 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source du document : <a href="https://www.q4os.org/dqa007.html" style="color: #2E86AB;">https://www.q4os.org/dqa007.html</a>
</p>

### 🌐 Lire dans votre langue :
[🇬🇧 English](Q4OS_Setup_and_Using.md) | [🇫🇷 Français](Q4OS_Setup_and_Using.fr.md) | [🇩🇪 Deutsch](Q4OS_Setup_and_Using.de.md) | [🇪🇸 Español](Q4OS_Setup_and_Using.es.md)

</div>

---

## 📑 <span style="color: #2E86AB;">Table des matières</span>

1. [Introduction](#1-introduction)
2. [Test](#2-test)
   - 2.1. [Live CD](#21-live-cd)
   - 2.2. [Dans Virtualbox](#22-dans-virtualbox)
3. [Installation](#3-installation)
4. [Configuration réseau sans fil](#4-configuration-réseau-sans-fil)
5. [Impression et numérisation](#5-impression-et-numérisation)
   - 5.1. [Imprimantes et scanners Hewlett-Packard](#51-imprimantes-et-scanners-hewlett-packard)
   - 5.2. [Autres imprimantes](#52-autres-imprimantes)
   - 5.3. [Scanners](#53-scanners)
6. [Gestion de l'alimentation](#6-gestion-de-lalimentation)
7. [Capteurs matériels](#7-capteurs-matériels)
8. [Pavé tactile](#8-pavé-tactile)
9. [Codecs multimédia propriétaires](#9-codecs-multimédia-propriétaires)
10. [Pilotes vidéo propriétaires](#10-pilotes-vidéo-propriétaires)
11. [Utilisateurs et groupes](#11-utilisateurs-et-groupes)
    - 11.1. [Ajout d'un utilisateur régulier](#111-ajout-dun-utilisateur-régulier)
12. [Interconnexion Android](#12-interconnexion-android)
13. [Mises à jour de sécurité, gestion des logiciels](#13-mises-à-jour-de-sécurité-gestion-des-logiciels)
    - 13.1. [Gestionnaire de mises à jour](#131-gestionnaire-de-mises-à-jour)
14. [Dépôts de logiciels externes](#14-dépôts-de-logiciels-externes)
15. [Environnements de bureau alternatifs](#15-environnements-de-bureau-alternatifs)
16. [Ajout de plusieurs langues](#16-ajout-de-plusieurs-langues)
    - 16.1. [Ajouter des langues](#161-ajouter-des-langues)
    - 16.2. [Configuration utilisateur](#162-configuration-utilisateur)
    - 16.3. [Exemple](#163-exemple)
17. [Divers conseils](#17-divers-conseils)
    - 17.1. [Menu Démarrer Kickoff](#171-menu-démarrer-kickoff)
    - 17.2. [Icônes à simple clic](#172-icônes-à-simple-clic)
    - 17.3. [Effets de bureau](#173-effets-de-bureau)
    - 17.4. [Connexion automatique](#174-connexion-automatique)
    - 17.5. [Mise à l'échelle de l'écran](#175-mise-à-léchelle-de-lécran)
    - 17.6. [Sélection du fuseau horaire](#176-sélection-du-fuseau-horaire)
    - 17.7. [Mot de passe root](#177-mot-de-passe-root)

---

## <span style="color: #F77F00;">1. Introduction</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

Ce document couvre comment configurer, paramétrer et utiliser le système d'exploitation Q4OS.

Q4OS est recommandé pour être utilisé sur des machines de production, car il a été construit sur la base du système Debian extrêmement stable, sécurisé et fiable, testé par de nombreuses personnes à travers le monde.

Il existe une énorme base logicielle stable dans les dépôts par défaut - vous êtes libre de l'utiliser et d'adapter le système selon vos besoins.

</div>

---

## <span style="color: #06A77D;">2. Test</span>

### <span style="color: #06A77D;">2.1. Live CD</span>

Si vous souhaitez obtenir une expérience rapide de Q4OS ou le tester sur du matériel réel, vous pouvez démarrer en toute sécurité un CD ou USB live Q4OS.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Test sans risque :</strong> Il n'écrira rien sur votre disque dur et n'affectera pas votre installation existante. Il est possible d'installer le système Q4OS directement depuis le média live en utilisant l'installateur live.
</blockquote>

---

### <span style="color: #06A77D;">2.2. Dans Virtualbox</span>

Nous recommandons d'installer Q4OS dans [Virtualbox](http://www.virtualbox.org/) à des fins de test.

**Configuration :**
- Système d'exploitation : **Linux**
- Version : **Debian (32/64 bits)**

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Astuce :</strong> Il est approprié d'installer les "Additions invité Virtualbox" dans le système invité pour obtenir les meilleures performances. Un auto-installeur pratique est disponible dans le 'Centre logiciel' Q4OS. L'installateur contient des pilotes optimisés et il est préférable de l'installer plutôt que depuis les sources originales d'Oracle ou d'autres.
</blockquote>

---

## <span style="color: #D62828;">3. Installation</span>

Veuillez lire le [guide d'installation](https://www.q4os.org/dqa018.html) de Q4OS fraîche.

---

## <span style="color: #7209B7;">4. Configuration réseau sans fil</span>

Q4OS prend entièrement en charge les réseaux sans fil et inclut un outil appelé **tdenetworkmanager** pour gérer les connexions sans fil. Vous pouvez le trouver dans la zone système.

Si vous rencontrez des problèmes de connexion à un réseau sans fil, veuillez lire le [message de dépannage wifi](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #F77F00;">5. Impression et numérisation</span>

### <span style="color: #F77F00;">5.1. Imprimantes et scanners Hewlett-Packard</span>

Installez le système d'impression et d'imagerie HP Linux, satisfaites les dépendances et configurez une imprimante dans le terminal :

```bash
$ sudo apt install hplip hplip-gui avahi-utils cups
$ sudo apt install libcupsimage2-dev libdbus-1-dev libssl-dev libusb-1.0.0-dev python-dev
$ sudo hp-setup
```

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Note :</strong> Certaines imprimantes HP nécessitent un plugin de pilote téléchargeable. La commande 'hp-setup' téléchargera et installera automatiquement le plugin.
</blockquote>

---

### <span style="color: #F77F00;">5.2. Autres imprimantes</span>

Listez d'abord les pilotes et choisissez celui approprié pour votre modèle :

```bash
$ apt-cache search printer-driver
```

Installez un ensemble spécifique de pilotes, par exemple pour les imprimantes laser Samsung :

```bash
$ sudo apt install printer-driver-splix cups
```

Ou vous pouvez installer tous les pilotes d'imprimante disponibles :

```bash
$ sudo apt install foomatic-db printer-driver-all cups
```

Ensuite, ajoutez et configurez les imprimantes :

```
Menu Démarrer → Applications → Paramètres → Système d'impression
```

Vous pouvez trouver des informations supplémentaires précieuses sur le [wiki Debian](https://wiki.debian.org/SystemPrinting).

---

### <span style="color: #F77F00;">5.3. Scanners</span>

Nous recommandons d'utiliser l'application **Kooka** pour la numérisation. Installez le logiciel requis et ajoutez tous les utilisateurs qui ont besoin d'accéder au groupe 'scanner' :

```bash
$ sudo apt install libsane sane sane-utils xsane kooka-trinity
$ sudo adduser votre_nom_utilisateur scanner
```

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Important :</strong> L'utilisateur devra se déconnecter et se reconnecter pour que le nouveau groupe prenne effet.
</blockquote>

Vérifiez que le scanner est maintenant reconnu :

```bash
$ scanimage -L
$ sane-find-scanner
```

Si vous souhaitez configurer une numérisation réseau, consultez [Sane en réseau](https://wiki.debian.org/SaneOverNetwork).

---

## <span style="color: #06A77D;">6. Gestion de l'alimentation</span>

Il est souhaitable d'installer une application de contrôle de l'alimentation pour les ordinateurs portables et les appareils mobiles :

```bash
$ sudo apt update
$ sudo apt install rfkill tdepowersave-trinity
```

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 15px 0;">

Connectez-vous à nouveau, une belle application de contrôle de l'alimentation sera présente dans la zone système.

**Fonctionnalités :**
- 🔋 Contrôler la fréquence du CPU
- 📊 Voir l'état de la batterie
- 💤 Configurer les actions de veille et d'hibernation
- 🔘 Gérer les événements de fermeture du couvercle
- ⚡ Configuration du bouton d'alimentation

</div>

---

## <span style="color: #D62828;">7. Capteurs matériels</span>

La plupart des ordinateurs sont équipés de divers capteurs, qui peuvent être utilisés pour surveiller votre matériel et éviter les pannes inattendues. C'est là que l'application **ksensors** intervient.

```bash
$ sudo apt install ksensors-trinity
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

Vous trouverez l'application de surveillance 'ksensors' dans le menu Démarrer ou dans la zone système.

**Fonctionnalités :**
- 🌡️ Surveillance de la température
- ⚡ Capteurs de tension
- 🌀 Surveillance de la vitesse des ventilateurs
- 🔔 Alarmes et seuils
- ⚙️ Actions sur le dépassement des limites

</div>

Q4OS devrait reconnaître automatiquement les capteurs disponibles dès la première utilisation. Sinon, vous devez détecter les modules noyau nécessaires :

```bash
$ sudo sensors-detect
```

Il vous sera demandé à la fin du processus de numérisation si vous voulez que ce qu'il trouve soit ajouté au fichier '/etc/modules'. Répondez 'oui' puis redémarrez.

---

## <span style="color: #7209B7;">8. Pavé tactile</span>

Q4OS utilise le pilote **libinput** pour contrôler le pavé tactile et les périphériques de pointage associés par défaut.

Vérifiez la liste complète des options de configuration 'libinput' :

```bash
$ man libinput
```

Toutes les options peuvent être appliquées dans le fichier `/etc/X11/xorg.conf.d/60-libinput.conf`.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Alternative : Pilote Synaptics**

Vous pouvez faire en sorte qu'un ancien pilote 'synaptics' ait priorité sur 'libinput' :

```bash
$ sudo apt install xserver-xorg-input-synaptics
```

Utilisez l'outil en ligne de commande 'synclient' par défaut pour configurer les pavés tactiles Synaptics :

```bash
$ synclient
```

Pour voir toutes les options disponibles :

```bash
$ man synaptics
```

Exemple - désactiver le 'tap to click' du pavé tactile :

```bash
$ synclient TapButton1=0 TapButton2=0
```

</div>

Pour plus d'informations détaillées, veuillez lire la [documentation Debian](https://wiki.debian.org/SynapticsTouchpad).

---

## <span style="color: #F77F00;">9. Codecs multimédia propriétaires</span>

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 15px 0;">

De nombreux codecs sont déjà disponibles dans les dépôts par défaut. Ceux-ci incluent les codecs pour :
- 🎵 MP3
- 🎬 H264
- 🔊 Encodage et décodage AAC

Si vous souhaitez installer une collection supplémentaire de codecs de qualité professionnelle, vous pouvez exécuter un installateur facile à utiliser depuis le **Centre logiciel Q4OS**.

Les lecteurs multimédias tels que VLC et Mplayer utilisent ces codecs afin de fournir la prise en charge de la lecture de fichiers encodés via ces nombreux codecs différents.

</div>

---

## <span style="color: #06A77D;">10. Pilotes vidéo propriétaires</span>

Installez des pilotes propriétaires pour améliorer les performances vidéo et obtenir une accélération 3D complète. Consultez la page du [wiki Debian sur les cartes graphiques](https://wiki.debian.org/GraphicsCard) pour des instructions détaillées.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
🎮 <strong>Pour les utilisateurs NVIDIA :</strong> Si vous avez une carte graphique NVIDIA, vous pouvez exécuter l'installateur depuis le Centre logiciel Q4OS. Il sondra le matériel pour les pilotes disponibles et les installera de manière conviviale.
</blockquote>

---

## <span style="color: #D62828;">11. Utilisateurs et groupes</span>

### <span style="color: #D62828;">11.1. Ajout d'un utilisateur régulier</span>

Ouvrez la fenêtre "Utilisateurs et groupes" :

```
Panneau de configuration → Administration système → Utilisateurs et groupes
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Étapes :**

1. Cliquez sur le bouton "Ajouter"
2. Spécifiez le nouveau nom d'utilisateur et remplissez les détails de l'utilisateur
3. Assignez les utilisateurs à des groupes système spécifiques pour définir les droits d'utilisateur

**Groupes recommandés pour les nouveaux utilisateurs :**
- `cdrom` - Accès CD/DVD
- `audio` - Lecture audio
- `video` - Périphériques vidéo
- `plugdev` - Périphériques amovibles
- `netdev` - Gestion réseau
- `powerdev` - Gestion de l'alimentation
- `lpadmin` - Installation d'imprimante
- `sudo` - Permissions d'administrateur

</div>

---

## <span style="color: #7209B7;">12. Interconnexion Android</span>

Utilisez l'application **gmtp** - un gestionnaire de fichiers graphique rapide et bien organisé qui connecte la plupart des téléphones et autres appareils Android au PC via un câble USB.

```bash
$ sudo apt install gmtp
```

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Utilisation :**

1. Connectez votre appareil via un câble USB
2. Définissez-le comme appareil MTP
3. Lancez le gestionnaire de fichiers 'gmtp'

Vous pourrez parcourir la structure de répertoires interne et copier, supprimer et gérer des fichiers depuis votre appareil Android.

</div>

---

## <span style="color: #F77F00;">13. Mises à jour de sécurité, gestion des logiciels</span>

Q4OS utilise le système de gestion de paquets **Apt** et les outils associés pour maintenir la santé et la propreté du système. Il existe un mécanisme de mises à jour automatiques sans intervention pour obtenir silencieusement les mises à jour de sécurité et de logiciels.

Si vous devez mettre à jour votre système immédiatement manuellement, exécutez les commandes dans le terminal :

```bash
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
📚 <strong>Pour plus d'informations :</strong> Si vous souhaitez savoir comment installer des logiciels supplémentaires, veuillez suivre le manuel de l'utilisateur 'Applications Q4OS disponibles', disponible dans la section <a href="https://www.q4os.org/documents.html" style="color: #2E86AB;">Documents</a> du site web de Q4OS.
</blockquote>

---

### <span style="color: #F77F00;">13.1. Gestionnaire de mises à jour</span>

Le gestionnaire de mises à jour informe les utilisateurs des mises à jour de sécurité et de logiciels disponibles et leur permet de mettre à niveau le système à la demande.

Vous pouvez facilement installer le gestionnaire de mises à jour depuis le **Centre logiciel Q4OS**.

---

## <span style="color: #06A77D;">14. Dépôts de logiciels externes</span>

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Uniquement pour les utilisateurs avancés :</strong> Ce chapitre est destiné spécifiquement aux utilisateurs avancés familiers avec le système de gestion de paquets Debian.
</blockquote>

La configuration par défaut de Q4OS offre l'ensemble de base et fiable de dépôts de logiciels. Si vous souhaitez ajouter plus de dépôts externes, vous êtes libre de suivre les procédures Debian standard.

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Exemple : Installation du navigateur web Opera**

Listez les dépôts prédéfinis disponibles :

```bash
$ sudo qrepoadd --gui
```

Sélectionnez le dépôt 'opera' dans la zone de liste déroulante et cliquez sur le bouton 'Ok'. Alternativement :

```bash
$ sudo qrepoadd opera
```

Installez les paquets :

```bash
$ sudo apt update
$ sudo apt install opera-stable
```

**Pour désinstaller et désactiver le dépôt :**

```bash
$ sudo apt autoremove opera-stable
$ sudo qreporm opera
$ sudo apt update
```

</div>

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Avertissement :</strong> L'ajout de dépôts tiers externes est une action système de bas niveau et cela pourrait influencer profondément l'intégrité et les dépendances de la base de données de paquets. Heureusement, le système de gestion de paquets Apt contient des outils puissants pour les administrateurs afin de réparer les dépendances cassées.
</blockquote>

---

## <span style="color: #7209B7;">15. Environnements de bureau alternatifs</span>

D'autres environnements de bureau peuvent être intégrés au système Q4OS. Ils peuvent être installés aux côtés du bureau Trinity par défaut, par exemple :
- KDE Plasma
- LXQt
- XFCE
- Et d'autres

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Installation :**

Vous pouvez ajouter un environnement de bureau en utilisant l'outil Desktop Profiler :

```bash
$ swprofiler.exu
```

Cliquez sur le bouton ">" dans le coin supérieur droit pour sélectionner l'environnement de bureau et l'installer avec un profil de bureau.

**Changement de bureau :**

Après le redémarrage, les utilisateurs pourront choisir l'environnement de bureau dans lequel se connecter :

1. Sur l'écran de connexion TDM, cliquez sur le bouton 'Menu'
2. Allez dans 'Type de session'
3. Sélectionnez l'environnement de bureau souhaité

</div>

---

## <span style="color: #F77F00;">16. Ajout de plusieurs langues</span>

Il est possible d'ajouter plusieurs langues dans Q4OS et de définir différents environnements nationaux pour différents utilisateurs.

### <span style="color: #F77F00;">16.1. Ajouter des langues</span>

L'administrateur installe des paquets de localisation séparés et les utilisateurs pourront basculer entre différentes langues.

Lancez l'assistant de nouvelle langue depuis le terminal (répétez pour plusieurs langues) :

```bash
$ addlanguage
```

Si vous avez installé certaines applications ayant des paquets de localisation séparés, installez-les également. **Exemple Libre Office :**

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-xx
```

**Optionnel - changer la locale globale du système et le fuseau horaire :**

```bash
$ sudo dpkg-reconfigure locales
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #F77F00;">16.2. Configuration utilisateur</span>

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Étape 1 :** Choisir et définir une locale (préférer les locales UTF8) :

```bash
$ chqloc --list
$ chqloc --setlocale xx_XX.utf8
```

**Étape 2 :** Sélectionner la nouvelle langue de l'utilisateur

Ouvrez la boîte de dialogue "Pays/Région et Langue" :

```
Panneau de configuration → Régional et Accessibilité → Pays/Région et Langue
```

Choisissez votre pays en cliquant sur le bouton du pays. Cela définira la langue de l'utilisateur ainsi que diverses conventions nationales (format de date/heure, devise, etc.).

**Étape 3 :** Sélectionner une disposition de clavier :

```
Panneau de configuration → Régional et Accessibilité → Disposition du clavier
```

Connectez-vous à nouveau - vous verrez votre profil traduit dans la langue choisie !

</div>

---

### <span style="color: #F77F00;">16.3. Exemple</span>

<div style="background-color: #E3F2FD; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

**Scénario :** Installation fraîche de Q4OS avec la suite Libre Office installée. Nous souhaitons configurer la langue allemande.

**Étape 1 :** Lancez l'assistant de nouvelle langue pour sélectionner l'allemand :

```bash
$ addlanguage
```

**Étape 2 :** Pack linguistique Libre Office :

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-de
```

**Étape 3 :** Définir la locale allemande de l'utilisateur :

```bash
$ chqloc --list
$ chqloc --setlocale de_DE.utf8
```

**Étape 4 :** Ouvrez la boîte de dialogue "Pays/Région et Langue" :

```
Panneau de configuration → Régional et Accessibilité → Pays/Région et Langue
```

Cliquez sur le premier bouton avec le drapeau du pays et choisissez "Europe, Centrale → Allemagne".

**Étape 5 :** Sélectionnez la disposition de clavier allemande :

```
Panneau de configuration → Régional et Accessibilité → Disposition du clavier
```

**Étape 6 :** Connectez-vous à nouveau - votre profil est maintenant en allemand ! 🇩🇪

</div>

---

## <span style="color: #D62828;">17. Divers conseils</span>

### <span style="color: #D62828;">17.1. Menu Démarrer Kickoff</span>

Un menu Démarrer moderne et bien organisé offre une barre de recherche, un onglet favoris, l'historique et plus encore.

Pour passer au menu Kickoff, clic droit sur le panneau système :

```
Configurer le panneau → Menus → Style du menu Démarrer → Kickoff
```

Vous pouvez restaurer le menu Démarrer par défaut de la même manière.

---

### <span style="color: #D62828;">17.2. Icônes à simple clic</span>

L'activation des icônes par double-clic de souris est par défaut dans Q4OS. Il est facile de définir l'activation par simple clic :

```
Panneau de configuration → Périphériques → Souris → Onglet Général → Simple clic pour ouvrir les fichiers et dossiers
```

---

### <span style="color: #D62828;">17.3. Effets de bureau</span>

Activez les effets de lissage et d'embellissement du bureau.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Note :</strong> Les effets de bureau ne fonctionneront parfaitement que sur du matériel moderne. Il n'est pas recommandé de les utiliser avec du matériel ancien.
</blockquote>

Activer les effets de bureau :

```bash
$ ctrl-compmgr --enable
```

Désactiver les effets de bureau :

```bash
$ ctrl-compmgr --disable
```

---

### <span style="color: #D62828;">17.4. Connexion automatique</span>

Il est possible de contourner l'écran de connexion et de connecter automatiquement un utilisateur spécifié après le démarrage du système.

Voir toutes les options possibles :

```bash
$ sudo ctrl-autologin --help
```

Activer la connexion automatique :

```bash
$ sudo ctrl-autologin --enable username
```

---

### <span style="color: #D62828;">17.5. Mise à l'échelle de l'écran</span>

Une installation fraîche de Q4OS devrait détecter automatiquement la résolution de l'écran. Cependant, vous pouvez forcer le système à utiliser un DPI (points par pouce) défini par l'utilisateur :

```
Panneau de configuration → Administration système → Mise à l'échelle de l'écran
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Astuce :</strong> Augmenter la valeur DPI rendra les polices et les icônes plus grandes. Une valeur correcte pour les écrans modernes varie de 120 à 200 DPI selon le type d'écran.
</blockquote>

---

### <span style="color: #D62828;">17.6. Sélection du fuseau horaire</span>

Exécutez la commande dans le terminal pour sélectionner le fuseau horaire du système :

```bash
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #D62828;">17.7. Mot de passe root</span>

Le mot de passe superutilisateur root est désactivé par défaut dans Q4OS. Utilisez "sudo" pour exécuter des commandes en tant que root.

Vous pouvez également activer manuellement et modifier le mot de passe root pour pouvoir utiliser directement le compte root :

```bash
$ sudo passwd
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Configuration et Utilisation</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Manuel utilisateur Trinity desktop, rév. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Site officiel Q4OS</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Documentation</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Forum communautaire</a>
</p>

</div>
