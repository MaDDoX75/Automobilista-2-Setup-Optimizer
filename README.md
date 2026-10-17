# Automobilista 2 Setup Optimizer – v0.61
© 2026 MaDDoX · "The Game Central"

Ein Renningenieur für den zweiten Bildschirm. Das Tool liest während der Fahrt die Telemetrie von Automobilista 2 (AMS2) und hilft dir, deine Reifen im Rennen optimal zu nutzen.
---
## Wofür das Tool gedacht ist

**In erster Linie geht es um die Reifen.** Du fährst vor dem Rennen ein paar Testrunden mit dem Auto und auf der Strecke, die du im Rennen fährst. Das Tool beobachtet dabei, wie sich deine Reifen verhalten – wie warm sie werden, wie sich der Druck aufbaut und wie gleichmäßig die Lauffläche arbeitet. Daraus berechnet es, mit welchem **Reifendruck** du ins Rennen gehen solltest, damit Druck und **Temperatur** über die Renndistanz im optimalen Bereich liegen.

- **Mindestens 1–2 Testrunden** nach der Out-Lap sind nötig.
- **Je mehr Runden, desto besser:** Ab 3 Runden erkennt das Tool, wie schnell sich Druck und Temperatur stabilisieren, und die Hochrechnung auf das Rennen wird deutlich zuverlässiger.
- Das Ergebnis ist eine klare Ansage pro Reifen, z. B. „Kaltdruck SENKEN um 0,05 bar“ – genau der Wert, den du in der Garage einstellst.

**Alles andere sind Extras,** die dir im Rennen zusätzlich helfen:
**Spritrechner - Wieviel Sprit im Rennen Verbraucht wird nach den Werten deiner Testrunden
**Boxenstopp-Manager - Plane Deinen Boxenstop egal ob 1 Stop oder 10 es wird Dir alles berechnet
**Unter-/Übersteuer-Erkennung - Du erkennt Ob dein Fahrzeug über die Vorderräder schiebt oder ob dein Heck zum Ausbrechen neigt
**Bremstemperaturen - Gibt Dir Tips für deine Bremsöffnungen ob zu klein oder zu gros
**Statistik und CSV-Export
**Demo Modus

---

## Funktionen im Überblick

### Hauptfunktion: Reifen
- **Reifendruck optimieren:** Misst Druck und Temperatur aller vier Reifen (innen, Mitte, außen) und berechnet, um wie viel du den **Kaltdruck** in der Garage erhöhen oder senken sollst, damit der Heißdruck über die Renndistanz im Ziel liegt.
- **Kaltdruck automatisch erfassen:** Steht das Auto mit kalten Reifen in der Box, merkt sich das Tool den eingestellten Druck und zeigt direkt z. B. „Kalt 1,72 bar → 1,67 bar“.
- **Temperaturen:** Lauffläche live und farblich markiert, mit Min/Ø/Max über die letzten 2 Runden und Hinweisen, ob Druck oder Sturz nicht passen.
- **Profile:** merkt sich Zielwerte pro Auto und zeigt pro Auto und Strecke „Letztes Mal hier: …“ mit dem damals empfohlenen Kaltdruck.

### Extras
- **Boxenstopp-Manager:** plant die Stopps automatisch gleichmäßig oder nach deinen Vorgaben, berechnet den Sprit für jeden Stint und zeigt im Rennen live, wann du reinkommen und wie viel du nachtanken musst.
- **Spritrechner:** Verbrauch pro Runde und pro Minute, Restrunden und Restminuten, benötigte Liter für die Renndistanz. Runden unter Full Course Yellow werden herausgerechnet.
- **Warnung bei wenig Sprit:** spielt „Box Box“ oder eine Sprachansage ab.
- **Unter-/Übersteuer-Erkennung:** Abzeichen auf den Reifenkarten (vorne: Untersteuern, hinten: Übersteuern) mit Auswertung nach Bremsen, Rollen und Gas sowie Setup-Tipps.
- **Bremsen:** Temperaturen mit Hinweisen zur Bremsbelüftung.
- **Statistik und CSV-Export:** alle Runden im Überblick, Export für Excel.

---

## Voraussetzungen

