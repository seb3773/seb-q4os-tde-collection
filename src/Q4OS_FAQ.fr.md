<div align="center">

# 🖥️ <span style="color: #2E86AB;">Q4OS Foire Aux Questions</span>

### <span style="color: #6C757D;">Manuel Utilisateur Trinity Desktop</span>
*<span style="color: #A23B72;">Révision 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Source du document : <a href="https://www.q4os.org/dqa011.html" style="color: #2E86AB;">https://www.q4os.org/dqa011.html</a>
</p>

### 🌐 Lire dans votre langue :
[🇬🇧 English](Q4OS_FAQ.md) | [🇫🇷 Français](Q4OS_FAQ.fr.md) | [🇩🇪 Deutsch](Q4OS_FAQ.de.md) | [🇪🇸 Español](Q4OS_FAQ.es.md)

</div>

---

## 📑 <span style="color: #2E86AB;">Table des matières</span>

### <span style="color: #F77F00;">1. [Introduction](#1-introduction)</span>

### <span style="color: #06A77D;">2. [Installation](#2-installation)</span>
- 2.1. [Comment créer un disque USB d'installation Q4OS bootable ?](#21-comment-créer-un-disque-usb-dinstallation-q4os-bootable)
- 2.2. [Existe-t-il un moyen de dual-booter Q4OS avec Windows ?](#22-existe-t-il-un-moyen-de-dual-booter-q4os-avec-windows)
- 2.3. [Je n'ai pas de son après l'installation, que dois-je faire ?](#23-je-nai-pas-de-son-après-linstallation-que-dois-je-faire)
- 2.4. [Impossible de se connecter au réseau sans fil, que faire ?](#24-impossible-de-se-connecter-au-réseau-sans-fil-que-faire)

### <span style="color: #D62828;">3. [Système](#3-système)</span>
- 3.1. [Il y a des dépendances de paquets cassées dans mon système. Comment les réparer ?](#31-il-y-a-des-dépendances-de-paquets-cassées-dans-mon-système-comment-les-réparer)
- 3.2. [Certaines lettres sont mal saisies ('L' s'affiche comme '3', 'J' comme '1')](#32-certaines-lettres-sont-mal-saisies-l-saffiche-comme-3-j-comme-1)
- 3.3. [Les polices et icônes sont trop petites sur mon écran hiDPI, puis-je les agrandir ?](#33-les-polices-et-icônes-sont-trop-petites-sur-mon-écran-hidpi-puis-je-les-agrandir)
- 3.4. [Comment afficher la température actuelle du CPU dans le panneau système ?](#34-comment-afficher-la-température-actuelle-du-cpu-dans-le-panneau-système)
- 3.5. [Je suis derrière un proxy, les applications basées sur le gestionnaire de paquets ne fonctionnent pas](#35-je-suis-derrière-un-proxy-les-applications-basées-sur-le-gestionnaire-de-paquets-ne-fonctionnent-pas)
- 3.6. [Je veux utiliser un noyau Linux récent, est-ce possible ?](#36-je-veux-utiliser-un-noyau-linux-récent-est-ce-possible)

### <span style="color: #7209B7;">4. [Bureau](#4-bureau)</span>
- 4.1. [Comment configurer plusieurs bureaux virtuels dans Q4OS ?](#41-comment-configurer-plusieurs-bureaux-virtuels-dans-q4os)
- 4.2. [Je ne peux pas renommer ou modifier certaines icônes sur mon Bureau](#42-je-ne-peux-pas-renommer-ou-modifier-certaines-icônes-sur-mon-bureau)
- 4.3. [Comment puis-je éditer le menu Démarrer ?](#43-comment-puis-je-éditer-le-menu-démarrer)
- 4.4. [Puis-je personnaliser l'affichage et les raccourcis du panneau droit du menu Démarrer 'Bourbon' par défaut de Q4OS ?](#44-puis-je-personnaliser-laffichage-et-les-raccourcis-du-panneau-droit-du-menu-démarrer-bourbon-par-défaut-de-q4os)
- 4.5. [Je veux que l'entrée de l'écran de bienvenue soit affichée dans le menu Démarrer](#45-je-veux-que-lentrée-de-lécran-de-bienvenue-soit-affichée-dans-le-menu-démarrer)
- 4.6. [Comment puis-je démarrer automatiquement une application ?](#46-comment-puis-je-démarrer-automatiquement-une-application)
- 4.7. [J'ai compromis mon bureau, comment puis-je restaurer les couleurs, polices, thème et autres paramètres par défaut ?](#47-jai-compromis-mon-bureau-comment-puis-je-restaurer-les-couleurs-polices-thème-et-autres-paramètres-par-défaut)
- 4.8. [Comment puis-je définir des icônes à simple clic au lieu de double-clic ?](#48-comment-puis-je-définir-des-icônes-à-simple-clic-au-lieu-de-double-clic)
- 4.9. [Dites-moi le moyen le plus simple de faire une capture d'écran](#49-dites-moi-le-moyen-le-plus-simple-de-faire-une-capture-décran)
- 4.10. [Est-il possible de changer de thème d'icônes ?](#410-est-il-possible-de-changer-de-thème-dicônes)
- 4.11. [J'ai défini des raccourcis clavier dans le Panneau de configuration, mais ils ne fonctionnent pas](#411-jai-défini-des-raccourcis-clavier-dans-le-panneau-de-configuration-mais-ils-ne-fonctionnent-pas)
- 4.12. [J'ai remarqué que l'entrée 'Programmes' a disparu du menu Démarrer](#412-jai-remarqué-que-lentrée-programmes-a-disparu-du-menu-démarrer)
- 4.13. [Le raccourci clavier ne fonctionne pas pour basculer entre les dispositions de clavier non-latines](#413-le-raccourci-clavier-ne-fonctionne-pas-pour-basculer-entre-les-dispositions-de-clavier-non-latines)
- 4.14. [J'ai besoin d'ajuster la luminosité de l'écran](#414-jai-besoin-dajuster-la-luminosité-de-lécran)

### <span style="color: #F77F00;">5. [Applications](#5-applications)</span>
- 5.1. [Comment puis-je configurer la transparence de 'Conky' ?](#51-comment-puis-je-configurer-la-transparence-de-conky)

---

## <span style="color: #F77F00;">1. Introduction</span>

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
📢 Signalez-nous toutes les erreurs que vous trouvez, vos suggestions sont les bienvenues. Si possible, envoyez-nous ce qui vous semblerait être une solution plus claire. Vous pouvez vous référer en toute sécurité à la <a href="http://www.trinitydesktop.org/faq/index.php" style="color: #2E86AB;">FAQ de l'environnement de bureau Trinity</a>.
</blockquote>

---

## <span style="color: #06A77D;">2. Installation</span>

### <span style="color: #06A77D;">2.1. Comment créer un disque USB d'installation Q4OS bootable ?</span>

Le moyen le plus simple sous Linux est de brancher votre clé USB, ne pas la monter, et exécuter dans le terminal :

```bash
$ sudo cp bootable.iso /dev/sdx
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Note :</strong><br>
• <code>sdx</code> est le lecteur USB cible, par exemple <code>sdb</code><br>
• <code>bootable.iso</code> est l'image CD d'installation Q4OS bootable, vous pouvez la télécharger depuis le site web de Q4OS
</blockquote>

Alternativement, vous pouvez utiliser les logiciels multiplateformes **UNetbootin** ou **Rufus** pour créer des disques USB bootables. Voir [comment créer un média live](https://www.q4os.org/dqa018.html#creat).

---

### <span style="color: #06A77D;">2.2. Existe-t-il un moyen de dual-booter Q4OS avec Windows ?</span>

Bien sûr ! La méthode préférée est de procéder à l'installation depuis un CD 'Live', car cela vous donne l'option d'installer le chargeur de démarrage. Si vous laissez l'installateur installer le chargeur de démarrage Grub, il détectera automatiquement les systèmes d'exploitation disponibles y compris Windows et les proposera tous à chaque démarrage.

Si vous voulez garder le chargeur de démarrage Windows, n'oubliez pas de décocher la case correspondante pendant l'installation.

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Important :</strong> Nous recommandons vivement de sauvegarder toutes vos données avant. Veuillez lire les <a href="https://www.q4os.org/dqa018.html" style="color: #D62828;">instructions d'installation</a>.
</blockquote>

---

### <span style="color: #06A77D;">2.3. Je n'ai pas de son après l'installation, que dois-je faire ?</span>

Nous vous recommandons d'abord d'installer le serveur sonore Pipewire :

```bash
$ sudo apt install pipewire pavucontrol-qt
```

Redémarrez votre ordinateur. Ensuite, suivez ces étapes :

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Étapes de configuration :**

1. Clic droit sur l'icône 'mixeur' dans la zone système → 'Sélectionner le canal maître...'
2. Définir 'Mixeur actuel' sur 'PipeWire' dans la liste déroulante en haut à droite
3. Cliquer sur 'Ok' pour fermer la boîte de dialogue
4. Lancer l'application 'Contrôle du volume' depuis le menu Démarrer
5. Configurer les paramètres du mixeur de sortie dans l'onglet 'Périphériques de sortie'
6. Vérifier que les canaux de sortie ne sont pas muets

</div>

Le système audio devrait fonctionner maintenant. Sinon, continuez à suivre les étapes ci-dessous.

**Diagnostic supplémentaire :**

Clic gauche sur l'icône 'mixeur' dans la zone système, et cliquez sur le bouton 'Mixeur' pour vérifier et mettre à jour les niveaux du mixeur audio. Assurez-vous que la carte son 'PipeWire' est sélectionnée dans le coin supérieur droit de la fenêtre du mixeur 'kmix'.

Ensuite, exécutez la commande dans le terminal et vérifiez la sortie de débogage :

```bash
$ artsplay /opt/trinity/share/sounds/KDE_Startup.wav
```

S'il n'y a toujours pas de son, termpez temporairement le serveur sonore Trinity et essayez de lire l'audio avec un lecteur alsa indépendant :

```bash
$ artsshell terminate
$ aplay /opt/trinity/share/sounds/KDE_Startup.wav
```

Encore une fois, vérifiez la sortie de débogage. Si votre système audio ne fonctionne toujours pas, continuez à suivre le [Dépannage des problèmes de son](http://www.trinitydesktop.org/faq/sound.php) dans la FAQ Trinity.

---

### <span style="color: #06A77D;">2.4. Impossible de se connecter au réseau sans fil, que faire ?</span>

Q4OS prend entièrement en charge les réseaux sans fil et inclut un outil appelé **tdenetworkmanager** pour gérer les connexions sans fil. Vous pouvez le trouver dans la zone système.

Si vous rencontrez des problèmes de connexion à un réseau sans fil, veuillez lire le [message de dépannage wifi](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #D62828;">3. Système</span>

### <span style="color: #D62828;">3.1. Il y a des dépendances de paquets cassées dans mon système. Comment les réparer ?</span>

Nous avons un outil pratique pour réparer automatiquement les dépendances cassées dans Q4OS, il suffit d'exécuter dans le terminal :

```bash
$ sudo sh /usr/share/apps/q4os_system/bin/qapt_fix.sh
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Rappel :</strong> Nous recommandons vivement d'installer des logiciels provenant uniquement de sources fiables et compatibles avec Debian pour empêcher le système de paquets d'être corrompu.
</blockquote>

---

### <span style="color: #D62828;">3.2. Certaines lettres sont mal saisies ('L' s'affiche comme '3', 'J' comme '1')</span>

Un problème courant qui se produit sur les netbooks avec un petit clavier. Le clavier est bloqué par NumLock, vous pourriez essayer de désactiver NumLock.

Lancez le Panneau de configuration :

```
Panneau de configuration → Périphériques → Clavier → NumLock au démarrage de KDE → définir sur Désactivé
```

Connectez-vous à nouveau et essayez le clavier.

---

### <span style="color: #D62828;">3.3. Les polices et icônes sont trop petites sur mon écran hiDPI, puis-je les agrandir ?</span>

Oui, Q4OS peut mettre à l'échelle la résolution de l'écran. Veuillez lire le chapitre [résolution d'écran](https://www.q4os.org/dqa007.html#tips.6).

---

### <span style="color: #D62828;">3.4. Comment afficher la température actuelle du CPU dans le panneau système ?</span>

Lancez l'application **ksensors** depuis :

```
Menu Démarrer → Programmes → Accessoires → Système → KSensors
```

Si **ksensors** n'est pas encore installé, suivez le chapitre [capteurs matériels](https://www.q4os.org/dqa007.html#hwsens) pour l'installer.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0; border-left: 5px solid #7209B7;">

**Configuration :**

1. Clic droit sur l'icône 'ksensors' dans la zone système → Configurer
2. Sélectionner le groupe de capteurs matériels concerné
3. Sélectionner le capteur désiré dans la liste
4. Onglet Dock → cocher la case 'Visible'

Vous pouvez éventuellement définir les couleurs, alarmes, seuils, actions sur le dépassement des limites et autres options. Cliquez sur le bouton 'Appliquer' et fermez la boîte de dialogue.

</div>

---

### <span style="color: #D62828;">3.5. Je suis derrière un proxy, les applications basées sur le gestionnaire de paquets ne fonctionnent pas</span>

Vous devez définir des variables d'environnement à l'échelle du système. Ouvrez le fichier `/etc/environment` avec votre éditeur préféré et ajoutez les lignes suivantes (en modifiant appropriément) :

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
📝 <strong>Note :</strong> Vous devez dupliquer en majuscules et minuscules car certains programmes recherchent uniquement l'un ou l'autre.
</blockquote>

Le système de gestion de paquets APT n'obéira pas aux variables d'environnement lorsqu'il est utilisé normalement avec sudo. Donc configurez-les séparément ; créez un fichier appelé `95proxies` dans `/etc/apt/apt.conf.d/`, et incluez ce qui suit :

```bash
Acquire::http::proxy "http://myproxy.server.com:8080/";
Acquire::ftp::proxy "ftp://myproxy.server.com:8080/";
Acquire::https::proxy "https://myproxy.server.com:8080/";
```

Enfin, redémarrez pour vous assurer que les changements prennent effet.

---

### <span style="color: #D62828;">3.6. Je veux utiliser un noyau Linux récent, est-ce possible ?</span>

Nous recommandons d'utiliser le noyau Q4OS/Debian par défaut, fiable et profondément éprouvé. Il n'y a pas trop de raisons pour les utilisateurs ordinaires d'utiliser un noyau plus récent.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Avertissement :</strong> Les derniers noyaux ne sont pas aussi sécurisés que le noyau Debian par défaut, stable comme un roc et testé de manière exhaustive, cependant ils pourraient apporter des améliorations et de nouveaux pilotes de périphériques et support.
</blockquote>

Si vous préférez pour certaines raisons le dernier noyau Linux, exécutez le script d'auto-installation dans le terminal pour l'installer facilement depuis le dépôt backports :

```bash
$ qinst-kernel-bpo
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Bon à savoir :</strong> L'ancien bon noyau par défaut ne sera pas désinstallé, donc vous pouvez à tout moment le choisir et le démarrer depuis le menu de démarrage grub, si vous rencontrez des problèmes.
</blockquote>

---

## <span style="color: #7209B7;">4. Bureau</span>

### <span style="color: #7209B7;">4.1. Comment configurer plusieurs bureaux virtuels dans Q4OS ?</span>

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Étape 1 :** Lancez le Panneau de configuration et allez à :

```
Bureau → Bureaux multiples
```

Sélectionnez combien de bureaux virtuels vous souhaitez avoir.

**Étape 2a :** Ajoutez un applet de changement de bureau à votre barre des tâches :

1. Clic droit sur la barre des tâches
2. Sélectionner 'Ajouter un applet au panneau' (si la barre des tâches est verrouillée, déverrouillez-la d'abord)
3. Dans la fenêtre contextuelle, sélectionner 'Pager / Commutateur de bureau'
4. Cliquer sur 'Ajouter au panneau'

**Étape 3a :** Configurez un raccourci clavier :

1. Lancez le Panneau de configuration
2. Allez à : `Régional et Accessibilité → Raccourcis clavier`
3. Sous l'onglet 'Raccourcis globaux', faites défiler vers le bas et trouvez 'Aller au bureau suivant' sous 'Changement de bureau'
4. Cliquez sur le bouton à côté de l'option 'Personnalisé'
5. Assignez la combinaison de touches que vous souhaitez utiliser
6. Cliquez sur 'OK' pour sauvegarder

</div>

---

### <span style="color: #7209B7;">4.2. Je ne peux pas renommer ou modifier certaines icônes sur mon Bureau</span>

Il pourrait y avoir trois types logiques d'icônes présents sur votre bureau :

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 10px 0;">

**1. Icônes Système** 🔒
- 'Mon Ordinateur', 'Mes Documents', 'Mes Lieux Réseau', 'Corbeille', 'Navigateur Web', 'Imprimantes'
- Appartiennent à root
- Non modifiables directement par un utilisateur
- Peuvent être supprimées du bureau

**2. Icônes Globales** 🌐
- Généralement créées par les installateurs d'applications
- Appartiennent à root et partagées par tous les utilisateurs
- Les utilisateurs peuvent les masquer mais pas les éditer ou les renommer

**3. Icônes Utilisateur** 👤
- Créées par un seul utilisateur
- Contrôle total : supprimer, renommer, éditer les propriétés (clic droit → Propriétés)

</div>

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Astuce :</strong> Si vous voulez éditer une icône globale ou système, nous recommandons de la supprimer du bureau et de créer une icône utilisateur correspondante en utilisant Glisser-déposer → Copier depuis le menu Démarrer. Elle appartiendra à l'utilisateur et sera entièrement modifiable.
</blockquote>

---

### <span style="color: #7209B7;">4.3. Comment puis-je éditer le menu Démarrer ?</span>

1. Ouvrez le menu Démarrer
2. Clic droit sur n'importe quel élément sous l'entrée 'Programmes'
3. Sélectionner 'Editer le menu'
4. La fenêtre de l'éditeur de menu apparaît

Vous pourrez créer une nouvelle structure personnalisée de sous-menus/dossiers et la remplir avec les éléments de menu souhaités. Vous pouvez créer de nouveaux raccourcis en utilisant le clic droit, ou glisser-déposer des icônes depuis le menu Démarrer ou le Bureau dans la fenêtre de l'éditeur de menu.

Les éléments nouvellement créés apparaîtront dans le menu Démarrer après la fermeture de la fenêtre de l'éditeur de menu.

**Bonus :** Vous pouvez également basculer l'organisation des éléments du menu Démarrer par Catégories ou par Applications :

```bash
$ sh /usr/share/apps/q4os_system/bin/kmenu_struct.sh --help
```

---

### <span style="color: #7209B7;">4.4. Puis-je personnaliser l'affichage et les raccourcis du panneau droit du menu Démarrer 'Bourbon' par défaut de Q4OS ?</span>

Oui ! Éditez le fichier `$HOME/.trinity/share/config/kickerrc` dans votre répertoire personnel.

Il y a plusieurs options de configuration commençant par 'Bourbon' commentées par défaut. Vous devez :

1. Décommenter la ligne `BourbonSysViewCustomItems`
2. Spécifier les liens `.desktop` que vous souhaitez afficher sur le panneau de menu droit
3. Utiliser une virgule `,` comme délimiteur

**Options supplémentaires :**

- Masquer les raccourcis par défaut :
  - `BourbonShowSysViewFolders=false`
  - `BourbonShowSysViewApps=false`

---

### <span style="color: #7209B7;">4.5. Je veux que l'entrée de l'écran de bienvenue soit affichée dans le menu Démarrer</span>

Exécutez la commande pour mettre à jour le raccourci de l'écran de bienvenue dans le terminal :

```bash
$ sudo kwriteconfig --file '/usr/share/applications/q4os-welcome-screen.desktop' --group 'Desktop Entry' --key 'NoDisplay' 'false'
```

Alternativement, vous pouvez éditer manuellement le fichier `/usr/share/applications/q4os-welcome-screen.desktop`.

L'icône de l'écran de bienvenue apparaîtra sous :

```
Menu Démarrer → Programmes → Accessoires → Système
```

---

### <span style="color: #7209B7;">4.6. Comment puis-je démarrer automatiquement une application ?</span>

Vous devez ajouter un raccourci d'application (fichier `.desktop`) dans le dossier de démarrage automatique :

- `$HOME/.trinity/Autostart`
- ou `$HOME/.q4data/Programs/Startup`

L'application sera lancée immédiatement après la connexion de l'utilisateur.

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Méthodes :**

1. Faites glisser n'importe quel raccourci d'application depuis le menu Démarrer ou le Bureau et déposez-le dans le dossier de démarrage automatique
2. Il est également possible de placer un script shell ou un exécutable dans le dossier de démarrage automatique

</div>

---

### <span style="color: #7209B7;">4.7. J'ai compromis mon bureau, comment puis-je restaurer les couleurs, polices, thème et autres paramètres par défaut ?</span>

Simplement exécuter dans le terminal :

```bash
$ sh /usr/share/apps/q4os_system/bin/default_desktop_settings.sh
```

---

### <span style="color: #7209B7;">4.8. Comment puis-je définir des icônes à simple clic au lieu de double-clic ?</span>

L'activation des icônes par double-clic de souris est par défaut dans Q4OS. Il est facile de définir l'activation par simple clic, l'effet de survol et plus encore dans le Panneau de configuration :

```
Panneau de configuration → Périphériques → Souris → Onglet Général → Simple clic pour ouvrir les fichiers et dossiers
```

---

### <span style="color: #7209B7;">4.9. Dites-moi le moyen le plus simple de faire une capture d'écran</span>

Vous pouvez faire cela sans aucun paquet supplémentaire :

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Méthode rapide :**

1. Appuyez sur la touche `PrtScr`
2. Clic droit sur le bureau
3. Sélectionner 'Coller le contenu du presse-papiers'
4. Une boîte de dialogue apparaît où vous pouvez entrer le nom de fichier et le type d'image
5. Le fichier sera sauvegardé sur le bureau

Vous pouvez également ouvrir Konqueror pour naviguer vers le dossier préféré, clic droit et sélectionner 'Coller le contenu du presse-papiers' pour sauvegarder le fichier à l'emplacement préféré.

</div>

**Application dédiée :**

Il existe une application légère et puissante **ksnapshot-trinity**, capable de capturer l'écran entier, une région, une fenêtre ou une partie de fenêtre uniquement.

Installation :

```bash
$ sudo apt install ksnapshot-trinity
```

---

### <span style="color: #7209B7;">4.10. Est-il possible de changer de thème d'icônes ?</span>

Oui ! Vous devez déverrouiller les options avancées du Panneau de configuration dans le terminal :

```bash
$ sudo kcmodules --unlock
```

Ensuite allez à :

```
Panneau de configuration → Apparence & Thèmes → Icônes
```

Configurez le thème que vous préférez.

---

### <span style="color: #7209B7;">4.11. J'ai défini des raccourcis clavier dans le Panneau de configuration, mais ils ne fonctionnent pas</span>

Vous devez seulement activer le service khotkeys pour qu'il soit exécuté lors de la connexion à la session.

Allez au Panneau de configuration :

```
Panneau de configuration → Régional et Accessibilité → Actions d'entrée → Onglet Paramètres Généraux → décocher la case Désactiver KHotKeys
```

---

### <span style="color: #7209B7;">4.12. J'ai remarqué que l'entrée 'Programmes' a disparu du menu Démarrer</span>

Cela arrive rarement sur certains systèmes spécifiquement configurés. La solution de contournement qui devrait corriger cela est de rebasculer depuis le menu classique - kicker - classique.

Vous pourriez le signaler comme un nouveau bogue dans notre [Bug tracker](https://sourceforge.net/p/q4os/tickets), et ajouter une description si vous trouvez des connexions.

---

### <span style="color: #7209B7;">4.13. Le raccourci clavier ne fonctionne pas pour basculer entre les dispositions de clavier non-latines</span>

Le raccourci de basculement de clavier par défaut est `Alt+Espace` ou `Ctrl+Alt+K`. Cela fonctionne sans problème si vous avez uniquement installé des dispositions de clavier latines.

Pour pouvoir basculer librement entre les claviers non-latins, vous devez ajouter une 'disposition latine' à chaque disposition de clavier que vous utilisez.

Exécutez le Panneau de configuration :

```
Panneau de configuration → Régional et Accessibilité → Disposition du clavier → sélectionner une disposition de clavier non-latine → cocher la case 'Inclure la disposition latine'
```

---

### <span style="color: #7209B7;">4.14. J'ai besoin d'ajuster la luminosité de l'écran</span>

Survolez simplement avec votre souris l'icône **tdepowersave** dans la zone système, et utilisez la molette de la souris pour ajuster la luminosité vers le haut ou le bas.

Si l'icône n'est pas disponible dans la zone système, vous devez installer le paquet `tdepowersave-trinity` et vous connecter à nouveau à la session de bureau Trinity.

**Alternative :**

Vous pouvez installer le paquet `klcddimmer-trinity` et ajouter un applet dans le panneau système. Cependant, vous devrez le configurer pour utiliser un backend de contrôle de luminosité, par exemple `xbacklight`.

---

## <span style="color: #F77F00;">5. Applications</span>

### <span style="color: #F77F00;">5.1. Comment puis-je configurer la transparence de 'Conky' ?</span>

Vous devez avoir les effets de bureau Q4OS/Trinity activés. Cela peut être configuré via l'écran de bienvenue ou le Panneau de configuration.

Éditez le fichier `/etc/conky/conky.conf` et ajoutez les lignes :

```bash
own_window yes
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
own_window_argb_visual
own_window_argb_value 0
```

Commentez la ligne :

```bash
#own_window_type desktop
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Foire aux Questions</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Manuel utilisateur Trinity desktop, rév. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Site officiel Q4OS</a> | 
🐛 <a href="https://sourceforge.net/p/q4os/tickets" style="color: #FFD700; text-decoration: none;">Bug Tracker</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Forum</a>
</p>

</div>
