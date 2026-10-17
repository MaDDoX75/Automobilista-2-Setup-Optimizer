<img width="704" height="384" alt="AMS2SO_lg2" src="https://github.com/user-attachments/assets/b080b14c-4dc6-46ad-a3e5-5fd3bfdbc32a" />

# 🏁 Automobilista 2 Setup Optimizer

Dein Renningenieur für den zweiten Bildschirm – by MaDDoX

Der Setup Optimizer liest während der Fahrt die Telemetrie von **Automobilista 2** und sagt dir, mit welchem **Reifendruck** du ins Rennen gehen solltest. Ein paar Testrunden fahren, Empfehlung ablesen, in der Garage einstellen – fertig. Dazu kommen Spritrechner, Boxenstopp-Planer und eine Unter-/Übersteuer-Erkennung.

[![Download](https://img.shields.io/github/v/release/MaDDoX75/Automobilista-2-Setup-Optimizer?label=Download&style=for-the-badge&color=3B82F6)](https://github.com/MaDDoX75/Automobilista-2-Setup-Optimizer/releases/latest)

---

## ✨ Was das Tool kann

### 🛞 Reifen – die Hauptfunktion
- Misst **Druck und Temperatur** aller vier Reifen (innen, Mitte, außen) live
- Rechnet nach **1–2 Testrunden** aus, um wie viel du den **Kaltdruck** erhöhen oder senken musst – z. B. *„Kaltdruck SENKEN um 0,05 bar“*
- Optimiert wahlweise für das **Rennen** (Ø über die Renndistanz) oder das **Qualifying** (optimal ab der ersten schnellen Runde)
- Erfasst den eingestellten Kaltdruck automatisch in der Box und zeigt direkt den neuen Zielwert
- Merkt sich pro Auto und Strecke, was beim **letzten Mal** gepasst hat
- Rechnet auf die **Rennbedingungen** um: Asphalttemperatur im Rennen eintragen, fertig
- Abgestimmt auf die **GT3-Klasse**, Vorlagen auch für GT4, Formel/Prototyp und Straßenwagen/Cup

### ⛽ Sprit & Boxenstopps
- Verbrauch pro Runde und Minute, Reichweite, benötigte Liter für die Renndistanz
- **Boxenstopp-Manager:** Stopps automatisch oder nach Runde planen, Nachtank-Menge pro Stopp
- Live-Anzeige *„BOX AM ENDE DIESER RUNDE – 14,2 L nachtanken“*
- Startsprit vorgeben und sehen, wann du spätestens rein musst – inklusive Hinweis zum Reifenwechsel
- **Sprachansagen:** Boxenstopp-Plan vor dem Rennen, „In 3 Runden Boxenstopp, 31 Liter nachtanken“, Empfehlungen nach jeder Runde
- **Status-Ansage auf Knopfdruck** – Taste frei belegbar auf Tastatur, Lenkrad oder Buttonbox
- Warnung bei knappem Sprit per **„Box Box“-Sound** oder **Sprachansage**

### 🏎️ Fahrverhalten & Bremsen
- Erkennt **Untersteuern** und **Übersteuern** – getrennt nach Bremsen, Rollen und Gas, langsamen und schnellen Kurven – mit Setup-Tipps
- Bremstemperaturen mit Hinweisen zu den Bremskühlschächten

### 📊 Und außerdem
- Statistik aller Runden, **CSV-Export** für Excel und **Rennbericht**
- Profile **exportieren und importieren** – Setups mit Kumpels teilen, Notizen pro Strecke
- Profile pro Auto, **Großanzeige** (F11) für den zweiten Bildschirm, dunkles Design
- Kurze **Erklärungen per Tooltip** an allen Knöpfen und Eingabefeldern
- **Demo-Modus** zum Ausprobieren ohne Spiel

---

## 🚀 Schnellstart

1. **[Neueste Version herunterladen](https://github.com/MaDDoX75/Automobilista-2-Setup-Optimizer/releases/latest)** – unter *Assets* die `AMS2-Setup-Optimizer_vX.XX.exe`
2. In einen **eigenen Ordner** legen (nicht unter `C:\Programme`)
3. In AMS2: **Optionen → System → Shared Memory = „Project CARS 2“**
4. EXE starten, Session in AMS2 starten, losfahren

Keine Installation nötig – eine einzige Datei. Anleitung, Warnton und Einstellungen legt das Programm selbst daneben ab. Die ausführliche Anleitung findest du im Programm unter **„Hilfe“**.

> **Hinweis:** Beim ersten Start meldet Windows evtl. *„Der Computer wurde durch Windows geschützt“*, weil das Programm nicht digital signiert ist. Auf **„Weitere Informationen“ → „Trotzdem ausführen“** klicken.

---

## 💻 Voraussetzungen

- Windows 10 oder 11
- Automobilista 2 (Steam)
- Shared Memory in AMS2 auf **„Project CARS 2“**

---

## 🔄 Updates

Neue Versionen erscheinen unter **[Releases](https://github.com/MaDDoX75/Automobilista-2-Setup-Optimizer/releases)** – jeweils mit Changelog. Zum Aktualisieren die neue EXE in denselben Ordner legen und die alte löschen. Einstellungen und Profile bleiben erhalten.

---

## ⚖️ Rechtliches

© 2026 MaDDoX Alle Rechte vorbehalten.  
Das THC-Sim-Racing-Logo ist Eigentum von THC Sim Racing.  
The Game Central [TGC] sowie die TGC-Logos sind Eigentum von MaDDoX.

Kostenlos für die private Nutzung und unverändert weitergebbar. Verkauf oder Veröffentlichung veränderter Versionen nur mit Zustimmung des Autors. Nutzung auf eigene Gefahr – alle Empfehlungen sind berechnete Schätzwerte ohne Gewähr.

Fan-Projekt ohne Verbindung zu Reiza Studios. „Automobilista 2“ ist eine Marke von Reiza Studios. Das Programm liest nur die Telemetrie, die AMS2 über die Shared-Memory-Schnittstelle bereitstellt, und verändert nichts am Spiel.
