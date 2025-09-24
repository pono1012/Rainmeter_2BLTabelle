# 2. Bundesliga Tabelle (Rainmeter Skin)

Ein Rainmeter-Skin, der die **aktuelle Tabelle der 2. Bundesliga** anzeigt – inklusive Vereinslogos, Punkten, Torverhältnis und Tordifferenz.  
Die Daten werden live von [OpenLigaDB](https://www.openligadb.de) geladen und automatisch an die aktuelle Saison angepasst.  

---

## Features
- 📊 **Live-Tabelle** mit Punkten, GF:GA, GD  
- 🖼️ **Automatische Logos**: Vereine werden erkannt, Logos aus `@Resources\logos\` eingebunden  
- 🔄 **Manuelles Refresh per Klick**  
- 🕔 **Automatische Aktualisierung alle 5 Minuten**  
- ⚙️ **Vollständig anpassbar** (Spaltenbreite, Schrift, Update-Intervall …)  

---

## Installation
1. [Rainmeter](https://www.rainmeter.net/) installieren (falls noch nicht vorhanden).  
2. Das `.rmskin`-Paket aus den Releases laden und per Doppelklick installieren.  
   - Enthält **JsonParser.dll** → keine extra Installation notwendig.  
3. Logos (`.png`, empfohlen 80×80 px) nach `@Resources\logos\` kopieren.  
   - Fehlt ein Logo, wird automatisch `default.png` genutzt.  

---

## Abhängigkeiten / Credits
- **Rainmeter** – Desktop-Customization-Tool  
- **JsonParser.dll** von [e2e8](https://github.com/e2e8/rainmeter-jsonparser) – zum Auslesen der OpenLigaDB-Daten  
- **OpenLigaDB API** – kostenlose Datenquelle für Fußballergebnisse  

🙏 Danke an die Entwickler dieser Komponenten – ohne sie wäre dieses Projekt nicht möglich.  

---

## Aktualisierungsintervall
Standardmäßig fragt der Skin **alle 5 Minuten (300 000 ms)** neue Daten ab.  

- Vorteil: Sehr geringe CPU-/RAM-Belastung, praktisch kein Leistungsverlust im Alltag.  
- Nach dem ersten Laden siehst du deshalb **erst nach bis zu 5 Minuten** die Tabelle.  

➡️ Wer schnellere Aktualisierungen möchte, kann in der `.ini`-Datei anpassen:  

<img width="359" height="398" alt="image" src="https://github.com/user-attachments/assets/9f6b0dc8-3eaf-4a51-8148-baf0f2286146" />


```ini
[Rainmeter]
Update=300000   ; 5 Minuten = 300000 ms


