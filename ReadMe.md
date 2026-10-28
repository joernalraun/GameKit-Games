# Spiele für das Calliope mini GameKit

Diese Sammlung enthält Spiele für den **Calliope mini mit der Hardwareerweiterung GameKit**.
Jedes Spiel hat ein individuelles mit Spielprinzip und dementsprechend eine eigene Steuerung.
Diese Datei beschreibt, was alle Spiele gemeinsam haben.

---

## Hardware-Voraussetzungen

| **Mikrocontroller** | Calliope mini mit **nRF52833** |
| **Speicher** | 512 KB Flash, 128 KB RAM |
| **Erweiterung** | **GameKit** mit Farbdisplay, Steuerkreuz und den Tasten **A** und **B** |
| **Display** | MakeCode-Arcade-Auflösung **160 × 120 Pixel**, 16 Farben |
| **Ton** | Piezo-Buzzer des Calliope mini |
| **Verbindung** | USB-Kabel zum Aufspielen, Stromversorgung über USB oder Batterie |

Die Spiele nutzen nur die Eingaben, die MakeCode Arcade fest vorsieht: **Steuerkreuz** (oben, unten, links, rechts) und die Tasten **A** und **B**.

---

## Mehrspieler-Spiele

| **Tennis**
| **Mini Racer**

Diese Spiele können allein oder zu zweit gespielt werden. Damit man sie zusammen spielen kann, ist es wichtig, dass man ein Jacdac-Kabel an beiden Calliope mini ansteckt. Die Verbindung läuft automatisch, sobald der zweite Calliope mini erkannt wird.

---

## Ein Spiel aufspielen

**Variante A – im Browser (ohne Installation):**
1. Hex-Datei laden
3. Den Calliope mini per USB anschließen und die `.hex`-Datei auf das Laufwerk `MINI` kopieren
4. Loslegen!

---

## Ton

Der Piezo-Buzzer des Calliope mini kann **nur einen Ton zur selben Zeit** spielen, und tiefe Töne sind sehr leise. Die Spiele berücksichtigen das:
- Musik ist **einstimmig** und eine Oktave höher gelegt, weil der Buzzer zwischen etwa 1 und 2 kHz am lautesten ist.
- Effekte **unterbrechen** die Musik kurz, statt sich mit ihr zu überlagern.
- Im Titelbild schaltet meist **B** den Ton um oder aus. Die Wahl bleibt gespeichert.

---

## Speichern

Bestwerte, Rekorde und die Ton-Einstellung speichern die Spiele im **Flash** des Calliope mini. Dafür nutzen sie die MakeCode-Funktion `settings`. Die Werte bleiben auch nach dem Ausschalten erhalten. Wird ein anderes Programm aufgespielt, können sie verloren gehen.

---

## Hinweis

Die Spiele sind im Stil bekannter Klassiker gehalten. Figuren, Grafik und Musik sind keine Kopien der Originale. Namen von Spielen und Marken gehören ihren jeweiligen Inhabern.
