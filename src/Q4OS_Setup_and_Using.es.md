<div align="center">

# ⚙️ <span style="color: #2E86AB;">Q4OS Configuración y Uso</span>

### <span style="color: #6C757D;">Manual de Usuario de Trinity Desktop</span>
*<span style="color: #A23B72;">Revisión 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Fuente del documento: <a href="https://www.q4os.org/dqa007.html" style="color: #2E86AB;">https://www.q4os.org/dqa007.html</a>
</p>

### 🌐 Leer en su idioma:
[🇬🇧 English](Q4OS_Setup_and_Using.md) | [🇫🇷 Français](Q4OS_Setup_and_Using.fr.md) | [🇩🇪 Deutsch](Q4OS_Setup_and_Using.de.md) | [🇪🇸 Español](Q4OS_Setup_and_Using.es.md)

</div>

---

## 📑 <span style="color: #2E86AB;">Tabla de Contenidos</span>

1. [Introducción](#1-introducción)
2. [Prueba](#2-prueba)
   - 2.1. [Live CD](#21-live-cd)
   - 2.2. [En Virtualbox](#22-en-virtualbox)
3. [Instalación](#3-instalación)
4. [Configuración de red inalámbrica](#4-configuración-de-red-inalámbrica)
5. [Imprimir y escanear](#5-imprimir-y-escanear)
   - 5.1. [Impresoras y escáneres Hewlett-Packard](#51-impresoras-y-escáneres-hewlett-packard)
   - 5.2. [Otras impresoras](#52-otras-impresoras)
   - 5.3. [Escáneres](#53-escáneres)
6. [Gestión de energía](#6-gestión-de-energía)
7. [Sensores de hardware](#7-sensores-de-hardware)
8. [Dispositivo táctil](#8-dispositivo-táctil)
9. [Códecs multimedia propietarios](#9-codecs-multimedia-propietarios)
10. [Controladores de video propietarios](#10-controladores-de-video-propietarios)
11. [Usuarios y grupos](#11-usuarios-y-grupos)
    - 11.1. [Agregar un usuario regular](#111-agregar-un-usuario-regular)
12. [Interconexión Android](#12-interconexión-android)
13. [Actualizaciones de seguridad, gestión de software](#13-actualizaciones-de-seguridad-gestión-de-software)
    - 13.1. [Administrador de actualizaciones](#131-administrador-de-actualizaciones)
14. [Repositorios de software externos](#14-repositorios-de-software-externos)
15. [Entornos de escritorio alternativos](#15-entornos-de-escritorio-alternativos)
16. [Agregar más idiomas](#16-agregar-más-idiomas)
    - 16.1. [Agregar idiomas](#161-agregar-idiomas)
    - 16.2. [Configuración de usuario](#162-configuración-de-usuario)
    - 16.3. [Ejemplo](#163-ejemplo)
17. [Varios consejos](#17-varios-consejos)
    - 17.1. [Menú Inicio Kickoff](#171-menú-inicio-kickoff)
    - 17.2. [Iconos de un solo clic](#172-iconos-de-un-solo-clic)
    - 17.3. [Efectos de escritorio](#173-efectos-de-escritorio)
    - 17.4. [Inicio de sesión automático](#174-inicio-de-sesión-automático)
    - 17.5. [Escalado de pantalla](#175-escalado-de-pantalla)
    - 17.6. [Selección de zona horaria](#176-selección-de-zona-horaria)
    - 17.7. [Contraseña root](#177-contraseña-root)

---

## <span style="color: #F77F00;">1. Introducción</span>

<div style="background-color: #F0F8FF; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

Este documento cubre cómo configurar, establecer y usar el sistema operativo Q4OS.

Q4OS se recomienda para usar en máquinas de producción, ya que ha sido construido sobre el sistema Debian extremadamente estable, seguro y confiable, probado por muchas personas en todo el mundo.

Existe una enorme base de software estable en los repositorios predeterminados - usted es libre de usarla y ajustar el sistema según sus necesidades.

</div>

---

## <span style="color: #06A77D;">2. Prueba</span>

### <span style="color: #06A77D;">2.1. Live CD</span>

Si desea obtener una experiencia rápida de Q4OS o probarlo en hardware real, puede arrancar con seguridad un CD o USB live de Q4OS.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Prueba segura:</strong> No escribirá nada en su disco duro y no afectará su instalación existente. Es posible instalar el sistema Q4OS directamente desde el medio live usando el instalador live.
</blockquote>

---

### <span style="color: #06A77D;">2.2. En Virtualbox</span>

Recomendamos instalar Q4OS dentro de [Virtualbox](http://www.virtualbox.org/) para fines de prueba.

**Configuración:**
- Sistema operativo: **Linux**
- Versión: **Debian (32/64 bits)**

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Consejo:</strong> Es apropiado instalar las "Virtualbox guest additions" dentro del sistema invitado para lograr el mejor rendimiento. Hay un autoinstalador conveniente disponible en el 'Centro de software' Q4OS. El instalador contiene controladores optimizados y es preferible instalarlo desde fuentes originales de Oracle u otras.
</blockquote>

---

## <span style="color: #D62828;">3. Instalación</span>

Por favor lea la [guía de instalación](https://www.q4os.org/dqa018.html) de Q4OS nueva.

---

## <span style="color: #7209B7;">4. Configuración de red inalámbrica</span>

Q4OS admite completamente las redes inalámbricas e incluye una herramienta llamada **tdenetworkmanager** para gestionar conexiones inalámbricas. Puede encontrarla en la bandeja del sistema.

Si tiene problemas para conectarse a una red inalámbrica, por favor lea la [publicación de solución de problemas wifi](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #F77F00;">5. Imprimir y escanear</span>

### <span style="color: #F77F00;">5.1. Impresoras y escáneres Hewlett-Packard</span>

Instale el sistema de impresión e imágenes HP Linux, satisfaga las dependencias y configure una impresora en la terminal:

```bash
$ sudo apt install hplip hplip-gui avahi-utils cups
$ sudo apt install libcupsimage2-dev libdbus-1-dev libssl-dev libusb-1.0.0-dev python-dev
$ sudo hp-setup
```

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Nota:</strong> Algunas impresoras HP requieren un controlador descargable. El comando 'hp-setup' descargará e instalará el controlador automáticamente.
</blockquote>

---

### <span style="color: #F77F00;">5.2. Otras impresoras</span>

Primero liste los controladores y elija el adecuado para su modelo:

```bash
$ apt-cache search printer-driver
```

Instale un conjunto específico de controladores, por ejemplo para impresoras láser Samsung:

```bash
$ sudo apt install printer-driver-splix cups
```

O puede instalar todos los controladores de impresora disponibles:

```bash
$ sudo apt install foomatic-db printer-driver-all cups
```

Luego agregue y configure las impresoras:

```
Menú Inicio → Aplicaciones → Configuración → Sistema de impresión
```

Puede encontrar información adicional valiosa en la [wiki de Debian](https://wiki.debian.org/SystemPrinting).

---

### <span style="color: #F77F00;">5.3. Escáneres</span>

Recomendamos usar la aplicación **Kooka** para escanear. Instale el software requerido y agregue cualquier usuario que necesite acceso al grupo 'scanner':

```bash
$ sudo apt install libsane sane sane-utils xsane kooka-trinity
$ sudo adduser su_nombre_de_usuario scanner
```

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Importante:</strong> Un usuario necesitará cerrar sesión y volver a iniciar para que el nuevo grupo surta efecto.
</blockquote>

Verifique que el escáner ahora sea reconocido:

```bash
$ scanimage -L
$ sane-find-scanner
```

Si desea configurar un escaneo de red, consulte [Sane en red](https://wiki.debian.org/SaneOverNetwork).

---

## <span style="color: #06A77D;">6. Gestión de energía</span>

Es deseable instalar una aplicación de control de energía para portátiles y dispositivos móviles:

```bash
$ sudo apt update
$ sudo apt install rfkill tdepowersave-trinity
```

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 15px 0;">

Inicie sesión nuevamente, una bonita aplicación de control de energía estará presente en la bandeja del sistema.

**Características:**
- 🔋 Controlar frecuencia de CPU
- 📊 Ver estado de la batería
- 💤 Configurar acciones de suspensión e hibernación
- 🔘 Manejar eventos de cierre de tapa
- ⚡ Configuración del botón de encendido

</div>

---

## <span style="color: #D62828;">7. Sensores de hardware</span>

La mayoría de las computadoras vienen con varios sensores, que pueden usarse para monitorear su hardware y prevenir fallos inesperados. Aquí es donde entra la aplicación **ksensors**.

```bash
$ sudo apt install ksensors-trinity
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #D62828;">

Encontrará la aplicación de monitoreo 'ksensors' en el menú Inicio o en la bandeja del sistema.

**Características:**
- 🌡️ Monitoreo de temperatura
- ⚡ Sensores de voltaje
- 🌀 Monitoreo de velocidad del ventilador
- 🔔 Alarmas y umbrales
- ⚙️ Acciones al superar límites

</div>

Q4OS debería reconocer los sensores disponibles automáticamente fuera de la caja. Si no, debe detectar los módulos del kernel necesarios:

```bash
$ sudo sensors-detect
```

Se le preguntará al final del proceso de escaneo si desea agregar lo que encuentre al archivo '/etc/modules'. Responda 'sí' y luego reinicie.

---

## <span style="color: #7209B7;">8. Dispositivo táctil</span>

Q4OS usa el controlador **libinput** para controlar el panel táctil y los dispositivos apuntadores relacionados de forma predeterminada.

Consulte la lista completa de opciones de configuración de 'libinput':

```bash
$ man libinput
```

Todas las opciones se pueden aplicar en el archivo `/etc/X11/xorg.conf.d/60-libinput.conf`.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Alternativa: Controlador Synaptics**

Puede hacer que un controlador 'synaptics' más antiguo tenga prioridad sobre 'libinput':

```bash
$ sudo apt install xserver-xorg-input-synaptics
```

Use la herramienta de línea de comandos 'synclient' predeterminada para configurar paneles táctiles Synaptics:

```bash
$ synclient
```

Para ver todas las opciones disponibles:

```bash
$ man synaptics
```

Ejemplo - deshabilitar el 'tap to click' del panel táctil:

```bash
$ synclient TapButton1=0 TapButton2=0
```

</div>

Para obtener información más detallada, por favor lea la [documentación de Debian](https://wiki.debian.org/SynapticsTouchpad).

---

## <span style="color: #F77F00;">9. Códecs multimedia propietarios</span>

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 15px 0;">

Muchos códecs ya están disponibles en los repositorios predeterminados. Estos incluyen códecs para:
- 🎵 MP3
- 🎬 H264
- 🔊 Codificación y decodificación AAC

Si desea instalar una colección adicional de códecs de calidad profesional, puede ejecutar un instalador fácil de usar desde el **Centro de software Q4OS**.

Reproductores multimedia como VLC y Mplayer hacen uso de estos códecs para proporcionar soporte para la reproducción de archivos codificados a través de estos muchos códecs diferentes.

</div>

---

## <span style="color: #06A77D;">10. Controladores de video propietarios</span>

Instale controladores propietarios para mejorar el rendimiento de video y obtener aceleración 3D completa. Consulte la página de la [wiki de tarjetas gráficas de Debian](https://wiki.debian.org/GraphicsCard) para obtener instrucciones detalladas.

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
🎮 <strong>Para usuarios de NVIDIA:</strong> Si tiene una tarjeta gráfica NVIDIA, puede ejecutar el instalador desde el Centro de software Q4OS. Sondeará el hardware para buscar controladores disponibles y los instalará de manera amigable.
</blockquote>

---

## <span style="color: #D62828;">11. Usuarios y grupos</span>

### <span style="color: #D62828;">11.1. Agregar un usuario regular</span>

Abra la ventana "Usuarios y grupos":

```
Panel de Control → Administración del Sistema → Usuarios y grupos
```

<div style="background-color: #FFEBEE; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Pasos:**

1. Haga clic en el botón "Agregar"
2. Especifique el nuevo nombre de usuario y complete los detalles del usuario
3. Asigne usuarios a grupos específicos del sistema para especificar los derechos de usuario

**Grupos recomendados para nuevos usuarios:**
- `cdrom` - Acceso a CD/DVD
- `audio` - Reproducción de audio
- `video` - Dispositivos de video
- `plugdev` - Dispositivos extraíbles
- `netdev` - Gestión de red
- `powerdev` - Gestión de energía
- `lpadmin` - Instalación de impresora
- `sudo` - Permisos de administrador

</div>

---

## <span style="color: #7209B7;">12. Interconexión Android</span>

Use la aplicación **gmtp** - un administrador de archivos gráfico rápido y bien organizado que conecta la mayoría de los teléfonos y otros dispositivos Android a la PC mediante un cable USB.

```bash
$ sudo apt install gmtp
```

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Uso:**

1. Conecte su dispositivo mediante un cable USB
2. Configúrelo como dispositivo MTP
3. Ejecute el administrador de archivos 'gmtp'

Podrá navegar por la estructura de directorios interna y copiar, eliminar y administrar archivos desde su dispositivo Android.

</div>

---

## <span style="color: #F77F00;">13. Actualizaciones de seguridad, gestión de software</span>

Q4OS usa el sistema de gestión de paquetes **Apt** y herramientas relacionadas para mantener la salud y limpieza del sistema. Hay un mecanismo automático de actualizaciones desatendidas para obtener actualizaciones de seguridad y software silenciosamente.

Si necesita actualizar su sistema inmediatamente manualmente, ejecute los comandos en la terminal:

```bash
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
📚 <strong>Más información:</strong> Si desea saber cómo instalar software adicional, por favor siga el manual del usuario 'Aplicaciones Q4OS disponibles', disponible en la sección <a href="https://www.q4os.org/documents.html" style="color: #2E86AB;">Documentos</a> del sitio web de Q4OS.
</blockquote>

---

### <span style="color: #F77F00;">13.1. Administrador de actualizaciones</span>

El Administrador de actualizaciones notifica a los usuarios sobre las actualizaciones de seguridad y software disponibles y les permite actualizar el sistema bajo demanda.

Puede instalar fácilmente el Administrador de actualizaciones desde el **Centro de software Q4OS**.

---

## <span style="color: #06A77D;">14. Repositorios de software externos</span>

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Solo para usuarios avanzados:</strong> Este capítulo está destinado específicamente a usuarios avanzados familiarizados con el sistema de gestión de paquetes de Debian.
</blockquote>

La configuración predeterminada de Q4OS ofrece el conjunto básico y confiable de repositorios de software. Si desea agregar más repositorios externos, es libre de seguir los procedimientos estándar de Debian.

<div style="background-color: #E8F5E9; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Ejemplo: Instalación del navegador web Opera**

Enumere los repositorios predefinidos disponibles:

```bash
$ sudo qrepoadd --gui
```

Seleccione el repositorio 'opera' del cuadro combinado desplegable y haga clic en el botón 'Aceptar'. Alternativamente:

```bash
$ sudo qrepoadd opera
```

Instale paquetes:

```bash
$ sudo apt update
$ sudo apt install opera-stable
```

**Para desinstalar y deshabilitar el repositorio:**

```bash
$ sudo apt autoremove opera-stable
$ sudo qreporm opera
$ sudo apt update
```

</div>

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Advertencia:</strong> Agregar repositorios externos de terceros es una acción de sistema de bajo nivel y podría influir profundamente en la integridad y dependencias de la base de datos de paquetes. Afortunadamente, el sistema de gestión de paquetes Apt contiene herramientas poderosas para que los administradores reparen dependencias rotas.
</blockquote>

---

## <span style="color: #7209B7;">15. Entornos de escritorio alternativos</span>

Se admite la integración de otros entornos de escritorio en el sistema Q4OS. Pueden instalarse junto con el escritorio Trinity predeterminado, por ejemplo:
- KDE Plasma
- LXQt
- XFCE
- Y otros

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 15px 0;">

**Instalación:**

Puede agregar un entorno de escritorio usando la herramienta Desktop Profiler:

```bash
$ swprofiler.exu
```

Haga clic en el botón ">" en la esquina superior derecha para seleccionar el entorno de escritorio e instalarlo junto con un perfil de escritorio.

**Cambiar de escritorio:**

Después de reiniciar, los usuarios podrán elegir a qué entorno de escritorio iniciar sesión:

1. En la pantalla de inicio de sesión TDM, haga clic en el botón 'Menú'
2. Vaya a 'Tipo de sesión'
3. Seleccione el entorno de escritorio deseado

</div>

---

## <span style="color: #F77F00;">16. Agregar más idiomas</span>

Es posible agregar múltiples idiomas a Q4OS y establecer diferentes entornos nacionales para diferentes usuarios.

### <span style="color: #F77F00;">16.1. Agregar idiomas</span>

El administrador instala paquetes de localización separados y los usuarios podrán cambiar entre diferentes idiomas.

Ejecute el asistente de nuevo idioma desde la terminal (repita para varios idiomas):

```bash
$ addlanguage
```

Si ha instalado algunas aplicaciones que tienen paquetes de localización separados, instálelos también. **Ejemplo Libre Office:**

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-xx
```

**Opcional - cambiar la configuración regional global del sistema y la zona horaria:**

```bash
$ sudo dpkg-reconfigure locales
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #F77F00;">16.2. Configuración de usuario</span>

<div style="background-color: #FFF8E7; padding: 20px; border-radius: 8px; margin: 15px 0;">

**Paso 1:** Elegir y establecer una configuración regional (preferir configuraciones regionales UTF8):

```bash
$ chqloc --list
$ chqloc --setlocale xx_XX.utf8
```

**Paso 2:** Seleccionar el nuevo idioma del usuario

Abra el diálogo "País/Región e Idioma":

```
Panel de Control → Regional y Accesibilidad → País/Región e Idioma
```

Elija su país haciendo clic en el botón del país. Esto configurará el idioma del usuario así como varias convenciones nacionales (formato de fecha/hora, moneda, etc.).

**Paso 3:** Seleccionar una distribución de teclado:

```
Panel de Control → Regional y Accesibilidad → Distribución del teclado
```

¡Inicie sesión nuevamente - verá su perfil traducido al idioma elegido!

</div>

---

### <span style="color: #F77F00;">16.3. Ejemplo</span>

<div style="background-color: #E3F2FD; padding: 20px; border-radius: 8px; margin: 15px 0; border-left: 5px solid #2E86AB;">

**Escenario:** Instalación nueva de Q4OS con la suite Libre Office instalada. Nos gustaría configurar el idioma alemán.

**Paso 1:** Ejecute el asistente de nuevo idioma para seleccionar alemán:

```bash
$ addlanguage
```

**Paso 2:** Paquete de idioma de Libre Office:

```bash
$ apt-cache search libreoffice-l10n
$ sudo apt install libreoffice-l10n-de
```

**Paso 3:** Establecer la configuración regional alemana del usuario:

```bash
$ chqloc --list
$ chqloc --setlocale de_DE.utf8
```

**Paso 4:** Abra el diálogo "País/Región e Idioma":

```
Panel de Control → Regional y Accesibilidad → País/Región e Idioma
```

Haga clic en el primer botón con la bandera del país y elija "Europa, Central → Alemania".

**Paso 5:** Seleccionar la distribución de teclado alemán:

```
Panel de Control → Regional y Accesibilidad → Distribución del teclado
```

**Paso 6:** ¡Inicie sesión nuevamente - su perfil ahora está en alemán! 🇩🇪

</div>

---

## <span style="color: #D62828;">17. Varios consejos</span>

### <span style="color: #D62828;">17.1. Menú Inicio Kickoff</span>

Un menú Inicio bien organizado y de estilo moderno ofrece barra de búsqueda, pestaña de favoritos, historial y más.

Para cambiar al menú Kickoff, haga clic derecho en el panel del sistema:

```
Configurar panel → Menús → Estilo del menú Inicio → Kickoff
```

Puede restaurar el menú Inicio predeterminado de la misma manera.

---

### <span style="color: #D62828;">17.2. Iconos de un solo clic</span>

La activación de iconos mediante doble clic del mouse es predeterminada en Q4OS. Es fácil configurar la activación con un solo clic:

```
Panel de Control → Periféricos → Mouse → Pestaña General → Abrir archivos y carpetas con un solo clic
```

---

### <span style="color: #D62828;">17.3. Efectos de escritorio</span>

Active los efectos de suavizado y embellecimiento del escritorio.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Nota:</strong> Los efectos de escritorio funcionarán perfectamente solo en hardware moderno. No se recomienda usarlos con hardware heredado.
</blockquote>

Habilitar efectos de escritorio:

```bash
$ ctrl-compmgr --enable
```

Deshabilitar efectos de escritorio:

```bash
$ ctrl-compmgr --disable
```

---

### <span style="color: #D62828;">17.4. Inicio de sesión automático</span>

Es posible omitir la pantalla de inicio de sesión e iniciar sesión automáticamente con un usuario especificado después del arranque del sistema.

Ver todas las opciones posibles:

```bash
$ sudo ctrl-autologin --help
```

Habilitar inicio de sesión automático:

```bash
$ sudo ctrl-autologin --enable username
```

---

### <span style="color: #D62828;">17.5. Escalado de pantalla</span>

Una instalación nueva de Q4OS debería detectar la resolución de pantalla automáticamente. Sin embargo, puede forzar al sistema a usar un DPI (puntos por pulgada) definido por el usuario:

```
Panel de Control → Administración del Sistema → Escalado de pantalla
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Consejo:</strong> Aumentar el valor de DPI hará que las fuentes y los iconos sean más grandes. Un valor correcto para pantallas modernas varía de 120 a 200 DPI dependiendo del tipo de pantalla.
</blockquote>

---

### <span style="color: #D62828;">17.6. Selección de zona horaria</span>

Ejecute el comando en la terminal para seleccionar la zona horaria del sistema:

```bash
$ sudo dpkg-reconfigure tzdata
```

---

### <span style="color: #D62828;">17.7. Contraseña root</span>

La contraseña de superusuario root está deshabilitada de forma predeterminada en Q4OS. Use "sudo" para ejecutar comandos como root.

También puede habilitar y cambiar manualmente la contraseña root para poder usar la cuenta root directamente:

```bash
$ sudo passwd
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Configuración y Uso</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Manual de usuario de Trinity desktop, rev. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Sitio web oficial de Q4OS</a> | 
📖 <a href="https://www.q4os.org/documents.html" style="color: #FFD700; text-decoration: none;">Documentación</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Foro comunitario</a>
</p>

</div>
