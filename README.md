# Einführung in das Maschinelle Lernen
Code-Repository für den Kurs "Einführung in das Maschinelle Lernen" an der Hochschule Karlsruhe.

## Conda installieren

Der empfohlene Weg zur Einrichtung deiner Entwicklungsumgebung ist die Nutzung von Miniconda:

Lade Miniconda [hier](https://www.anaconda.com/download/success) herunter und installiere es.

## Conda einrichten

Starte unter Windows die Anwendung `Anaconda Prompt`. Öffne unter Mac oder Linux einfach ein neues Terminal-Fenster.

Die folgenden Schritte sind für beide Betriebssysteme identisch:

1. Erstelle eine neue Umgebung für diesen Kurs:

   `conda create --name ml-course python=3.11`

2. Aktiviere diese Umgebung:

   `conda activate ml-course`

3. Installiere die folgenden Pakete:

   `conda install -c conda-forge numpy pandas matplotlib scikit-learn jupyter seaborn`

4. Teste deine Installation, indem du ein neues Jupyter Notebook öffnest. Es sollte sich ein neues Browserfenster öffnen.

   `jupyter notebook`

## Code-Repository mit Git runterladen

1. Führe im Terminal folgenden Befehl aus: `git clone https://github.com/pabair/ml-kurs-ws26.git`

2. Wechsle in das Verzeichnis: `cd ml-kurs-ws26`

3. (Später) Wenn das ursprüngliche Repository aktualisiert wird, führe im Terminal `git pull` aus, um die Änderungen von GitHub auf deinen Computer zu holen.

## Alternative Einrichtung unter Linux / Windows-Subsystem für Linux (WSL)

Wenn du Conda nicht verwenden möchtest, kannst du die Pakete auch mit `pip` in einer virtuellen Umgebung installieren:

1. Erstelle eine neue virtuelle Umgebung:

   `python3 -m venv venv/`

2. Aktiviere die Umgebung:

   `source venv/bin/activate`

3. Installiere die Pakete:

   `pip install -r requirements.txt`

4. Starte das Jupyter Notebook mit `jupyter notebook .`

Anstelle von `jupyter notebook` kannst du das Projekt auch in VSCode öffnen (mit installierter Jupyter-Erweiterung), indem du im Terminal `code .` ausführst und anschließend die `venv` als Python-Interpreter für Jupyter auswählst.