<div align="center">

# 🖥️ <span style="color: #2E86AB;">Q4OS Preguntas Frecuentes</span>

### <span style="color: #6C757D;">Manual de Usuario de Trinity Desktop</span>
*<span style="color: #A23B72;">Revisión 10/2025</span>*

<p style="color: #888; font-size: 0.9em; margin-top: 10px;">
Fuente del documento: <a href="https://www.q4os.org/dqa011.html" style="color: #2E86AB;">https://www.q4os.org/dqa011.html</a>
</p>

### 🌐 Leer en su idioma:
[🇬🇧 English](Q4OS_FAQ.md) | [🇫🇷 Français](Q4OS_FAQ.fr.md) | [🇩🇪 Deutsch](Q4OS_FAQ.de.md) | [🇪🇸 Español](Q4OS_FAQ.es.md)

</div>

---

## 📑 <span style="color: #2E86AB;">Tabla de Contenidos</span>

### <span style="color: #F77F00;">1. [Introducción](#1-introducción)</span>

### <span style="color: #06A77D;">2. [Instalación](#2-instalación)</span>
- 2.1. [¿Cómo puedo crear un disco USB de instalación de Q4OS booteable?](#21-cómo-puedo-crear-un-disco-usb-de-instalación-de-q4os-booteable)
- 2.2. [¿Hay alguna manera de hacer dual boot de Q4OS junto con Windows?](#22-hay-alguna-manera-de-hacer-dual-boot-de-q4os-junto-con-windows)
- 2.3. [No tengo sonido después de la instalación, ¿qué debo hacer?](#23-no-tengo-sonido-después-de-la-instalación-qué-debo-hacer)
- 2.4. [No puedo conectarme a la red inalámbrica, ¿qué hacer?](#24-no-puedo-conectarme-a-la-red-inalámbrica-qué-hacer)

### <span style="color: #D62828;">3. [Sistema](#3-sistema)</span>
- 3.1. [Hay dependencias de paquetes rotas en mi sistema. ¿Cómo puedo arreglarlo?](#31-hay-dependencias-de-paquetes-rotas-en-mi-sistema-cómo-puedo-arreglarlo)
- 3.2. [Algunas letras se escriben mal ('L' aparece como '3', 'J' como '1')](#32-algunas-letras-se-escriben-mal-l-aparece-como-3-j-como-1)
- 3.3. [Las fuentes y los iconos son demasiado pequeños en mi pantalla hiDPI, ¿puedo hacerlos más grandes?](#33-las-fuentes-y-los-iconos-son-demasiado-pequeños-en-mi-pantalla-hidpi-puedo-hacerlos-más-grandes)
- 3.4. [¿Cómo puedo mostrar la temperatura actual de la CPU en el panel del sistema?](#34-cómo-puedo-mostrar-la-temperatura-actual-de-la-cpu-en-el-panel-del-sistema)
- 3.5. [Estoy detrás de un proxy, las aplicaciones basadas en el gestor de paquetes no funcionan](#35-estoy-detrás-de-un-proxy-las-aplicaciones-basadas-en-el-gestor-de-paquetes-no-funcionan)
- 3.6. [Quiero usar un kernel de Linux reciente, ¿es posible?](#36-quiero-usar-un-kernel-de-linux-reciente-es-posible)

### <span style="color: #7209B7;">4. [Escritorio](#4-escritorio)</span>
- 4.1. [¿Cómo configuro múltiples escritorios virtuales en Q4OS?](#41-cómo-configuro-múltiples-escritorios-virtuales-en-q4os)
- 4.2. [No puedo renombrar o editar algunos iconos en mi Escritorio](#42-no-puedo-renombrar-o-editar-algunos-iconos-en-mi-escritorio)
- 4.3. [¿Cómo puedo editar el menú Inicio?](#43-cómo-puedo-editar-el-menú-inicio)
- 4.4. [¿Puedo personalizar la vista y los accesos directos en el panel derecho del menú Inicio 'Bourbon' predeterminado de Q4OS?](#44-puedo-personalizar-la-vista-y-los-accesos-directos-en-el-panel-derecho-del-menú-inicio-bourbon-predeterminado-de-q4os)
- 4.5. [Quiero que la entrada de la pantalla de bienvenida aparezca en el menú Inicio](#45-quiero-que-la-entrada-de-la-pantalla-de-bienvenida-aparezca-en-el-menú-inicio)
- 4.6. [¿Cómo puedo iniciar automáticamente una aplicación?](#46-cómo-puedo-iniciar-automáticamente-una-aplicación)
- 4.7. [He estropeado mi escritorio, ¿cómo puedo revertir los colores, fuentes, tema y otras configuraciones predeterminadas?](#47-he-estropeado-mi-escritorio-cómo-puedo-revertir-los-colores-fuentes-tema-y-otras-configuraciones-predeterminadas)
- 4.8. [¿Cómo puedo configurar iconos de un solo clic en lugar de doble clic?](#48-cómo-puedo-configurar-iconos-de-un-solo-clic-en-lugar-de-doble-clic)
- 4.9. [Dígame la forma más fácil de obtener una captura de pantalla](#49-dígame-la-forma-más-fácil-de-obtener-una-captura-de-pantalla)
- 4.10. [¿Es posible cambiar el tema de iconos?](#410-es-posible-cambiar-el-tema-de-iconos)
- 4.11. [He definido atajos de teclado en el Panel de Control, pero no funcionan](#411-he-definido-atajos-de-teclado-en-el-panel-de-control-pero-no-funcionan)
- 4.12. [He notado que la entrada 'Programas' ha desaparecido del menú Inicio](#412-he-notado-que-la-entrada-programas-ha-desaparecido-del-menú-inicio)
- 4.13. [El atajo de teclado no funciona para cambiar entre distribuciones de teclado no latinas](#413-el-atajo-de-teclado-no-funciona-para-cambiar-entre-distribuciones-de-teclado-no-latinas)
- 4.14. [Necesito ajustar el brillo de la pantalla](#414-necesito-ajustar-el-brillo-de-la-pantalla)

### <span style="color: #F77F00;">5. [Aplicaciones](#5-aplicaciones)</span>
- 5.1. [¿Cómo puedo configurar la transparencia de 'Conky'?](#51-cómo-puedo-configurar-la-transparencia-de-conky)

---

## <span style="color: #F77F00;">1. Introducción</span>

<blockquote style="background-color: #FFF8E7; border-left: 5px solid #F77F00; padding: 15px; margin: 15px 0; border-radius: 5px;">
📢 Infórmenos sobre cualquier error que encuentre, las sugerencias son bienvenidas. Cuando sea posible, envíenos lo que crea que sería una solución más clara. Puede acudir con seguridad a las <a href="http://www.trinitydesktop.org/faq/index.php" style="color: #2E86AB;">FAQ del entorno de escritorio Trinity</a>.
</blockquote>

---

## <span style="color: #06A77D;">2. Instalación</span>

### <span style="color: #06A77D;">2.1. ¿Cómo puedo crear un disco USB de instalación de Q4OS booteable?</span>

La forma más fácil en Linux es conectar su dispositivo USB, no montarlo, y ejecutar en la terminal:

```bash
$ sudo cp bootable.iso /dev/sdx
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
📝 <strong>Nota:</strong><br>
• <code>sdx</code> es la unidad USB de destino, por ejemplo <code>sdb</code><br>
• <code>bootable.iso</code> es la imagen CD de instalación booteable de Q4OS, puede descargarla desde el sitio web de Q4OS
</blockquote>

Alternativamente, puede usar el software multiplataforma **UNetbootin** o **Rufus** para crear discos USB booteables. Vea [cómo crear un medio live](https://www.q4os.org/dqa018.html#creat).

---

### <span style="color: #06A77D;">2.2. ¿Hay alguna manera de hacer dual boot de Q4OS junto con Windows?</span>

¡Por supuesto! La forma preferida es proceder con la instalación desde un CD 'Live', ya que le da la opción de instalar el cargador de arranque. Si deja que el instalador instale el cargador de arranque Grub, detectará automáticamente los sistemas operativos disponibles incluyendo Windows y los ofrecerá todos en cada arranque.

Si desea mantener el cargador de arranque de Windows, no olvide desmarcar la casilla correspondiente durante la instalación.

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Importante:</strong> Recomendamos encarecidamente hacer una copia de seguridad de todos sus datos antes. Por favor lea las <a href="https://www.q4os.org/dqa018.html" style="color: #D62828;">instrucciones de instalación</a>.
</blockquote>

---

### <span style="color: #06A77D;">2.3. No tengo sonido después de la instalación, ¿qué debo hacer?</span>

Le recomendamos instalar primero el servidor de sonido Pipewire:

```bash
$ sudo apt install pipewire pavucontrol-qt
```

Reinicie su computadora. Luego siga estos pasos:

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Pasos de configuración:**

1. Clic derecho en el ícono 'mezclador' en la bandeja del sistema → 'Seleccionar canal maestro...'
2. Establezca 'Mezclador actual' en 'PipeWire' en la lista desplegable superior derecha
3. Haga clic en 'Aceptar' para cerrar el diálogo
4. Ejecute la aplicación 'Control de volumen' desde el menú Inicio
5. Configure los ajustes del mezclador de salida en la pestaña 'Dispositivos de salida'
6. Verifique que los canales de salida no estén silenciados

</div>

El sistema de audio debería funcionar ahora. Si no, continúe siguiendo los pasos a continuación.

**Diagnóstico adicional:**

Haga clic izquierdo en el ícono 'mezclador' en la bandeja del sistema, y haga clic en el botón 'Mezclador' para verificar y actualizar los niveles del mezclador de audio. Asegúrese de que la tarjeta de sonido 'PipeWire' esté seleccionada en la esquina superior derecha de la ventana del mezclador 'kmix'.

Luego ejecute el comando en la terminal y verifique la salida de depuración:

```bash
$ artsplay /opt/trinity/share/sounds/KDE_Startup.wav
```

Si todavía no hay sonido, termine temporalmente el servidor de sonido Trinity e intente reproducir audio con un reproductor alsa independiente:

```bash
$ artsshell terminate
$ aplay /opt/trinity/share/sounds/KDE_Startup.wav
```

Nuevamente, verifique la salida de depuración. Si su sistema de audio todavía no funciona, continúe siguiendo la [Solución de problemas de sonido](http://www.trinitydesktop.org/faq/sound.php) en las FAQ de Trinity.

---

### <span style="color: #06A77D;">2.4. No puedo conectarme a la red inalámbrica, ¿qué hacer?</span>

Q4OS admite completamente las redes inalámbricas e incluye una herramienta llamada **tdenetworkmanager** para gestionar conexiones inalámbricas. Puede encontrarla en la bandeja del sistema.

Si tiene problemas para conectarse a una red inalámbrica, por favor lea la [publicación de solución de problemas wifi](https://www.q4os.org/forum/viewtopic.php?id=4698).

---

## <span style="color: #D62828;">3. Sistema</span>

### <span style="color: #D62828;">3.1. Hay dependencias de paquetes rotas en mi sistema. ¿Cómo puedo arreglarlo?</span>

Tenemos una herramienta práctica para reparar automáticamente las dependencias rotas en Q4OS, simplemente ejecute en la terminal:

```bash
$ sudo sh /usr/share/apps/q4os_system/bin/qapt_fix.sh
$ sudo apt update
$ sudo apt dist-upgrade
```

<blockquote style="background-color: #FFEBEE; border-left: 5px solid #D62828; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Recordatorio:</strong> Recomendamos encarecidamente instalar software solo de fuentes confiables y compatibles con Debian para evitar que el sistema de paquetes se corrompa.
</blockquote>

---

### <span style="color: #D62828;">3.2. Algunas letras se escriben mal ('L' aparece como '3', 'J' como '1')</span>

Un fallo común que ocurre en netbooks con un teclado pequeño. El teclado está bloqueado por NumLock, podría intentar desactivar NumLock.

Inicie el Panel de Control:

```
Panel de Control → Periféricos → Teclado → NumLock al inicio de KDE → establecer en Desactivado
```

Inicie sesión nuevamente e intente usar el teclado.

---

### <span style="color: #D62828;">3.3. Las fuentes y los iconos son demasiado pequeños en mi pantalla hiDPI, ¿puedo hacerlos más grandes?</span>

¡Sí! Q4OS puede escalar la resolución de pantalla. Por favor lea el capítulo [resolución de pantalla](https://www.q4os.org/dqa007.html#tips.6).

---

### <span style="color: #D62828;">3.4. ¿Cómo puedo mostrar la temperatura actual de la CPU en el panel del sistema?</span>

Ejecute la aplicación **ksensors** desde:

```
Menú Inicio → Programas → Accesorios → Sistema → KSensors
```

Si **ksensors** aún no está instalado, siga el capítulo [sensores de hardware](https://www.q4os.org/dqa007.html#hwsens) para instalarlo.

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0; border-left: 5px solid #7209B7;">

**Configuración:**

1. Clic derecho en el ícono 'ksensors' en la bandeja del sistema → Configurar
2. Seleccione el grupo de sensores HW relacionado
3. Seleccione el sensor deseado de la lista
4. Pestaña Dock → marque la casilla 'Visible'
5. Opcionalmente puede establecer colores, alarmas, umbrales, acciones al superar límites y otras opciones
6. Haga clic en el botón 'Aplicar' y cierre el diálogo

</div>

---

### <span style="color: #D62828;">3.5. Estoy detrás de un proxy, las aplicaciones basadas en el gestor de paquetes no funcionan</span>

Necesita establecer variables de entorno a nivel de sistema. Abra el archivo `/etc/environment` con su editor favorito y agregue las siguientes líneas (modificando apropiadamente):

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
📝 <strong>Nota:</strong> Debe duplicar tanto en mayúsculas como en minúsculas porque algunos programas solo buscan uno u otro.
</blockquote>

El sistema de gestión de paquetes APT no obedecerá las variables de entorno cuando se usa normalmente con sudo. Así que configúrelas por separado; cree un archivo llamado `95proxies` en `/etc/apt/apt.conf.d/`, e incluya lo siguiente:

```bash
Acquire::http::proxy "http://myproxy.server.com:8080/";
Acquire::ftp::proxy "ftp://myproxy.server.com:8080/";
Acquire::https::proxy "https://myproxy.server.com:8080/";
```

Finalmente, reinicie para asegurarse de que los cambios surtan efecto.

---

### <span style="color: #D62828;">3.6. Quiero usar un kernel de Linux reciente, ¿es posible?</span>

Recomendamos usar el kernel predeterminado de Q4OS/Debian, fiable y profundamente probado. No hay demasiadas razones para que los usuarios ordinarios usen un kernel más nuevo.

<blockquote style="background-color: #FFF3E0; border-left: 5px solid #F77F00; padding: 12px; margin: 10px 0; border-radius: 5px;">
⚠️ <strong>Advertencia:</strong> Los últimos kernels no son tan seguros como el kernel predeterminado de Debian, estable como una roca y exhaustivamente probado, sin embargo podrían traer mejoras y nuevos controladores de dispositivos y soporte.
</blockquote>

Si prefiere por alguna razón el último kernel de Linux, ejecute el script de autoinstalación en la terminal para instalarlo fácilmente desde el repositorio backports:

```bash
$ qinst-kernel-bpo
```

<blockquote style="background-color: #E8F5E9; border-left: 5px solid #06A77D; padding: 12px; margin: 10px 0; border-radius: 5px;">
✅ <strong>Bueno saber:</strong> El antiguo buen kernel predeterminado no será desinstalado, por lo que puede elegirlo y arrancarlo en cualquier momento desde el menú de arranque grub, si tiene algún problema.
</blockquote>

---

## <span style="color: #7209B7;">4. Escritorio</span>

### <span style="color: #7209B7;">4.1. ¿Cómo configuro múltiples escritorios virtuales en Q4OS?</span>

<div style="background-color: #F3E5F5; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Paso 1:** Inicie el Panel de Control y vaya a:

```
Escritorio → Múltiples escritorios
```

Seleccione cuántos escritorios virtuales desea tener.

**Paso 2a:** Agregue un applet cambiador de escritorio a su barra de tareas:

1. Clic derecho en la barra de tareas
2. Seleccione 'Agregar applet al panel' (si la barra de tareas está bloqueada, desbloquéela primero)
3. En la ventana emergente, seleccione 'Pager / Switcher de escritorio'
4. Haga clic en 'Agregar al panel'

**Paso 3a:** Configure un atajo de teclado:

1. Inicie el Panel de Control
2. Vaya a: `Regional y Accesibilidad → Atajos de teclado`
3. En la pestaña 'Atajos globales', desplácese hacia abajo y encuentre 'Cambiar al siguiente escritorio' bajo 'Cambio de escritorio'
4. Haga clic en el botón junto a la opción 'Personalizado'
5. Asigne la combinación de teclas que desea usar
6. Haga clic en 'Aceptar' para guardar

</div>

---

### <span style="color: #7209B7;">4.2. No puedo renombrar o editar algunos iconos en mi Escritorio</span>

Podría haber tres tipos lógicos de iconos presentes en su escritorio:

<div style="background-color: #FFF8E7; padding: 15px; border-radius: 8px; margin: 10px 0;">

**1. Iconos del Sistema** 🔒
- 'Mi Equipo', 'Mis Documentos', 'Mis Sitios de Red', 'Papelera', 'Navegador Web', 'Impresoras'
- Propiedad de root
- No editables directamente por un usuario
- Pueden eliminarse del escritorio

**2. Iconos Globales** 🌐
- Generalmente creados por instaladores de aplicaciones
- Propiedad de root y compartidos por todos los usuarios
- Los usuarios pueden ocultarlos pero no editarlos o renombrarlos

**3. Iconos de Usuario** 👤
- Creados por un solo usuario
- Control total: eliminar, renombrar, editar propiedades (clic derecho → Propiedades)

</div>

<blockquote style="background-color: #E3F2FD; border-left: 5px solid #2E86AB; padding: 12px; margin: 10px 0; border-radius: 5px;">
💡 <strong>Consejo:</strong> Si desea editar un icono global o del sistema, recomendamos eliminarlo del escritorio y crear un icono de usuario correspondiente usando Arrastrar y soltar → Copiar desde el menú Inicio. Será propiedad del usuario y completamente editable.
</blockquote>

---

### <span style="color: #7209B7;">4.3. ¿Cómo puedo editar el menú Inicio?</span>

1. Abra el menú Inicio
2. Clic derecho en cualquier elemento bajo la entrada 'Programas'
3. Seleccione 'Editar menú'
4. Aparece la ventana del editor de menús

Podrá crear una nueva estructura personalizada de submenús/carpetas y llenarla con los elementos de menú deseados. Puede crear nuevos accesos directos usando el clic derecho, o arrastrar y soltar iconos desde el menú Inicio o el Escritorio en la ventana del editor de menús.

Los elementos recién creados aparecerán en el menú Inicio después de cerrar la ventana del editor de menús.

**Bonus:** También puede cambiar para que los elementos del menú Inicio se organicen por Categorías o por Aplicaciones:

```bash
$ sh /usr/share/apps/q4os_system/bin/kmenu_struct.sh --help
```

---

### <span style="color: #7209B7;">4.4. ¿Puedo personalizar la vista y los accesos directos en el panel derecho del menú Inicio 'Bourbon' predeterminado de Q4OS?</span>

¡Sí! Edite el archivo `$HOME/.trinity/share/config/kickerrc` en su directorio personal.

Hay varias opciones de configuración que comienzan con 'Bourbon' comentadas por defecto. Necesita:

1. Descomentar la línea `BourbonSysViewCustomItems`
2. Especificar los enlaces `.desktop` que desea que se muestren en el panel de menú derecho
3. Usar coma `,` como delimitador

**Opciones adicionales:**

- Ocultar accesos directos predeterminados:
  - `BourbonShowSysViewFolders=false`
  - `BourbonShowSysViewApps=false`

---

### <span style="color: #7209B7;">4.5. Quiero que la entrada de la pantalla de bienvenida aparezca en el menú Inicio</span>

Ejecute el comando para actualizar el acceso directo de la pantalla de bienvenida en la terminal:

```bash
$ sudo kwriteconfig --file '/usr/share/applications/q4os-welcome-screen.desktop' --group 'Desktop Entry' --key 'NoDisplay' 'false'
```

Alternativamente, puede editar manualmente el archivo `/usr/share/applications/q4os-welcome-screen.desktop`.

El icono de la pantalla de bienvenida aparecerá bajo:

```
Menú Inicio → Programas → Accesorios → Sistema
```

---

### <span style="color: #7209B7;">4.6. ¿Cómo puedo iniciar automáticamente una aplicación?</span>

Necesita agregar un acceso directo de aplicación (archivo `.desktop`) en la carpeta de inicio automático:

- `$HOME/.trinity/Autostart`
- o `$HOME/.q4data/Programs/Startup`

La aplicación se iniciará inmediatamente después del inicio de sesión del usuario.

<div style="background-color: #E8F5E9; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Métodos:**

1. Arrastre cualquier acceso directo de aplicación desde el menú Inicio o el Escritorio y suéltelo en la carpeta de inicio automático
2. También es posible colocar un script shell o ejecutable en la carpeta de inicio automático

</div>

---

### <span style="color: #7209B7;">4.7. He estropeado mi escritorio, ¿cómo puedo revertir los colores, fuentes, tema y otras configuraciones predeterminadas?</span>

Simplemente ejecute en la terminal:

```bash
$ sh /usr/share/apps/q4os_system/bin/default_desktop_settings.sh
```

---

### <span style="color: #7209B7;">4.8. ¿Cómo puedo configurar iconos de un solo clic en lugar de doble clic?</span>

La activación de iconos mediante doble clic es predeterminada en Q4OS. Es fácil configurar la activación con un solo clic, el efecto de pasar el cursor y más en el Panel de Control:

```
Panel de Control → Periféricos → Ratón → Pestaña General → Abrir archivos y carpetas con un solo clic
```

---

### <span style="color: #7209B7;">4.9. Dígame la forma más fácil de obtener una captura de pantalla</span>

Puede hacer esto sin ningún paquete adicional:

<div style="background-color: #F0F8FF; padding: 15px; border-radius: 8px; margin: 10px 0;">

**Método rápido:**

1. Presione la tecla `PrtScr`
2. Clic derecho en el escritorio
3. Seleccione 'Pegar contenido del portapapeles'
4. Aparece un diálogo donde puede ingresar el nombre de archivo y el tipo de imagen
5. El archivo se guardará en el escritorio

También puede abrir Konqueror para navegar a la carpeta preferida, hacer clic derecho y seleccionar 'Pegar contenido del portapapeles' para guardar el archivo en la ubicación preferida.

</div>

**Aplicación dedicada:**

Existe una aplicación ligera y poderosa **ksnapshot-trinity**, capaz de capturar pantalla completa, región, una ventana o solo una parte de la ventana.

Instalación:

```bash
$ sudo apt install ksnapshot-trinity
```

---

### <span style="color: #7209B7;">4.10. ¿Es posible cambiar el tema de iconos?</span>

¡Sí! Necesita desbloquear las opciones avanzadas del Panel de Control en la terminal:

```bash
$ sudo kcmodules --unlock
```

Luego vaya a:

```
Panel de Control → Apariencia y Temas → Iconos
```

Configure el tema que prefiera.

---

### <span style="color: #7209B7;">4.11. He definido atajos de teclado en el Panel de Control, pero no funcionan</span>

Solo necesita habilitar el servicio khotkeys para que se ejecute al iniciar sesión.

Vaya al Panel de Control:

```
Panel de Control → Regional y Accesibilidad → Acciones de entrada → Pestaña Configuración General → desmarque la casilla Deshabilitar KHotKeys
```

---

### <span style="color: #7209B7;">4.12. He notado que la entrada 'Programas' ha desaparecido del menú Inicio</span>

Ocurre raramente en algunos sistemas configurados específicamente. La solución alternativa que debería solucionarlo es volver a cambiar desde el menú clásico - kicker - clásico.

Podría reportarlo como un nuevo error en nuestro [Seguimiento de errores](https://sourceforge.net/p/q4os/tickets), y agregar alguna descripción si encuentra alguna conexión.

---

### <span style="color: #7209B7;">4.13. El atajo de teclado no funciona para cambiar entre distribuciones de teclado no latinas</span>

El atajo de cambio de teclado es `Alt+Espacio` o `Ctrl+Alt+K` por defecto. Funciona perfectamente si solo tiene instaladas distribuciones de teclado latinas.

Para poder cambiar libremente teclados no latinos, necesita agregar una 'distribución latina' a cada distribución de teclado que use.

Ejecute el Panel de Control:

```
Panel de Control → Regional y Accesibilidad → Distribución del teclado → seleccione una distribución de teclado no latina → marque la casilla 'Incluir distribución latina'
```

---

### <span style="color: #7209B7;">4.14. Necesito ajustar el brillo de la pantalla</span>

Simplemente pase el mouse sobre el ícono **tdepowersave** en la bandeja del sistema, y use la rueda del mouse para ajustar el brillo hacia arriba o hacia abajo.

Si el ícono no está disponible en la bandeja del sistema, necesita instalar el paquete `tdepowersave-trinity` e iniciar sesión en la sesión de escritorio Trinity nuevamente.

**Alternativa:**

Puede instalar el paquete `klcddimmer-trinity` y agregar un applet en el panel del sistema. Sin embargo, necesitará configurarlo para usar un backend de control de brillo, por ejemplo `xbacklight`.

---

## <span style="color: #F77F00;">5. Aplicaciones</span>

### <span style="color: #F77F00;">5.1. ¿Cómo puedo configurar la transparencia de 'Conky'?</span>

Debe tener los efectos de escritorio de Q4OS/Trinity habilitados. Puede configurarse a través de la pantalla de bienvenida o el Panel de Control.

Edite el archivo `/etc/conky/conky.conf` y agregue líneas:

```bash
own_window yes
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
own_window_argb_visual
own_window_argb_value 0
```

Comente la línea:

```bash
#own_window_type desktop
```

---

<div align="center" style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 30px; border-radius: 10px; margin-top: 40px;">

<h3 style="color: white; margin: 0;">Q4OS Preguntas Frecuentes</h3>
<p style="color: #E0E0E0; margin: 10px 0;"><em>Manual de usuario de Trinity desktop, rev. 10/2025</em></p>

---

<p style="color: white; margin: 20px 0;">
📚 <a href="https://www.q4os.org/" style="color: #FFD700; text-decoration: none;">Sitio web oficial de Q4OS</a> | 
🐛 <a href="https://sourceforge.net/p/q4os/tickets" style="color: #FFD700; text-decoration: none;">Bug Tracker</a> | 
💬 <a href="https://www.q4os.org/forum/" style="color: #FFD700; text-decoration: none;">Foro</a>
</p>

</div>