- Windows 10 oder 11
- Automobilista 2 über Steam
- In AMS2: **Optionen → System → Shared Memory = „Project CARS 2“**

---

## Installation

1. Einen eigenen Ordner anlegen, z. B. `D:\AMS2 Setup Optimizer`.
2. **AMS2-Setup-Optimizer_v0.61.exe** hineinlegen (die Versionsnummer steht im Dateinamen).
3. Fertig – mehr braucht es nicht.

Beim ersten Start legt das Programm diese Dateien selbst neben der EXE ab:

| Datei | Inhalt |
|---|---|
| box_box.mp3 | Warnton bei wenig Sprit |
| README_v0.61.md | diese Anleitung (wird über „Hilfe“ angezeigt) |
| ams2_setup_optimizer.json | deine Einstellungen (beim Beenden) |
| ams2_setup_profiles.json | Profile pro Auto und Ergebnisse pro Auto und Strecke |

Im Demo-Modus kommen noch ams2_setup_optimizer_demo.json und ams2_setup_profiles_demo.json dazu. So bleiben deine echten Einstellungen und Profile von der Demo unberührt.

**Eigener Warnton:** Ersetze box_box.mp3 einfach durch eine eigene Datei mit gleichem Namen. Vorhandene Dateien überschreibt das Programm nie.

Leg den Ordner nicht unter `C:\Programme`, sonst darf das Programm dort nichts speichern.

### Update auf eine neue Version

Einfach die alte EXE durch die neue ersetzen. Einstellungen, Profile und deine MP3 bleiben erhalten, die neue README wird automatisch dazugelegt. Welche Version läuft, steht in der Titelzeile.
Da die Versionsnummer im Dateinamen steht (z. B. AMS2-Setup-Optimizer_v0.62.exe), die alte EXE danach löschen.

---

## Starten

- **Doppelklick auf AMS2-Setup-Optimizer_v0.61.exe.** Am besten vor oder während AMS2 starten – das Programm verbindet sich automatisch, sobald das Spiel läuft.
- Die Datei SharedMemory.h aus dem Spielordner wird automatisch gesucht. Findet das Programm sie nicht, nutzt es eine eingebaute Kopie. Du musst nichts einstellen.

### Demo-Modus (ohne Spiel)

Zum Ausprobieren gibt es einen Demo-Modus mit einem simulierten GT4-Auto. Gestartet wird er über den Knopf **„▶ Demo-Modus starten“** unten links im Programmfenster.

- Die Demo öffnet sich in einem **zweiten Fenster**, das normale Programm läuft weiter.
- Sie hat absichtlich Balance-Probleme eingebaut, damit du alle Anzeigen siehst.
- Sie speichert in eigene Dateien, deine echten Einstellungen und Profile bleiben unberührt.
- Zum Beenden einfach das Demo-Fenster schließen.

---

## Bedienung

### Kopfzeile

- **Live / Statistik / Profile** – zwischen Fahransicht, Rundenstatistik und Profilverwaltung umschalten
- **Immer im Vordergrund** – Fenster bleibt über anderen Fenstern
- **Einstellungen** – alle Zielwerte und Optionen
- **Großanzeige (F11)** – nur das Wichtigste in großer Schrift, ideal für den zweiten Bildschirm
- **Zurücksetzen** – Messung neu starten
- **Diagnose** – Rohwerte aus dem Spiel, Datenquelle, Zustand der Erkennung
- **Hilfe** – zeigt diese Anleitung

### Fußzeile

- **▶ Demo-Modus starten** – öffnet die Demo in einem zweiten Fenster

### Kacheln oben

Luft- und Streckentemperatur, Sprit Ø pro Runde, letzte Runde, pro Minute, Tankinhalt, wie lange der Sprit noch reicht und wie viel du für das Rennen brauchst.

### Reifenkarten

