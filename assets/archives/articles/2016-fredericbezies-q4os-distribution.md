# Archived Article

**Original URL:** https://blog.fredericbezies-ep.fr/2016/11/11/que-devient-la-distribution-gnulinux-q4os/  
**Source:** Frédéric Bézies Blog  
**Author:** Frederic Bezies  
**Date:** vendredi 11 novembre 2016 (mis à jour le samedi 29 février 2020)  
**Categories:** Informatique, Libreries, Trucs de geek  
**Archived:** February 2025

---

# Que devient la distribution GNU/Linux Q4OS ?

**Auteur :** Frederic Bezies  
**Date de publication :** vendredi 11 novembre 2016 (mis à jour le samedi 29 février 2020)  
**Catégories :** Informatique, Libreries, Trucs de geek  
**Étiquettes :** debian, distribution, geekeries, Informatique, libre, Libreries, linux, logiciel, logiciel libre, Q4OS, Trinity Desktop Environment, Trucs de geek

---

Il y a un an et demi, en avril 2015, je parlais de cette distribution basée sur la Debian GNU/Linux Jessie avec le « fork » de KDE 3.5.x, Trinity Desktop Environment. Début novembre 2016, la version 14.0.4 du Trinity Desktop Environment étant sortie, pour prendre en charge par exemple CUPS 2.2, gstreamer 1.x ou encore gcc 6.x et ffmpeg3, l'équipe de Q4OS en a profité pour proposer des nouvelles images ISO live et d'installation.

Petite parenthèse en passant : cet article aurait très bien pu faire partie de la série « Les projets un peu fous du logiciel libre », ne serait-ce que pour l'utilisation de Trinity Desktop Environment. Mais passons 😀

J'ai donc récupéré l'énorme image ISO d'installation… Un peu moins de 300 Mo…

```
[fred@fredo-arch ISO à tester]$ wget -c http://netix.dl.sourceforge.net/project/q4os/stable/q4os-1.8.1-x64.iso
–2016-11-11 13:24:07– http://netix.dl.sourceforge.net/project/q4os/stable/q4os-1.8.1-x64.iso
Résolution de netix.dl.sourceforge.net (netix.dl.sourceforge.net)… 87.121.121.2
Connexion à netix.dl.sourceforge.net (netix.dl.sourceforge.net)|87.121.121.2|:80… connecté.
requête HTTP transmise, en attente de la réponse… 200 OK
Taille : 294649856 (281M) [application/octet-stream]
Sauvegarde en : « q4os-1.8.1-x64.iso »

q4os-1.8.1-x64.iso 100%[===================>] 281,00M 981KB/s in 5m 20s

2016-11-11 13:29:28 (898 KB/s) — « q4os-1.8.1-x64.iso » sauvegardé [294649856/294649856]
```

Mon ami VirtualBox a été mis à contribution, avec les caractéristiques habituelles : 2 Go de mémoire vive, 128 Go de disque virtuels, et 2 CPUs.

Comme pour l'article précédent, l'installateur est en mode texte, que l'on peut passer dans la langue de Molière. La version live propose un installateur, mais je ne suis pas fan de ce dernier.

Après l'installation qui est assez rapide, l'OS propose à la première connexion de récupérer les paquets linguistiques.

Et d'installer les additions VirtualBox si nécessaire. C'est ce que j'apprécie dans cette distribution. Elle est bien conçue, et c'est incroyable ce que c'est plaisant !

Une fois déconnecté et reconnecté, j'ai choisi l'outil « gestionnaire de profils » pour installer la totale. En gros, cela entraine la récupération d'environ 520 Mo. Il faut compter à peu près 20 minutes pour que l'ensemble des logiciels soient récupérés et installés.

J'ai aussi apprécié l'outil d'ajout des codecs non libres, même si cela hérissera le poil d'une partie du monde du logiciel libre.

Ensuite, SimpleScreenRecorder a pris le relai pour capturer l'ensemble en vidéo.

La distribution est très agréable d'emploi. Trinity est un vrai bonheur à utiliser. Dommage cependant que par défaut, Google Chrome soit proposé. Les traductions presque complète, l'outil d'ajout facile de logiciels. Seul point noir ? Le menu déroulant de Trinity choisi par Q4OS n'est pas celui que j'aurai sélectionné, mais cela ce change un clic de souris.

Je concluais mon précédent article ainsi :

> C'est une distribution dont la légereté la fait rentrer en concurrence frontale avec des projets comme la antiX MX voire la HandyLinux pour la catégorie grands débutants sous Linux.
>
> Ce qui pourrait la desservir, c'est son côté vieillot, car KDE 3.5.x, ça commence à dater.

La conclusion serait la même, ou presque. Il est vrai qu'il est intéressant de voir des outils comme LibreOffice 5.x dans une interface qui a été celle de KDE entre 2002 et 2008. Mais si vous cherchez une distribution légère, rapide et conçue comme telle, elle restera toujours un choix à envisager. Avec DFLinux our encore la MX-16.
