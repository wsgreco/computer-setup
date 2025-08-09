# Purge libreoffice
sudo apt remove --purge libreoffice*

# Stops libreoffice from being reinstalled
sudo apt-mark hold libreoffice*

# Removes empty folders
sudo rm -r /etc/libreoffice
sudo rm -r /usr/share/fonts/truetype/libreoffice

# Disables auto start for Pop!_Shop and others
sudo sed --in-place 's/NoDisplay=true/NoDisplay=false/g' /etc/xdg/autostart/*.desktop

# Enable Wayland
sudo nano /etc/gdm3/custom.conf
Change to “WaylandEnable=true”

# Installs packages
sudo apt install htop gufw

# Install from Pop!_Shop
VSCode, Audacity, Tweaks

# Install Chrome, Rust, NVM

# Git
git config --global user.name "William Greco"
git config --global user.email "wsgreco@users.noreply.github.com"

# Create “Projects” folder

# Fix apt
sudo dpkg --configure -a
sudo apt --fix-broken install