- **Drei Temperaturfelder** pro Reifen (links, Mitte, rechts der Lauffläche). Farben: dunkelblau = viel zu kalt, hellblau = etwas zu kalt, grün = im Fenster, orange = etwas zu heiß, rot = viel zu heiß.
- **Druck** in großer Schrift, daneben Luft-Innentemperatur und Verschleiß.
- **Bremse** mit Live-Temperatur und Hinweis zur Bremsbelüftung.
- **Empfehlung:** grün „Druck passt“, orange „Kaltdruck ERHÖHEN um …“, blau „Kaltdruck SENKEN um …“.
- **Kaltdruck:** eingestellter Wert und neuer Zielwert, sofern erfasst.
- **Abzeichen:** vorne orange **UNTERSTEUERN**, hinten rot **ÜBERSTEUERN**, mit Stärke in Prozent.
- Mit der Maus über eine Karte fahren zeigt alle Details als Tooltip.

### Seitenleiste

- **Profil** – erkanntes Auto, **Rennklasse** (GT3, GT4, Formel/Prototyp, Straßenwagen/Cup) zum schnellen Umstellen, Profilstatus, „Profil speichern“ und „Letztes Mal hier“.
- **Auswertung** – Anzahl gültiger Runden und Renndistanz.
- **Fahrverhalten** – Tabelle Bremsen/Rollen/Gas × langsam/schnell mit Untersteuern (US) und Übersteuern (OS) in Prozent, darunter die zwei wichtigsten Setup-Tipps.
- **Sprit** – Knopf „⛽ Boxenstopp planen …“ und alle Sprit-Werte im Detail.

---

## So optimierst du den Reifendruck

1. Renndistanz in den Einstellungen eintragen (Runden oder Minuten, z. B. 1:30 für 90 Minuten). Im Rennen übernimmt das Tool die Distanz automatisch aus der Session.
2. Auto in der Box stehen lassen, bis die Karten „Kalt … “ anzeigen können (kalte Reifen).
3. Losfahren: Out-Lap plus **mindestens 1–2 gezeitete Runden**. Je mehr Runden du fährst, desto zuverlässiger wird die Empfehlung – ab 3 Runden erkennt das Tool, wie sich Druck und Temperatur auf dieser Strecke einpendeln. Fahr dabei möglichst im Renntempo, sonst werden die Reifen nicht so warm wie im Rennen.
4. Empfehlung ablesen und den Kaltdruck in der Garage entsprechend ändern.
5. Neuer Stint, prüfen, ob jetzt „Druck passt“ angezeigt wird.

Die Zielwerte (Heißdruck, Temperaturfenster) kommen aus Vorlagen für GT3, GT4, Formel/Prototyp und Straßenwagen/Cup. **Das sind grobe Startwerte** – AMS2 veröffentlicht keine offiziellen Zielwerte. Passe sie pro Auto an, das Profil merkt sie sich.

---

## Boxenstopp-Manager

Öffnen über **„⛽ Boxenstopp planen …“** in der Seitenleiste unter Sprit.

**Voraussetzung:** Fahr zuerst 1–2 Testrunden mit dem Auto, das du im Rennen nutzt. Erst dann kennt das Programm den Verbrauch und gibt den Planer frei. Mit einer Runde ist das Ergebnis vorläufig, ab zwei Runden zuverlässig. Die Messung bleibt erhalten, wenn du vom Training ins Rennen wechselst – nur bei einem **Autowechsel** werden Messung und Plan gelöscht.

**Eingaben** (das meiste ist vorausgefüllt):
- **Renndistanz (Runden)** – aus den Einstellungen bzw. der Session. Bei Zeitrennen aus deiner Ø Rundenzeit geschätzt.
- **Anzahl Stopps** – 0 bis 5.
- **Aufteilung:**
  - **Automatisch (gleichmäßig):** Die Stopps werden gleichmäßig verteilt, z. B. bei 2 Stopps nach etwa einem und zwei Dritteln des Rennens.
  - **Manuell (Runden vorgeben):** Du trägst selbst ein, nach welcher Runde du jeweils reinkommst, z. B. Stopp 1 nach Runde 4, Stopp 2 nach Runde 10.
- **Verbrauch je Runde** – der gemessene Wert, darf überschrieben werden (z. B. etwas mehr als Puffer).
- **Reserve je Stint** – Sicherheit in Runden, Standard 1 Runde.
- **Tankgröße** – aus dem Spiel.

