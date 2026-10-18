<img width="1376" height="768" alt="AMS2SO_bg" src="https://github.com/user-attachments/assets/7b37b84e-216b-467c-b038-70537428e017" />

# 🏁 Automobilista 2 Setup Optimizer

**Dein Renningenieur für den zweiten Bildschirm – by MaDDoX**

Der Setup Optimizer liest während der Fahrt die Telemetrie von **Automobilista 2** und sagt dir, mit welchem **Reifendruck** du ins Rennen gehen solltest. Ein paar Testrunden fahren, Empfehlung ablesen, in der Garage einstellen – fertig. Dazu kommen Spritrechner, Boxenstopp-Planer, Sprachansagen, Fahrverhaltens-Analyse und die Standard-Setups der GT3-Autos.

[![Download](https://img.shields.io/github/v/release/MaDDoX75/Automobilista-2-Setup-Optimizer?label=Download&style=for-the-badge&color=3B82F6)](https://github.com/MaDDoX75/Automobilista-2-Setup-Optimizer/releases/latest)

---

## ✨ Was das Tool kann

### 🛞 Reifen – die Hauptfunktion
- Misst **Druck und Temperatur** aller vier Reifen (innen, Mitte, außen) live
- Rechnet nach **1–2 Testrunden** den richtigen **Kaltdruck** aus – mit Zielwert, z. B. *„Kalt 1,58 → 1,61 bar“*
- Optimiert für das **Rennen** (Ø über die Renndistanz) oder das **Qualifying** (optimal ab der ersten schnellen Runde)
- **Rennbedingungen:** Asphalttemperatur des Rennens eintragen – das Tool rechnet die Empfehlung aus dem Training um
- Abgestimmt auf **GT3**: Ziel-Heißdruck 1,96 bar (Sweetspot laut Tests 1,95–1,97 bar), getrennte Vorlagen für **GT3 Gen2** und **GT3 Gen1** – automatisch erkannt
- Berücksichtigt die **vorgeheizten Reifen** der GT3-Gen1-Autos
- Merkt sich pro Auto und Strecke, was beim **letzten Mal** gepasst hat

### 🔧 Setup
- **Setup eintragen** – aufgebaut wie das AMS2-Setup-Menü (Reifen/Bremsen/Karosserie, Aufhängung, Antriebsstrang)
- **AMS2-Standard-Setups für 14 GT3-Autos** eingebaut – das Formular ist automatisch vorausgefüllt, du änderst nur, was du verstellt hast
- Erkennt die **Low-Downforce-Variante** der GT3-Gen2-Autos (Le Mans, Monza, Daytona)
- **Auf Standard zurücksetzen** mit einem Klick
- Jede Runde in der CSV enthält das eingetragene Setup – so lassen sich Änderungen später den Messwerten zuordnen

### ⛽ Sprit & Boxenstopps
- Verbrauch pro Runde und Minute, Reichweite, benötigte Liter für die Renndistanz
- Merkt sich den **Verbrauch pro Auto und Strecke** – warst du schon mal dort, ist der Planer sofort startklar
- **Boxenstopp-Manager:** Stopps automatisch, nach Runde oder per **Startsprit** planen, Nachtank-Menge pro Stopp, Hinweis zum Reifenwechsel
- Live-Anzeige *„BOX AM ENDE DIESER RUNDE – 14,2 L nachtanken“*
- Funktioniert auch auf langen Strecken wie **Nordschleife** und **Le Mans**
- Warnung bei knappem Sprit per **„Box Box“-Sound** oder **Sprachansage**

### 🗣️ Sprachansagen
- **Setup Report** nach jeder Runde: *„Reifendruck vorne links senken um 0,03 Bar“*, Hinweise zu Bremsen und Bremsschläuchen
- **Boxenstopp-Plan** wird vor dem Rennen vorgelesen, Ankündigung **x Minuten vorher**: *„In 2 Runden Boxenstopp, 31 Liter nachtanken“*
- **Status-Ansage auf Knopfdruck** – Taste frei belegbar auf **Tastatur, Lenkrad oder Buttonbox**

### 🏎️ Fahrverhalten & Fahrwerk
- Erkennt **Untersteuern** und **Übersteuern** – getrennt nach Bremsen, Rollen und Gas, langsamen und schnellen Kurven – mit Setup-Tipps
- Fahrstil-Einstellung **„Heck darf arbeiten“** für alle, die das Heck bewusst zum Einlenken nutzen
- **Schlupf, ABS und Traktionskontrolle** *(experimentell)*: blockierende und durchdrehende Räder, Tipps zu ABS, TC, Bremsbalance und Sperre
- Bremstemperaturen mit Hinweisen zu den Bremskühlschächten
- **Fahrwerks-Daten** in der CSV: Bodenfreiheit, Aero-Absenkung, Aufsetzer, Federweg, Dämpfer, Randsteine, Roll- und Nickwinkel, Top Speed, Kurven-g u. v. m.

### 📊 Und außerdem
- Statistik aller Runden, **CSV-Export** für Excel und **Rennbericht**
- Profile pro Auto, **exportieren und importieren** – Setups mit Kumpels teilen, Notizen pro Strecke
- **Großanzeige** (F11) für den zweiten Bildschirm, **dunkles Design** oder Windows-Standard
- **Einrichtungs-Assistent** beim ersten Start, **Tooltips** an allen Knöpfen
- **Automatische Updates** über GitHub
- **Demo-Modus** zum Ausprobieren ohne Spiel

---

## 🚀 Schnellstart

1. **[Neueste Version herunterladen](https://github.com/MaDDoX75/Automobilista-2-Setup-Optimizer/releases/latest)** – unter *Assets* die `AMS2-Setup-Optimizer_vX.XX.exe`
2. In einen **eigenen Ordner** legen (nicht unter `C:\Programme`)
3. In AMS2: **Optionen → System → Shared Memory = „Project CARS 2“**
4. EXE starten, den kurzen Einrichtungs-Assistenten durchklicken, Session in AMS2 starten, losfahren

Keine Installation nötig – eine einzige Datei. Die ausführliche Anleitung findest du im Programm unter **„Hilfe“**.

> **Hinweis:** Beim ersten Start meldet Windows evtl. *„Der Computer wurde durch Windows geschützt“*, weil das Programm nicht digital signiert ist. Auf **„Weitere Informationen“ → „Trotzdem ausführen“** klicken.

---

## 🚗 Hinterlegte Standard-Setups

| GT3 Gen2 | GT3 Gen1 |
|---|---|
| Aston Martin Vantage GT3 Evo | Audi R8 LMS GT3 |
| Audi R8 LMS GT3 evo II | BMW M6 GT3 |
| BMW M4 GT3 | McLaren 720S GT3 |
| Chevrolet Corvette Z06 GT3.R | Mercedes-AMG GT3 |
| Lamborghini Huracan GT3 EVO2 | Nissan GT-R Nismo GT3 |
| McLaren 720S GT3 Evo | Porsche 911 GT3 R |
| Mercedes-AMG GT3 Evo | |
| Porsche 992 GT3 R | |

Low-Downforce-Standard bisher für den McLaren 720S GT3 Evo – weitere folgen. Alle anderen Autos funktionieren genauso, nur ohne vorausgefülltes Standard-Setup.

---

## 💻 Voraussetzungen

- Windows 10 oder 11
- Automobilista 2 (Steam)
- Shared Memory in AMS2 auf **„Project CARS 2“**

---

## 🔄 Updates

Das Programm prüft beim Start automatisch auf neue Versionen (abschaltbar) und kann sie direkt installieren. In der Hilfe gibt es dafür auch den Knopf **„Auf Updates prüfen“**. Alle Versionen mit Changelog stehen unter **[Releases](https://github.com/MaDDoX75/Automobilista-2-Setup-Optimizer/releases)**. Einstellungen und Profile bleiben bei einem Update erhalten.

---

## ⚖️ Rechtliches

© 2026 MaDDoX · THC Sim Racing. Alle Rechte vorbehalten.  
Das THC-Sim-Racing-Logo ist Eigentum von THC Sim Racing.  
The Game Central [TGC] sowie die TGC-Logos sind Eigentum von MaDDoX.

Kostenlos für die private Nutzung und unverändert weitergebbar. Verkauf oder Veröffentlichung veränderter Versionen nur mit Zustimmung des Autors. Nutzung auf eigene Gefahr – alle Empfehlungen sind berechnete Schätzwerte ohne Gewähr.

Fan-Projekt ohne Verbindung zu Reiza Studios. „Automobilista 2“ ist eine Marke von Reiza Studios. Das Programm liest nur die Telemetrie, die AMS2 über die Shared-Memory-Schnittstelle bereitstellt, und verändert nichts am Spiel.
