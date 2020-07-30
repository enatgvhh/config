#

Git Installation
================

Installieren wir [git](https://git-scm.com/downloads) und starten anschließend die *cmd.exe* mit unserem Standarduser, um die Installation zu überprüfen sowie User- und Proxy-Einstellungen zu setzen.
```
git --version
git help

git config --global user.name myUserName
git config --global user.email myEmail@adr
git config --global http.proxy 111.11.111.111:80
git config --global https.proxy 111.11.111.111:80
git config --list
```  
Jetzt legen wir uns einen Ordner für die git-workspaces an, initiieren den Ordner und clonen uns dieses Repository.
```
cd C:\git_workspaces
git init
git clone https://github.com/enatgvhh/config.git
```
Git lässt sich per command line recht einfach updaten. Dazu starten wir die *cmd.exe* mit **admin** Rechten.
```
git update-git-for-windows
```
Als Git Clients lassen sich sowohl Eclipse (*git Integration in Standardinstallation enthalten*) als auch VS Code nutzen. Von der Funktionalität her ist VS Code etwas schlanker und übersichtlicher, kann aber durch zusätzliche Extensions wie * Git History* erweitert werden.