**Ergebnis:** Eine Tabelle mit jedem Stint: Runden, benötigter Sprit, **Start-Tankmenge** bzw. **wie viel beim Stopp nachgetankt werden muss** und der Tankinhalt danach. Passt ein Stint nicht in den Tank oder reichen die Stopps nicht, gibt es eine Warnung samt Mindestanzahl Stopps.

**„Plan übernehmen“** aktiviert die Live-Anzeige über den Reifenkarten:
- „⛽ Stopp 1 von 2 nach Runde 7 (noch 3 Rd) · nachtanken ≈ 14,2 L“
- „⛽ BOX AM ENDE DIESER RUNDE · 14,2 L nachtanken“
- Reicht der Sprit nicht bis zum Stopp, wird die Zeile rot.

Die Nachtank-Menge rechnet sich im Rennen laufend mit deinem echten Verbrauch und Tankinhalt neu – fährst du sparsamer, musst du weniger tanken. Genau diesen Wert trägst du in AMS2 im Boxenmenü ein.

---

## Unter- und Übersteuern

- **Untersteuern:** Das Auto schiebt über die Vorderräder und lenkt weniger ein, als du lenkst.
- **Übersteuern:** Das Heck kommt, das Auto dreht stärker ein als gewollt.

Das Tool kalibriert sich pro Auto selbst: Fahr ein paar Kurven mit sanftem Lenken, bis „KALIBRIERE x/80“ verschwindet. Die Kalibrierung wird im Profil gespeichert. Ausgewertet wird nur in echten Kurven (ab ca. 0,4 g Querbeschleunigung).

Empfindlichkeit (Niedrig/Mittel/Hoch) und die Grenze zwischen langsamen und schnellen Kurven stellst du in den Einstellungen ein. Die Setup-Tipps sind Ansätze, keine Garantie – ändere immer nur eine Sache auf einmal.

---

## Profile

Für jedes Auto, das du fährst, legt das Programm automatisch ein Profil an. Die **Rennklasse** wird dabei aus der Fahrzeugklasse erkannt und kann links in der Seitenleiste jederzeit geändert werden – dabei werden die passenden Startwerte geladen.

Im Reiter **Profile** siehst du links alle gespeicherten Autos. Für das markierte Auto stehen rechts:
- **Rennklasse, Zieldrücke, Reifen- und Bremsenfenster** und ob die Unter-/Übersteuer-Erkennung schon kalibriert ist.
- **Ergebnisse pro Strecke:** Datum, Reifenmischung, Streckentemperatur, Runden, eingestellter und empfohlener Kaltdruck (VL · VR · HL · HR) und ob der Druck gepasst hat.

Knöpfe:
- **Werte für aktuelles Auto übernehmen** – z. B. um die Werte eines ähnlichen Autos als Start zu nehmen.
- **Kalibrierung Fahrverhalten löschen** – nach großen Setup-Änderungen an der Lenkung.
- **Profil löschen** – löscht das Profil samt allen Ergebnissen dieses Autos (mit Rückfrage).
- **Markiertes Ergebnis löschen** – entfernt einen einzelnen Eintrag, z. B. einen verunglückten Test.

---

## Statistik und CSV-Export

- Reiter **Statistik**: Zusammenfassung (Runden, beste und Ø Runde, Ø Sprit, Unter-/Übersteuern, Stints) und Tabelle aller Runden.
- **Alle Runden als CSV speichern …** fragt nach dem Speicherort.
- **Jede Runde automatisch mitschreiben** fragt einmal nach einer Datei und hängt danach jede fertige Runde an.
- Die CSV ist für das deutsche Excel formatiert (Semikolon, Dezimalkomma). Ist sie in Excel geöffnet, versucht das Tool es automatisch erneut.

---

## Einstellungen

- **Spalte 1:** Reifen (Vorlage, Druckeinheit, Zieldrücke vorne/hinten, Temperaturfenster, Optimieren für Ø oder Rennende) und Automatik (Renndistanz aus Session, automatisch neu messen bei Wechsel von Auto, Strecke, Session oder Reifenmischung).
- **Spalte 2:** Bremsenfenster, Fahrverhalten (Empfindlichkeit, schnell ab km/h, Kalibrierung neu starten) und Datenquelle (SharedMemory.h automatisch, aus Datei oder eingebaut).
- **Spalte 3:** Rennen und Sprit (Distanz, Einheit, Extrarunden) und Warnung (ab wie vielen Minuten, Audiodatei oder Sprachausgabe, Ansage Bayrisch/Hochdeutsch/eigener Text, Stimme, Test).

