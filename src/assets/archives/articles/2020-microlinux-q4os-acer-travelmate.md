# Archived Article

**Original URL:** https://archives.microlinux.fr/q4os-acer-travelmate/  
**Source:** Microlinux  
**Author:** Kikinovak  
**Date:** 10 Janvier 2020  
**Archived:** February 2025

---

# Refaire une jeunesse à un très vieux PC avec Q4OS

**Author:** Kikinovak  
**Date:** 10 Janvier 2020

---

Dans mon quotidien professionnel, je travaille assez régulièrement avec du matériel déstocké. Les distributions Linux modernes comme OpenSUSE Leap 15.1 tournent très bien sur des machines qui ont cinq voire même parfois dix ans d'âge.

La semaine dernière j'ai récupéré un vieux portable qui pourrait presque faire office de pièce de musée. Un Acer Travelmate 2310 datant de 2005 avec deux autocollants Intel Pentium M et Designed for Windows XP à côté du clavier. En règle générale j'évite ce genre de matériel trop ancien. Mais la machine a l'air très bien conservée, et dans quelques jours je pars grimper avec un ami guide de montagne qui vit chichement et qui n'a pas d'ordinateur. Je me dis que si j'arrive à bricoler quelque chose de viable, ça pourra faire un heureux.

En termes de distributions Linux, exit OpenSUSE, Ubuntu ou Fedora, qui ne démarrent même pas sur ce genre de machine. Quant aux distributions légères et minimalistes, elles manquent souvent de convivialité et d'usabilité, à moins de plonger les mains dans le cambouis et de passer des heures voire des weekends entiers à tout peaufiner. J'ai eu fait ce genre de configuration dans le temps (voir mon livre Débuter avec Linux, entièrement basé sur Slackware Linux et l'environnement Xfce), mais cette fois-ci je recherche quelque chose de plus simple et qui juste marche.

Mon choix se porte sur Q4OS, une distribution allemande (Deutsche Qualität) basée sur la branche stable de Debian. Parmi les moutures diverses et variées de Q4OS, je m'intéresse particulièrement à la version 32-bits basée sur l'environnement de bureau Trinity, une continuation de KDE 3.5.

Sur la page de téléchargement du projet, j'opte pour Q4OS Centaurus Trinity Install CD 32-bit i386. Le fichier q4os-3.10-i386-instcd.r1.iso pèse 434 Mo en tout et pour tout. Je le grave sur un CD, étant donné que mon vieux Acer Travelmate refuse de démarrer sur une clé USB.

Au démarrage, je choisis Q4OS Classic Install.

À partir de là, c'est tout simplement l'installateur de Debian Buster qui s'affiche dans une version légèrement simplifiée, du moins dans un premier temps. Je ne vais pas rentrer dans les détails de l'installation du système de base ici, vu que c'est une série d'opérations triviales comme le partitionnement et le formatage du disque, la création de l'utilisateur initial, etc.

Après le redémarrage initial, le gestionnaire de connexion KDM s'affiche brut de décoffrage.

Une fois que j'ai saisi mon mot de passe, un assistant de configuration (en anglais) me prend par la main et me permet dans un premier temps de peaufiner l'affichage graphique.

L'assistant propose de télécharger automatiquement les localisations françaises des paquets.

Dans le Gestionnaire de profil de bureau, j'opte pour l'environnement de bureau Trinity.

Dans l'écran subséquent du Gestionnaire de profil de bureau, je choisis une installation épurée.

L'assistant récupère les paquets nécessaires sur le réseau.

Au terme de l'installation, je retourne à l'écran de connexion de KDM, qui s'affiche en français et dans un style très sobre et épuré.

L'environnement Trinity affiche le même écran de démarrage que jadis KDE 3.5, et la petite musique au démarrage me ramène quinze ans en arrière.

Trinity est effectivement à KDE 3.5 ce que MATE est à GNOME 2.32. Apparemment, il n'y a que le logo du menu qui a changé.

La distribution Q4OS est livrée avec un écran d'accueil « maison » qui propose de faciliter les opérations les plus courantes.

- Gestionnaire de profil
- Installer des applications
- Codecs propriétaires
- Activer les effets visuels
- Menu démarrer style « KickOff »
- Authentification automatique

Puisqu'on dispose d'un clicodrome bien fait et bien pratique, autant en profiter. Je commence par installer quelques applications pour compléter mon bureau.

Les applications les plus courantes disposent d'un assistant d'installation qui se charge d'intégrer l'application bien proprement à l'environnement de bureau.

C'est très propre et bien fait, et il suffit de faire ses emplettes par une série de clics. Voici les composants que j'installe avec l'assistant pour disposer d'un bureau un peu plus fonctionnel.

- Network Manager
- Update Manager
- VLC
- Codecs multimédia

Je complète avec les paquets suivants, que j'installe à la main.

- firefox-esr
- firefox-esr-l10n-fr
- webext-ublock-origin
- thunderbird
- thunderbird-l10n-fr
- libreoffice
- libreoffice-gtk2
- libreoffice-gtk3
- libreoffice-l10n-fr
- ttf-mscorefonts-installer
- audacious
- gwenview-trinity
- gwenview-i18n-trinity
- aisleriot
- gimp
- inkscape
- ark-trinity

## Conclusion

Q4OS me semble une solution idéale pour refaire une jeunesse à un très vieux PC. L'environnement de bureau Trinity est très peu gourmand en ressources et constitue un compromis réussi entre légèreté et fonctionnalité. Même sur une très vieille machine comme un portable Acer Travelmate 2310 datant de 2005, on peut disposer d'un bureau complet avec des versions modernes de Firefox, Thunderbird, LibreOffice et VLC.

---

**Categories:** Poste de travail  
**Tags:** Debian, KDE, matériel, Q4OS, Trinity
