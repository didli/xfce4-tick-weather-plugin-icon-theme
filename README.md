## xfce4-tick-weather-plugin-icon-theme
ICONS = Original Icon Theme by xiao4 (aka Long Yin @http://xiao4.deviantart.com/) 

AUTHOR = Theme by mediaklan (aka didli @http://mediaklan.com) 

THEME = Weather Tick

	This icon theme should be supported by latest xfce4-weather-plugin version. 
	If not, xfce4-weather-plugin should be compiled in order to use this theme.
	Here's a method suitable for Fedora (use your own OS package manager to follow this procedure)  

**1. Xfce4-weather-plugin compilation :**

*- Verifiying we got what is needed :*
```
sudo dnf install xfce4-dev-tools && sudo dnf builddep xfce4-weather-plugin
git clone git://git.xfce.org/panel-plugins/xfce4-weather-plugin
cd xfce4-weather-plugin
./autogen.sh --prefix=/usr
make
sudo make install
```
**2. Create folders for the theme and get it :**
```
mkdir -p /home/$USER/.config/xfce4/weather/
mkdir -p /home/$USER/.config/xfce4/weather/icons/
cd /home/$USER/.config/xfce4/weather/icons/
wget http://mediaklan.com/_pix/xfce4-tick-weather-plugin-icon-theme.tar.gz
tar -xzvf xfce4-tick-weather-plugin-icon-theme.tar.gz
```
You should now get a a "tick" folder and a theme.info in /home/$USER/.config/xfce4/weather/icons/
Add the Xfce4-weather-plugin if it's not already present in one of your panel and from the plugin settings,
choose your new theme.