In eigenen Ansagen wird **{min}** durch die Restminuten ersetzt. Die Windows-Sprachausgabe liest bayrische Texte mit hochdeutscher Aussprache – für echten Dialekt den Spruch selbst als MP3 aufnehmen.

---

## Problemlösung

- **Keine Daten, obwohl AMS2 läuft:** In AMS2 Shared Memory auf „Project CARS 2“ stellen und eine Session starten (im Hauptmenü gibt es keine Daten).
- **Warnung „Shared-Memory-Version passt nicht“:** Nach einem AMS2-Update unter Einstellungen → Datenquelle → „Datei wählen …“ die neue SharedMemory.h aus dem Spielordner nehmen (Steam → Rechtsklick auf AMS2 → Verwalten → Lokale Dateien durchsuchen → Support → SharedMemory).
- **Druck wird falsch angezeigt:** Unter Diagnose den Rohwert prüfen. In der Datei ams2_setup_optimizer.json den Eintrag „raw_pressure_unit“ auf bar, psi oder kpa setzen (Programm vorher beenden).
- **Kein Warnton:** Unter Einstellungen → Warnung bei wenig Sprit mit „▶ Warnung jetzt testen“ prüfen. Direkt unter der Sounddatei steht, ob die Datei gefunden wurde. Ist box_box.mp3 neben der EXE gelöscht worden, legt das Programm sie beim nächsten Start neu an. Unter Diagnose steht, welche Sounddatei verwendet wird.
- **„Kaltdruck unbekannt“:** Der Stint muss mit kalten Reifen aus der Box starten. Nach einem Stopp mit heißen Reifen zeigt das Programm nur die Änderung („um X erhöhen/senken“).
- **Unter-/Übersteuern zeigt nichts:** Erst nach der Kalibrierung („KALIBRIERE x/80“ muss verschwinden). Sonst unter Einstellungen → Fahrverhalten die Empfindlichkeit auf „Hoch“ stellen.
- **CSV lässt sich nicht schreiben:** Die Datei ist vermutlich in Excel geöffnet. Excel schließen – das Programm schreibt automatisch nach.
- **Virenscanner meldet die EXE:** bekannter Fehlalarm bei selbst erstellten Programmen. Den Ordner als Ausnahme eintragen.
- **Fehlermeldung beim Start:** Screenshot machen und an den Entwickler schicken, zusammen mit dem Inhalt aus „Diagnose“.

---

## Changelog

### v0.61
- Ende der Beta-Phase: Versionsnummern ab jetzt ohne „b“
- Neuer Reiter „Profile“: alle gespeicherten Autos mit Werten und Ergebnissen pro Strecke, Profile und einzelne Ergebnisse löschbar, Werte auf das aktuelle Auto übertragbar
- Rennklasse direkt in der Seitenleiste wählbar

### v0.60b
- Reiter heißen jetzt „Live“ und „Statistik“ und werden vollständig angezeigt

### v0.59b
- Fehlerbehebung: v0.58b startete nicht
- README überarbeitet: Schwerpunkt Reifen, Demo-Modus über den Knopf im Programm

### v0.58b
- Neuer Boxenstopp-Manager: Stopps automatisch gleichmäßig oder manuell nach Runde planen, Sprit je Stint und Nachtank-Mengen, Warnung wenn der Tank nicht reicht
- Live-Anzeige des nächsten Stopps mit aktueller Nachtank-Menge („BOX AM ENDE DIESER RUNDE“)
- Freigabe erst nach 1–2 Testrunden; Messung und Plan werden nur bei einem Autowechsel zurückgesetzt

### v0.57b
- Warnton-Einstellungen übersichtlicher: „Andere Datei …“ zum Auswählen, darunter eine Anzeige, ob die MP3 gefunden wurde, und der Knopf „▶ Warnung jetzt testen“
- Je nach Ausgabe (Audiodatei oder Sprachausgabe) sind nur die passenden Felder aktiv

