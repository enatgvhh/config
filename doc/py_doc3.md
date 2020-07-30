#

Python in VS Code
=================

Download [Visual Studio Code](https://code.visualstudio.com/download) (System Installer) und Installation. Nach dem Start installieren wir noch die *Python extension for Visual Studio Code* von Microsoft. Die Extension steht nur dem installierenden Benutzer zur Verfügung. Python seitig benötigen wir, wenn nicht schon mit *pip* installiert, die packages *pylint* und ggf. *jupyter*. Nach dem Restart von VS Code kann es losgehen.

Haben wir VS Code mit dem System Installer installiert, kann es beim Update etwas komplizierter werden, da die Proxy Settings in VS Code anscheinend nicht greifen. Das lässt sich so lösen. Wie starten die *cmd.exe* mit **admin** Rechten.
```
cd C:\Program Files\Microsoft VS Code
code --proxy-server="111.11.111.111:80"

check for updates and update
```
