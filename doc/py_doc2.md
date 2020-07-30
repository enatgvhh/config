#

Python virtual environment
==========================

Es kann durchaus sinnvoll sein, die Pakete nicht im global environment sondern projektbezogen in einem virtual environment zu installieren. Das tun wir jetzt exemplarisch für ein machine learning Projekt. Die virtuelle Umgebung generieren wir mit *venv*, welches mit der Standardinstallation bereits vorhanden ist. Alternativ kann dies auch mit *virtualenv* oder *pipenv* erfolgen, was die Installation der entsprechenden Pakete voraussetzt. Dazu starten wir die *cmd.exe* mit **admin** Rechten.
```
cd C:\Program Files
mkdir python_37_env
cd python_37_env
mkdir project_ml
cd C:\Program Files\python_37_env\project_ml
python -m venv venv --prompt project_ml
```
Aktivieren die virtuelle Umgebung und installieren die benötigten Pakete.
```
cd C:\Program Files\python_37_env\project_ml\venv\Scripts
activate.bat

pip install --upgrade pip --proxy="111.11.111.111:80"
pip install pylint --proxy="111.11.111.111:80"
pip install numpy --proxy="111.11.111.111:80"
pip install pandas --proxy="111.11.111.111:80"
pip install scipy --proxy="111.11.111.111:80"
pip install matplotlib --proxy="111.11.111.111:80"
pip install sqlalchemy --proxy="111.11.111.111:80"
pip install scikit-learn --proxy="111.11.111.111:80"
pip install jupyter --proxy="111.11.111.111:80"
pip install Pillow --proxy="111.11.111.111:80"
pip install tensorflow --proxy="111.11.111.111:80"
pip install tensorflow-hub --proxy="111.11.111.111:80"

pip list
pip list --local
```
Die installierten Pakete können auch in ein Requirements-File geschrieben werden, welches sich für eine erneute Installation heranziehen lässt.
```
pip list freeze > requirements.txt
pip install -r requirements.txt

deactivate
```
Der Vollständigkeit halber noch das Upgrade…
```
pip install --upgrade pip --proxy="111.11.111.111:80"
pip install --upgrade pylint --proxy="111.11.111.111:80"
pip install --upgrade numpy --proxy="111.11.111.111:80"
pip install --upgrade pandas --proxy="111.11.111.111:80"
pip install --upgrade scipy --proxy="111.11.111.111:80"
pip install --upgrade matplotlib --proxy="111.11.111.111:80"
pip install --upgrade sqlalchemy --proxy="111.11.111.111:80"
pip install --upgrade scikit-learn --proxy="111.11.111.111:80"
pip install --upgrade jupyter --proxy="111.11.111.111:80"
pip install --upgrade Pillow --proxy="111.11.111.111:80"
pip install --upgrade tensorflow --proxy="111.11.111.111:80"
pip install --upgrade tensorflow-hub --proxy="111.11.111.111:80"
```
Um in VS Code in dieser virtuellen Umgebung zu arbeiten, gehen wir wie folgt vor. Starten die *cmd.exe* als normaler User, aktivieren die virtuelle Umgebung und starten per command line VS Code.
```
cd C:\Program Files\python_37_env\project_ml\venv\Scripts
activate.bat
cd C:\Program Files\Microsoft VS Code
code
```
Jetzt müssen wir nur darauf achten, dass auch der richtige Python Interpreter (*C:\Program Files\python_37_env\project_ml\venv\Scripts\python.exe*) verwendet wird. Auch für einen ggf. in VS Code gestarteten Jupyter Server ist darauf zu achten. Die ganze Handhabung ist in Eclipse sicher etwas bequemer, dafür fehlt in Eclipse der Jupyter Notebook und der ist im machine learning äußerst hilfreich.