### v0.56b
- Nur noch eine Datei: Warnton (box_box.mp3) und Anleitung sind in der EXE enthalten und werden beim Start automatisch abgelegt
- Knopf „Demo-Modus starten“ unten links – die Demo läuft in einem zweiten Fenster mit eigenen Einstellungen

### v0.55b
- Ein kleines Gimmick unten rechts im Fenster. Ausprobieren auf eigene Gefahr 😉

### v0.54b
- README mit Bedienungsanleitung (für die EXE-Version) und Changelog
- Knopf „Hilfe“ in der Kopfzeile zeigt die README direkt im Tool an

### v0.53b
- Neuer Reiter „Statistik“ mit Zusammenfassung und Rundentabelle
- CSV-Export mit Speichern-Dialog und automatisches Mitschreiben jeder Runde
- Warnung wahlweise per Windows-Sprachausgabe (Bayrisch, Hochdeutsch oder eigener Text, Stimme wählbar)
- Einstellungen in drei Spalten

### v0.52b
- App-Icon und Logo (THC Sim Racing)
- Gründlichere Suche nach der SharedMemory.h (Registry, alle Steam-Bibliotheken, alle Laufwerke)
- Eingebaute SharedMemory.h als Rückfall – das Tool startet immer
- Datenquelle in den Einstellungen wählbar, Warnung bei abweichender Shared-Memory-Version

### v0.51b
- Neuer Name „Automobilista 2 Setup Optimizer“ (vorher „AMS2 Reifen-Tool“)
- Fortlaufende Versionsnummer
- Neue Datei- und Konfigurationsnamen, alte Einstellungen und Profile werden übernommen

### v0.5b
- Unter-/Übersteuer-Erkennung mit Selbstkalibrierung, Abzeichen auf den Reifenkarten und Setup-Tipps
- Profile pro Auto, „Letztes Mal hier“ pro Auto und Strecke, Erfassung des Kaltdrucks
- Dunkles Design ohne Scrollbalken, Einstellungen im eigenen Fenster, Großanzeige
- Warnton als MP3 (box_box.mp3)

### Vor v0.5b (Entwicklung)
- Erste Versionen als Prototyp, danach als eigenständige EXE
- Reifendruck-Empfehlung mit Hochrechnung auf die Renndistanz
- Getrennte Zieldrücke vorne/hinten, Vorlagen GT3, GT4, Formel/Prototyp, Straßenwagen/Cup
- Spritrechner mit Extrarunden, Liter pro Minute, Restminuten, FCY-Erkennung
- Lauffläche- und Bremstemperaturen mit Min/Ø/Max
- Renndistanz automatisch aus der Session, automatisches Zurücksetzen bei Wechsel
- „Immer im Vordergrund“ und Großanzeige

## Über das Programm

**Automobilista 2 Setup Optimizer**
Entwickelt von MaDDoX für THC Sim Racing.
Version 0.61 · Oktober 2026

© 2026 MaDDoX · THC Sim Racing. Alle Rechte vorbehalten.
Das THC-Sim-Racing-Logo ist Eigentum von THC Sim Racing.

## Rechtliches

**Nutzung:** Das Programm darf kostenlos privat genutzt und unverändert
weitergegeben werden. Verkauf oder Veröffentlichung veränderter Versionen
nur mit Zustimmung des Autors.

**Keine Gewähr:** Die Nutzung erfolgt auf eigene Gefahr. Die Empfehlungen
zu Reifendruck, Sprit und Setup sind berechnete Schätzwerte ohne Garantie
auf Richtigkeit – im Zweifel gilt immer, was im Spiel passiert.

**Kein offizielles Produkt:** Dieses Programm ist ein Fan-Projekt und steht
in keiner Verbindung zu Reiza Studios. „Automobilista 2“ ist eine Marke
von Reiza Studios. Das Programm liest nur die Telemetrie, die AMS2 über die
Shared-Memory-Schnittstelle bereitstellt, und verändert nichts am Spiel.

**Kontakt:**
E-Mail: towi@thegamecentral.de
Website:www.TheGameCentral.de

# Automobilista 2 Setup Optimizer – v0.61

© 2026 MaDDoX · THC Sim Racing [THC]

