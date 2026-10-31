# Kleine Farm

Ein kleines Farmspiel – allein oder zusammen mit Freunden. Hier gibt es die fertigen Spieldateien zum Testen.

**Download:** unter [Releases](../../releases/latest) die passende Datei herunterladen.

## Windows

1. `kleineFarm-…-windows-setup.exe` herunterladen und starten.
2. Windows warnt eventuell („Der Computer wurde durch Windows geschützt“), weil das Spiel nicht signiert ist:
   auf **Weitere Informationen** und dann **Trotzdem ausführen** klicken.
3. Installieren (keine Adminrechte nötig), danach liegt „Kleine Farm“ im Startmenü und auf Wunsch auf dem Desktop.

Ohne Installer: `kleineFarm-…-windows.zip` entpacken und `kleineFarm.exe` starten.

## Linux

```
tar xzf kleineFarm-*-linux.tar.gz
cd kleineFarm
./installieren.sh
```

Danach steht „Kleine Farm“ im Anwendungsmenü. Entfernen: `~/.local/share/kleineFarm/installieren.sh --weg`.

## Updates

Beim Start schaut das Spiel nach, ob es eine neue Version gibt, lädt sie (nur ein paar MB) und startet neu.
Im Hauptmenü des Spiels steht unter dem Titel die Version. Ohne Internet startet das Spiel einfach mit der vorhandenen Version.

Spielstände bleiben bei Updates und beim Neuinstallieren erhalten. Sie liegen hier:

- Windows: `%APPDATA%\Godot\app_userdata\kleineFarm\saves`
- Linux: `~/.local/share/godot/app_userdata/kleineFarm/saves`

## Zusammen spielen

Alle brauchen **dieselbe Version** (einfach alle das Spiel einmal neu starten, dann ist jeder aktuell).

- **Im selben Netzwerk:** einer wählt „Spiel hosten“, die anderen finden das Spiel unter „Spiel beitreten“.
- **Übers Internet** gibt es zwei Wege:
  - **Einfach:** alle installieren [Tailscale](https://tailscale.com) (kostenlos) und melden sich im selben Netz an.
    Beim Beitreten die Tailscale-Adresse des Hosts eingeben (beginnt meist mit `100.`).
  - **Mit Router:** der Host leitet im Router den **UDP-Port 24565** auf seinen PC weiter. Die anderen geben beim
    Beitreten seine öffentliche IP-Adresse ein (z. B. von wieistmeineip.de).

## Fehler gefunden?

Einfach Bescheid sagen – am besten mit Version, was du gemacht hast und einem Screenshot.
