Este repositorio contiene la lista de software esencial para mi entorno de trabajo en Linux (enfocado en Arch/Pacman), incluyendo utilidades de sistema, desarrollo y personalización.

También los DotFiles de mi Config i3wm


🛠️ Herramientas de Sistema

    Gestor de Archivos: nemo (con soporte para archivos comprimidos vía nemo-fileroller, zip, unzip, p7zip, unrar).

    Particiones: gparted y dosfstools (Manejador FAT12, FAT16 y FAT32).

    Terminal: kitty.

    Mirror List: reflector (Actualizador de espejos de Pacman).

    Autenticación: polkit-gnome (Agente de autenticación).

💻 Desarrollo y Editores

    Editor de Texto: xed (Ligero) y code (Visual Studio Code).

    Entorno Java: jdk21-openjdk.

🎨 Interfaz y Personalización

    Lanzador (Launcher): rofi.

    Compositor (Transparencias/Sombras): picom.

    Temas: lxappearance (Selector de temas GTK).

    Fondo de Pantalla / Visor: feh.

🔡 Fuentes (Typography)

    General: noto-fonts y ttf-jetbrains-mono-nerd.

    Símbolos y Emojis: noto-fonts-emoji.

    Soporte CJK: noto-fonts-cjk (Chino, Japonés y Coreano).

🔌 Pantalla y Multimedia

    Reproductor de Video: mpv.

    Capturas de Pantalla: flameshot.

    Brillo Interno: brightnessctl.

    Monitor Externo (DDC/CI): ddcutil.

    [!IMPORTANT] Configuración de ddcutil: Para que funcione correctamente, es necesario cargar el módulo i2c-dev. Para automatizarlo, crea el archivo /etc/modules-load.d/i2c.conf y añade: i2c-dev

🧰 Utilidades Varias

    Calculadora: qalculate-gtk.

    USB Booteable: ventoy-bin.

🎨 Temas

    Iconos:  Flat-Remix-Blue-Dark

    Temas: Win11-Fantasy-Dark 

⚙️ Configuraciones

    📸 Gestión de Snapshots (Snapper)

        Configuración de respaldos automáticos para los subvolúmenes root y home.

        Ubicación de archivos: /etc/snapper/configs/

        Retención de Backups (Home):
            HOURLY: 10
            DAILY: 7


    🌙 Interfaz y Tema Dark
        Agregar: gtk-application-prefer-dark=theme=1 
        en: ~/.config/gtk-3.0/settings.ini


    📂 Para que Nemo sepa que Kitty es mi terminal
        Escribir en el terminal> gsettings set org.cinnamon.desktop.default-applications.terminal exec kitty

    📂 Nemo reconozca iconos
        Escribir en terminal> gsettings set org.gnome.desktop.interface gtk-theme "Flat-Remix-GTK-Blue"

