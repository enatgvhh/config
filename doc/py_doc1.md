#

Installation Python plus Packages
=================================

Downloaden wir eine aktuelle [Python Version](https://www.python.org/downloads/) und installieren diese benutzerdefiniert  für *all users*,  mit *environment path setting* sowie *launcher for all users*. Starten die *cmd.exe* und sehen uns Python-Version, Pip-Version sowie die im global environment installierten packages (*C:\Program Files\Python37\Lib\site-packages*) an. Vorinstalliert sind *pip* und *setuptools*.
```
python --version
pip --version
pip list
```
Wurde die Installation ohne path setting durchgeführt…
```
cd C:\Program Files\Python37
python --version
python -m pip --version

cd C:\Program Files\Python37\Scripts
pip --version
```
Jetzt installieren wir noch einige zusätzliche Pakete vom [PyPI repository](https://pypi.org/). Und zwar immer mit der neuesten Pip-Version. Die *cmd.exe* starten wir dazu mit **admin** Rechten. Ggf. ist ein Proxy zu verwenden.
```
pip install --upgrade pip --proxy="111.11.111.111:80"

pip install lxml --proxy="111.11.111.111:80"
pip install psycopg2 --proxy="111.11.111.111:80"
pip install requests --proxy="111.11.111.111:80"
pip install pylint --proxy="111.11.111.111:80"
pip install cryptography --proxy="111.11.111.111:80"
pip install schedule --proxy="111.11.111.111:80"
pip install numpy --proxy="111.11.111.111:80"
pip install pandas --proxy="111.11.111.111:80"
pip install matplotlib --proxy="111.11.111.111:80"
pip install jupyter --proxy="111.11.111.111:80"
pip install pdoc --proxy="111.11.111.111:80"

pip list
```
Von Zeit zu Zeit aktualisieren wir die Pakete…
```
pip install --upgrade pip --proxy="111.11.111.111:80"
pip install --upgrade lxml --proxy="111.11.111.111:80"
pip install --upgrade psycopg2 --proxy="111.11.111.111:80"
pip install --upgrade requests --proxy="111.11.111.111:80"
pip install --upgrade pylint --proxy="111.11.111.111:80"
pip install --upgrade cryptography --proxy="111.11.111.111:80"
pip install --upgrade schedule --proxy="111.11.111.111:80"
pip install --upgrade numpy --proxy="111.11.111.111:80"
pip install --upgrade pandas --proxy="111.11.111.111:80"
pip install --upgrade matplotlib --proxy="111.11.111.111:80"
pip install --upgrade jupyter --proxy="111.11.111.111:80"
pip install --upgrade pdoc --proxy="111.11.111.111:80"
```

