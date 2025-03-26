# Lastenheft: Druck-It-Yourself Lichtschach

## 1. Einleitung
### 1.1 Ziel des Projekts
Das Projekt "Druck-It-Yourself Lichtschach" zielt darauf ab, ein 3D-gedrucktes Schachspiel mit interaktiver Beleuchtung zu entwickeln. Es soll eine kostengünstige, modular aufgebaute und individuell anpassbare Lösung entstehen, die sich sowohl für den Eigenbau durch 3D-Druck-Enthusiasten als auch für eine quelloffene Weiterentwicklung durch die Maker-Community eignet.

### 1.2 Zielgruppe
Die Zielgruppe des Projekts sind Schachspieler und Technikbegeisterte, die an einer modernen Interpretation des klassischen Schachspiels interessiert sind. Das Projekt soll sowohl für Anfänger als auch für Fortgeschrittene attraktiv sein und eine Vielzahl von Funktionen bieten, die über das klassische Schachspiel hinausgehen.

## 2. Anforderungen
### 2.1 Funktionale Anforderungen
- **3D-Druckbares Design**
  - Schachbrett und Figuren, werden im 3D-Druck gefertigt. Sie sollen auf handelsüblichen 3D-Druckern herstellbar sein (z.b. Bamboolabs A1)
  - Das Design soll anpassbar sein (Formen und Stil der Figuren).
- **LED-Beleuchtung pro Spielfeld**
  - Jedes der 64 Felder kann individuell beleuchtet werden.
  - Unterschiedliche Farben können zur Anzeige von Spielzügen oder Modi genutzt werden.
- **Interaktive Zughilfe**
  - Beim Anheben einer Figur werden die möglichen legalen Züge durch eine Lichtvisualisierung hervorgehoben.
- **Webinterface mit ESP32**
  - Ermöglicht die Konfiguration von Spielerfarben und Beleuchtungseinstellungen.
  - Integrierte Schachuhr zur Zeitkontrolle.
  - Aufzeichnung des Spielverlaufs zur späteren Analyse.

### 2.2 Erweiterte Funktionen
- **Spielen gegen eine KI**
  - Die KI berechnet Züge und zeigt diese per Lichtsignal auf dem Schachbrett an.
  - Der Spieler führt den KI-Zug manuell aus.
- **Briefschach-Modus**
  - Zwei gekoppelte Schachbretter ermöglichen Fernpartien über eine Web-App.
- **Alternative Spielmodi**
  - Unterstützung von Blitzschach und anderen Sonderformen.
- **Schachrätsel-Modus**
  - Vorgabe von Schachstellungen gegen die KI.
- **Soundeffekte**
  - Ausgabe von Spielgeräuschen über die Web-App oder einen integrierten Lautsprecher.
- **Lichtanimationen**
  - Kleine Animationen auf dem Spielfeld zur Darstellung von Spielereignissen.

## 3. Technische Anforderungen
- **Hardware**
  - ESP32 als Steuerzentrale für das System.
  - Adressierbare RGB-LEDs für die Beleuchtung der Spielfelder.
  - Sensorik zur Erkennung der Positionen und Bewegungen der Figuren.
  - Eigene PCB zur Reduzierung der benötigten Anschlüsse.
  - Stromversorgung über USB-C.
- **Software**
  - Webbasierte Benutzeroberfläche zur Steuerung der Schachpartie.
  - WLAN-Kommunikation zwischen ESP32 und Webinterface.
  - Algorithmische Umsetzung von Schachregeln zur Erkennung gültiger Züge.
  - Integration von KI zur Berechnung von Zügen.

## 4. Projektumfang und Modularität
- Das System soll modular aufgebaut sein, sodass einzelne Komponenten (z. B. Lichtsteuerung, KI-Integration) unabhängig weiterentwickelt oder ausgetauscht werden können.
- Offene Schnittstellen für eine mögliche Erweiterung durch die Community.
- Dokumentation für den Nachbau durch Maker und Open-Source-Entwickler.

