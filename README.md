# SwitchBros-Updater

<p align="center">
<img src = "https://i.imgur.com/R2NRQ1g.jpg"\><br>
</p>

Eine Nintendo Switch Homebrew App um das Switch Bros. Paket, Firmwares und Cheats herunterzuladen und zu aktualisieren.

Basierend auf [kefir-updater](https://github.com/rashevskyv/kefir-updater) von [rashevskyv](https://github.com/rashevskyv) 
Original = [AiO-switch-updater](https://github.com/HamletDuFromage/aio-switch-updater) von [HamletDuFromage](https://github.com/HamletDuFromage)

## Installation
Kopiere die `switchbros-updater.nro`in den Ordner `/switch/switchbros-updater` auf deiner SD-Karte.

## Beschreibung der Funktionen
### ⬦ Switch Bros. aktualisieren
- Lade unser [Switch Bros. Basis Paket](https://github.com/Switch-Bros/Switch-Bros.-Pack/releases/tag/1.1.0) herunter. Nach dem herunterladen unseres Pakets, wird es entpackt und deine Switch in die Payload [TegraExplorer](https://github.com/suchmememanyskill/TegraExplorer/releases/) gestartet um das Paket korrekt zu installieren/aktualisieren.

### ⬦ Firmware Downloads
- Lade Firmwares in den `/firmware` Ordner runter und installiere sie mit der App DayBreak.

### ⬦ Cheat Downloads
- Herunterladen und extrahieren täglich aktualisierter Cheats. Die App extrahiert nur die Cheats von Spielen die installiert sind. Standardmäßig, überschreibt diese App vorhandene Cheats. Wenn du deine eigene Cheats hast die unverändert bleiben sollen, dann kannst du Cheat updates für bestimmte Titel in `Tools->Cheat Menü` ausstellen.
- Seit Version 2.0.0, kann aio-switch-updater Cheat Seiten von  [`CheatSlips.com`](https://www.cheatslips.com/) herunterladen. 

## Extras (im Reiter `Tools`)
- Schau nach welche Spiele Cheats besitzen.
- Starte den Internet Browser der Switch.

## Screenshots
<details><summary>Ausklappen um die Screenshots zu sehen</summary>
  
![1](https://user-images.githubusercontent.com/13203024/201618733-00a426a9-d9e6-4800-81cb-b134112241f6.jpg)
![2](https://user-images.githubusercontent.com/13203024/201618756-a42f6ae4-6f5e-438c-9421-7102212000bc.jpg)
![3](https://user-images.githubusercontent.com/13203024/201618769-8c1938e5-4773-4d92-926d-9c2b6681571d.jpg)
![4](https://user-images.githubusercontent.com/13203024/201618779-958a4b1d-3895-45ab-8d74-588dd3bec223.jpg)

</details>

## Kompilieren

<details><summary>Ausklappen um Instruktionen anzuzeigen</summary>

Du musst devkitPro und devkitARM installiert haben um dieses Projekt zu kompilieren.

Installiere die benötigten Zusatzmodule:
```bash
$ sudo (dkp-)pacman -Sy
```
```bash
$ sudo (dkp-)pacman -S  switch-glfw \
                        switch-curl \
                        switch-glm \
                        switch-mbedtls \
                        switch-zlib
```
Use [`switch-ex-curl`](https://github.com/eXhumer/switch-ex-curl) instead of `switch-curl` to use this app with an invalid SSL certificate.

Use portlibs and build with libnx provided in this repository

Repository klonen
```bash
$ git clone --recursive https://github.com/Switch-Bros/switchbros-updater.git
$ cd switchbros-updater
```

Kompilieren 
```bash
$ cd sbu-forwarder
$ make
$ cd ..
$ make
```

</details>

## Haftungsausschluss
Ich besitze, hoste oder vertreibe keine der Dateien, die mit diesem Homebrew-Tool heruntergeladen werden können. Auf Anfrage des Eigentümers werde ich die Möglichkeit, problematische Dateien herunterzuladen, sofort entfernen.

## Besonderer Dank an
- [natinusala](https://github.com/natinusala) für die Borealis Bibliothek.
- [tiansongyu](https://github.com/tiansongyu) für die Unterstützung von mehreren Sprachen und der Chinesischen Übersetzung.
- [yyoossk](https://github.com/yyoossk) für die japanische Übersetzung.
- [sergiou87](https://github.com/sergiou87) für die spanische Übersetzung.
- [pedruhb](https://github.com/pedruhb) für die brasilianische Übersetzung.
- [AD2076](https://github.com/AD2076) für die italienische Übersetzung.
- [qazrfv1234](https://github.com/qazrfv1234) für die Übersetzung in traditionellen chinesisch.
- [Team Neptune](https://github.com/Team-Neptune) dessen rcm code ich nutze.
- [fennectech](https://github.com/fennectech) dabei zu helfen die App zu testen und für seine Vorschläge.
- Iliak für cheatslips.com.

### Gefällt dir die App? Unterstütze den Original Entwickler!
- Liberapay : <a href="https://liberapay.com/HamletDuFromage/donate"><img alt="Spenden mit Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a>
- BTC: 1CoFc1bY5AHLP6Noe1zmqnJnp7ZWBxyo79
- ETH: 0xf68f568e21a15934e0e9a6949288c3ca009140ba
- CHAINLINK: 0xf68f568e21a15934e0e9a6949288c3ca009140ba
