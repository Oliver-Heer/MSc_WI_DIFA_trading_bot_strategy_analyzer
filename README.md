# Inhalt
Beinhaltet Docker und docker-compose Definitionen um einen lokalen Container mit sämtlichen Abhängigkeiten für Python, Anaconda und JupyterLab zu erstellen. Der Container ist anschliessend unter http://localhost/lab/ aufrufbar.

Im Unterverzeichnis *notebooks* sind die JupyterNotebook Dateien (.ipynb) aufzufinden. Dort befindet sich auch die Trading Bot Strategy Analyzer Implementation.

In der */srv/anaconda/conf/requirements.txt* Datei können benötigte Python Pakete eingetragen werden. Sie werden beim Erstellen des Containers automatisch mit *pip* installiert. Wenn neue Pakete benötigt werden, muss der Container neu erstellt werden.
> docker-compose up --build

# Getting Started
1. Docker muss installiert sein

2. *Docker-compose* in einer Konsole im Projektverzeichnis ausführen.
> docker-compose up --build

3. Im Browser JupyterLab aufrufen
> http://localhost/lab/

4. Passwort für JupyterLab: **password**

5. Der *Strategie Analyzer* ist im Verzeichnis *TradingBot* zu finden
