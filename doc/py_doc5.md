#

GDAL for Python
===============

Dazu benötigen wir zwei [Installer](http://www.gisinternals.com/release.php), z.B. *gdal-300-1911-x64-core.msi* und *GDAL-3.0.4.win-amd64-py3.7.msi*. Nach der Installation setzen wir den **System** PATH und fügen drei neue **System** Variablen hinzu.
```
PATH = C:\Program Files\GDAL
GDAL_DATA = C:\Program Files\GDAL\gdal-data
GDAL_DRIVER_PATH = C:\Program Files\GDAL\gdalplugins
PROJ_LIB = C:\Program Files\GDAL\projlib
```
Abschließend überprüfen wir die Installation und starten dazu die *cmd.exe*.
```
gdalinfo --version
ogrinfo --formats
```
