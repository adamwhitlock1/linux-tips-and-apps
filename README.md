# new-linux-install-programs
A simple repo of terminal commands, and other resources to install all dev apps I like to use for a new Ubuntu install

One way to look at a list of all your Aptitude based installs on an existing Linux drive
```
dpkg -l
```

## Part 1 Helpful Links / Terminal Commands

CURL
```
sudo apt install curl
```

GIT
```
sudo apt install git-all
```

GITHUB DESKTOP FOR LINUX
https://github.com/shiftkey/desktop/releases

NODE JS
https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions

XAMPP INSTALL INSTRUCTION
https://www.wikihow.com/Install-XAMPP-on-Linux

WEBSTORM
https://www.jetbrains.com/webstorm/download

VS CODE
https://code.visualstudio.com/docs/setup/linux

Fira Code Font
https://github.com/tonsky/FiraCode

ALL GOOGLE FONTS
https://github.com/adamwhitlock1/GetAllGoogleFonts-Ubuntu

HYPER TERMINAL
https://hyper.is/#installation

UBUNTU CLEANER
```
sudo add-apt-repository ppa:gerardpuig/ppa
sudo apt-get update && sudo apt-get install ubuntu-cleaner
```

GTK+ THEME: ADAPTA NOKTO
```
sudo add-apt-repository ppa:tista/adapta
sudo apt-get update
sudo apt-get install adapta-gtk-theme
```

GTK+ THEME AND ICONS: PAPER
```
sudo add-apt-repository ppa:snwh/pulp
sudo apt-get update
sudo apt-get install paper-gtk-theme paper-icon-theme
```

GTK+ THEME: ARC
```
sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/Horst3180/xUbuntu_16.04/ /' >> /etc/apt/sources.list.d/arc-theme.list"
sudo apt-get update && sudo apt-get install arc-theme
```
or
http://download.opensuse.org/repositories/home:/Horst3180/xUbuntu_16.04/all/

TERMIUS SSH CLIENT (uses snap)
https://snapcraft.io/termius-app

HIPCHAT
```
sudo sh -c 'echo "deb https://atlassian.artifactoryonline.com/atlassian/hipchat-apt-client $(lsb_release -c -s) main" > /etc/apt/sources.list.d/atlassian-hipchat4.list'
wget -O - https://atlassian.artifactoryonline.com/atlassian/api/gpg/key/public | sudo apt-key add -
sudo apt-get update
sudo apt-get install hipchat4
```
PINEGROW WEB EDITOR
http://download.pinegrow.com/PinegrowLinux64.4.8.zip

FILEZILLA (for ubuntu 16.04)
```
sudo sh -c 'echo "deb http://archive.getdeb.net/ubuntu xenial-getdeb apps" >> /etc/apt/sources.list.d/getdeb.list'
wget -q -O - http://archive.getdeb.net/getdeb-archive.key | sudo apt-key add -
sudo apt update
sudo apt install filezilla
```

MYSQL WORKBENCH
https://dev.mysql.com/downloads/file/?id=474211

MYSQL INSTALL
```
sudo apt-get update
sudo apt-get install mysql-server
```
OR READ THIS
https://support.rackspace.com/how-to/installing-mysql-server-on-ubuntu/

MYSQL UNINSTALL
```
sudo -i
service mysql stop
killall -KILL mysql mysqld_safe mysqld
apt-get --yes purge mysql-server mysql-client
apt-get --yes autoremove --purge
apt-get autoclean
deluser --remove-home mysql
delgroup mysql
rm -rf /etc/apparmor.d/abstractions/mysql /etc/apparmor.d/cache/usr.sbin.mysqld /etc/mysql /var/lib/mysql /var/log/mysql* /var/log/upstart/mysql.log* /var/run/mysqld
updatedb
exit
```
OR TRY
```
sudo apt-get remove --purge *mysql\*
sudo apt-get autoremove
sudo apt-get autoclean
```
SUDOCABULARY
```
curl https://raw.githubusercontent.com/badarsh2/Sudocabulary/master/script.sh | bash
```
LOLCAT
```
gem install lolcat
```
RAMBOX
https://rambox.pro/#download






