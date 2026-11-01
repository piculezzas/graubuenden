# Graubünden: Karte und Quiz

Interaktive Karte von Graubünden zum Üben und Wiederholen für die 5. Klasse (NMG, Lehrplan 21 GR, Zyklus 2). Die Schüler:innen entdecken die 11 Regionen und lernen Schritt für Schritt Ortschaften, Täler, Pässe, Flüsse und Berge kennen. Mit dem eingebauten Quiz können sie das Gelernte selbstständig üben.

Die ganze Anwendung steckt in **einer einzigen Datei** (`index.html`). Es braucht keinen Server, keine Installation und keine Internetverbindung zu fremden Diensten. Die Seite läuft direkt über GitHub Pages.

---

## Wochen freischalten

Welche Inhalte sichtbar sind, wird über die Adresse gesteuert. Die Stufen bauen aufeinander auf: Wer in Woche 3 ist, sieht auch alles aus Woche 1 und 2.

| Adresse | Sichtbar |
|---|---|
| `…/?woche=1` | Regionen |
| `…/?woche=2` | + Ortschaften und Täler |
| `…/?woche=3` | + Pässe |
| `…/?woche=4` | + Flüsse |
| `…/?woche=5` | + Berge (gilt auch für Woche 6) |

- Ohne Zusatz in der Adresse startet die Karte in **Woche 1**.
- Zahlen grösser als 5 werden wie Woche 5 behandelt.
- Für jede Woche kann ein eigener **QR-Code** mit der passenden Adresse erstellt werden.
- Die Freischaltung lenkt nur, sie schützt nichts: Wer die Adresse ändert, sieht mehr. Für das Üben in der Klasse reicht das aus.

Beispiel: `https://BENUTZERNAME.github.io/REPOSITORY/?woche=3`

---

## Karte

- Eine Region anklicken: Die Karte zoomt hinein und beschriftet, was in der aktuellen Woche freigeschaltet ist.
- Mit den Schaltflächen oben lassen sich Ortschaften, Täler, Pässe, Flüsse und Berge ein- und ausblenden. Die Schritte 1 bis 5 blenden die Inhalte nach und nach ein.
- Die Reliefdarstellung lässt sich ein- und ausschalten.
- Gestrichelte Symbole bedeuten: Die Lage ist geschätzt.
- Bei Flüssen zeigen die Pfeile die Fliessrichtung.

## Quiz

Mit «Quiz starten» wählen die Kinder selbst:

1. **Welche Regionen** geübt werden sollen.
2. **Was gefragt wird** (Regionen, Ortschaften, Täler, Pässe, Flüsse, Berge, je nach Woche).
3. **Wie geübt wird:**
   - Gemischt (alle Fragearten, auch Selber schreiben)
   - Antippen: «Zeig mir …»
   - Name wählen: «Wie heisst das?»
   - Selber schreiben: Name eintippen
   - Region finden: «Wo liegt …?»
4. **Wie viele Fragen:** 5, 10, 20, 30 oder alle.

Am Schluss gibt es ein Ergebnis, und falsch beantwortete Fragen können direkt nochmals geübt werden. Beim Selber-Schreiben werden kleine Tippfehler und alternative Schreibweisen toleriert. Die Auswahl wird pro Woche im Browser gemerkt und nirgends hingeschickt.

---

## Bearbeiten-Modus (nur für die Lehrperson)

Flüsse, Täler und Punkte (Ortschaften, Pässe, Berge) lassen sich direkt auf der Karte korrigieren.

1. Die Seite mit `?edit=1` öffnen, zum Beispiel `…/?edit=1`. Ohne diesen Zusatz ist der Modus für die Kinder nicht sichtbar. Die Karte startet dabei in Woche 5.
2. Oben links auf **Bearbeiten** klicken und eine Region wählen.
3. Anpassen:
   - Weisse Punkte ziehen, um Flüsse und Täler zu verändern.
   - Doppelklick auf eine Linie fügt einen Punkt ein.
   - Rechtsklick oder Umschalt+Klick auf einen Punkt löscht ihn.
   - Ortschaften, Pässe, Berge und die orangen Tal-Beschriftungen lassen sich direkt verschieben.
   - **Rückgängig** nimmt den letzten Schritt zurück.
4. **Speichern** klicken. Die Regionsgrenzen sind fest und lassen sich nicht bearbeiten.

### Speichern je nach Browser

- **Chrome und Edge:** Beim ersten Klick die eigene `index.html` im Projektordner auswählen und das Schreiben erlauben. Danach speichert jede Änderung automatisch in diese Datei.
- **Safari und Firefox:** Es erscheint ein Fenster zur Dateiauswahl (mit der Beschriftung «Hochladen», es wird aber nichts hochgeladen). Die Datei wählen, die gerade geöffnet ist. Danach wird eine fertige `index.html` heruntergeladen, die die alte Datei ersetzt.

Danach die geänderte `index.html` auf GitHub hochladen. GitHub Pages braucht danach meist ein bis zwei Minuten, bis die neue Version sichtbar ist.

**Wichtig:** Ungespeicherte Änderungen liegen nur im offenen Browser-Tab. Die Seite vorher nicht neu laden und den Tab nicht schliessen. Beim Beenden des Modus mit ungespeicherten Änderungen kommt eine Warnung.

---

## Dateien

| Datei | Inhalt |
|---|---|
| `index.html` | Karte, Quiz, Bearbeiten-Modus und alle Daten (Regionen, Orte, Täler, Pässe, Flüsse, Berge, Relief) |
| `README.md` | Diese Beschreibung |

## Datenquellen

- Grenzen: Gemeinden und Kanton (swisstopo / BFS, Stand 2024), zu den 11 Regionen zusammengefasst.
- Relief: swisstopo (swissALTI3D-Reliefschattierung).
- Die Lage der Einträge ist vereinfacht dargestellt. Flussverläufe, Täler und Punkte wurden von Hand dem Relief angepasst.

Die Nutzungsbedingungen der swisstopo-Daten gelten weiterhin. Bei einer Weitergabe bitte die Quellen angeben.

## Datenschutz

Die Seite sendet keine Daten an Dritte. Gespeichert werden nur die Quiz-Einstellungen, und zwar ausschliesslich im Browser der jeweiligen Person.
