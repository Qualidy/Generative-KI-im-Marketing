# Kapitel 16 – ChatGPT für A/B-Tests von Textvarianten

{{ progress(16) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was ein **A/B-Test** leistet – und warum KI das Ergebnis **nicht vorhersagen** kann
- Wie du eine prüfbare **Hypothese** formulierst, bevor du Varianten schreibst
- Wie du mit KI Varianten erzeugst, die sich in **genau einer Variable** unterscheiden
- Was **Stichprobengröße** und **Signifikanz** bedeuten – ohne Formeln, aber mit Zahlen
- Wie du Testergebnisse mit der **Datenanalyse** in ChatGPT auswertest und das Ergebnis prüfst
- Wie du Erkenntnisse in einem **Testlog** dokumentierst, damit das Team daraus lernt
</div>

---

## 16.1 Was ein A/B-Test leistet

Bei einem **A/B-Test** zeigst du zwei Varianten eines Textes zufällig verteilt an zwei vergleichbare Gruppen und misst, welche Variante ein vorher festgelegtes Ziel besser erreicht. Klassische Einsatzfelder im Textmarketing:

| Element | Gemessen an | Typisches Werkzeug |
|---|---|---|
| Newsletter-Betreffzeile | Klickrate (Öffnungsrate nur eingeschränkt) | E-Mail-Software mit A/B-Funktion |
| Call-to-Action-Button | Klickrate auf den Button | Webshop, Landingpage-Tool |
| Landingpage-Überschrift | Anmelderate | Landingpage-Tool, Testing-Werkzeug |
| Anzeigentext | Klickrate, Kosten pro Conversion | Werbeplattformen (Meta, Google, LinkedIn) |
| Produktbeschreibung | Warenkorbrate | Shop-System mit Testfunktion |

Die Öffnungsrate ist seit Jahren nur noch eingeschränkt aussagekräftig, weil manche E-Mail-Programme Mails automatisch vorladen und damit „Öffnungen" erzeugen, die kein Mensch ausgelöst hat. Für Betreffzeilen-Tests ist die **Klickrate** deshalb meist das verlässlichere Ziel.

KI hilft an drei Stellen: beim Formulieren der Hypothese, beim Erzeugen sauberer Varianten und bei der Auswertung. An einer Stelle hilft sie nicht: bei der Vorhersage, welche Variante gewinnt.

!!! info "Merksatz"
    Die KI kann dir sagen, welche Betreffzeile **nach Lehrbuch** besser sein müsste. Ob sie bei **deinen** 38.000 Abonnenten besser ist, sagt dir nur der Test. Genau deshalb testet man.

Auch „synthetische Personas", die du als simulierte Zielgruppe befragst (Kap. 18), ersetzen keinen Test. Sie eignen sich, um offensichtlich schwache Varianten vorab auszusortieren – nicht, um einen Gewinner zu bestimmen.

---

## 16.2 Erst die Hypothese, dann die Varianten

Der häufigste Fehler ist, zwei Texte zu schreiben und „mal zu schauen, was besser läuft". Selbst wenn eine Variante gewinnt, weißt du danach nicht, **warum** – und kannst das Ergebnis auf nichts übertragen. Eine **Hypothese** legt vorher fest, was du lernen willst.

Bewährte Form: **Wenn wir [Änderung], dann [messbare Wirkung], weil [Begründung].**

| Schwach | Stark |
|---|---|
| „Mal sehen, ob ein anderer Betreff besser ist." | „Wenn der Betreff den konkreten Nutzen nennt statt eine Stimmung, steigt die Klickrate, weil unsere Leser:innen den Newsletter vor allem für Pflegetipps abonniert haben." |
| „Wir testen einen emotionaleren Button." | „Wenn der Button ‚Kalender holen' statt ‚Jetzt anmelden' lautet, steigt die Anmelderate, weil der Nutzen sichtbar wird und das Wort ‚anmelden' nach Verpflichtung klingt." |
| „Kurz gegen lang." | „Wenn die Produktbeschreibung mit einem Anwendungsfall beginnt statt mit Materialangaben, steigt die Warenkorbrate auf Mobilgeräten, weil dort nur der erste Absatz sichtbar ist." |

Hier lohnt sich KI als Sparringspartner:

```text
Ich plane einen A/B-Test für den Fjordlicht-Newsletter (ca. 38.000
Abonnenten, Outdoor-Bekleidung). Ziel: höhere Klickrate.
Schlage 5 Hypothesen im Format "Wenn wir ..., dann ..., weil ..." vor.
Jede Hypothese ändert genau ein Element der Betreffzeile.
Bewerte je Hypothese: Wie gut ist das Ergebnis auf künftige
Newsletter übertragbar (hoch/mittel/niedrig)?
```

Die Bewertung der Übertragbarkeit ist entscheidend: Ein Test „Emoji ja oder nein" bringt ein Ergebnis, das du in jedem künftigen Newsletter anwenden kannst. Ein Test zwischen zwei völlig verschiedenen Betreffzeilen bringt einen Gewinner für genau diese eine Mail.

---

## 16.3 Varianten gezielt erzeugen: eine Variable

Wenn sich Variante A und B in Länge, Ton, Ansprache und Emoji unterscheiden, kannst du nach dem Test nicht sagen, welche Änderung gewirkt hat. Deshalb gilt: **Pro Test eine Variable.** Alles andere bleibt gleich.

| Variable | Variante A | Variante B |
|---|---|---|
| Nutzen vs. Stimmung | „Regenjacke waschen: 3 Fehler, die sie undicht machen" | „Herbst ist, wenn die Jacke wieder dran ist" |
| Frage vs. Aussage | „Wäschst du deine Regenjacke richtig?" | „So wäschst du deine Regenjacke richtig" |
| Personalisierung | „Anna, deine Jacke braucht Pflege" | „Deine Jacke braucht Pflege" |
| Zahl vs. keine Zahl | „3 Pflegetipps für den Herbst" | „Pflegetipps für den Herbst" |

KI neigt dazu, bei „Erstelle eine Variante B" gleich mehrere Dinge zu ändern. Gib deshalb ausdrücklich vor, was konstant bleibt – das ist der **Modifier** im P.R.O.M.P.T.-Framework (Kap. 5):

```text
Hier ist Betreffzeile A: "So wäschst du deine Regenjacke richtig"
Erstelle Variante B, die sich NUR in einem Punkt unterscheidet:
B formuliert als Frage statt als Aussage.
Gleich bleiben müssen: Kernaussage, Wortschatz soweit möglich,
Länge (+/- 5 Zeichen), Du-Ansprache, kein Emoji.
Liefere 3 Kandidaten für B und nenne bei jedem, ob sich außer
der Satzform noch etwas verändert hat.
```

!!! warning "Typische Falle"
    Die Selbstauskunft der KI („Es hat sich nur die Satzform geändert") ist nicht verlässlich. Prüfe selbst: Zähl die Zeichen, vergleiche Wort für Wort. Eine Variante, die zusätzlich ein starkes Wort wie „endlich" enthält, testet zwei Dinge auf einmal.

Mehr als zwei Varianten (A/B/C/D) sind möglich, brauchen aber entsprechend mehr Empfänger pro Variante. Bei Listen in der Größe von Fjordlicht ist A/B fast immer die bessere Wahl.

---

## 16.4 Test-Setup: Stichprobe und Signifikanz verständlich

Zwei Fragen musst du vor dem Start beantworten: **Wie viele Menschen brauche ich?** und **Ab wann glaube ich einem Unterschied?**

**Signifikanz** beschreibt, wie unwahrscheinlich ein beobachteter Unterschied wäre, wenn es in Wahrheit keinen gäbe. Im Marketing üblich ist ein **Signifikanzniveau von 5 Prozent**: Du akzeptierst ein Ergebnis als Unterschied, wenn ein so großer Abstand bei zwei gleich guten Varianten in weniger als 5 von 100 Fällen zufällig zustande käme. Der zugehörige Wert, den Auswertungen ausgeben, heißt **p-Wert**; liegt er unter 0,05, gilt der Unterschied als signifikant.

Wie viele Empfänger du brauchst, hängt vor allem davon ab, **wie klein der Unterschied ist, den du erkennen willst**. Für den Fjordlicht-Newsletter mit einer üblichen Klickrate von 3 Prozent (Planungswerte, gerundet, Signifikanz 5 %, Teststärke 80 %):

| Erwarteter Effekt | Klickrate B | nötige Empfänger **pro Variante** | machbar bei 38.000? |
|---|---|---|---|
| +30 % relativ | 3,9 % | ca. 6.500 | ja, mit Teilgruppe |
| +20 % relativ | 3,6 % | ca. 14.000 | ja, fast ganze Liste |
| +10 % relativ | 3,3 % | ca. 53.000 | nein |

Die Botschaft: **Kleine Unterschiede brauchen sehr große Gruppen.** Wer mit 2.000 Empfängern pro Variante testet, kann nur große Effekte sicher erkennen. Lass dir die Rechnung von der KI mit der Datenanalyse-Funktion durchführen, statt sie zu schätzen:

```text
Berechne mit Python die nötige Stichprobengröße pro Variante für
einen A/B-Test: Basis-Klickrate 3 %, erwartete Klickrate 3,6 %,
Signifikanzniveau 5 % (zweiseitig), Teststärke 80 %.
Zeige den Rechenweg in drei Sätzen für Nicht-Statistiker.
```

!!! tip "Testdauer vorher festlegen"
    Lege vor dem Start fest, wann du auswertest – etwa „7 Tage nach Versand" oder „nach 2.000 Besuchen pro Variante". Wer täglich nachschaut und bei der ersten signifikanten Zahl abbricht („Peeking"), findet häufig Unterschiede, die keine sind. Frühe Klicks kommen oft von einer besonders aktiven Teilgruppe und gleichen sich später aus.

---

## 16.5 Auswertung mit KI

Mit der **Datenanalyse** in ChatGPT (Python im Hintergrund) kannst du eine exportierte Ergebnistabelle hochladen oder einfügen und auswerten lassen. Vergleichbare Funktionen bieten Claude und Gemini; Copilot in Excel eignet sich, wenn die Daten ohnehin in Excel liegen. Wichtig: Nur aggregierte Zahlen hochladen, **keine** Empfängerlisten mit E-Mail-Adressen (Datenschutz, Kap. 4).

!!! example "Auswertung eines Betreffzeilen-Tests"
    Fjordlicht hat den Newsletter an zwei zufällige Gruppen von je 19.000 Abonnenten verschickt (fiktive Zahlen):

    ```text
    Variante;Empfänger;Klicks
    A_Aussage;19000;570
    B_Frage;19000;684
    ```

    ```text
    Werte diesen A/B-Test aus. Berechne Klickrate je Variante, den
    relativen Unterschied und prüfe mit einem Chi-Quadrat-Test, ob der
    Unterschied bei 5 % Signifikanzniveau signifikant ist.
    Erkläre das Ergebnis in 4 Sätzen für das Marketingteam.
    Nenne ausdrücklich, was wir aus diesem Test NICHT schließen können.
    ```

    Erwartbares Ergebnis: A 3,0 %, B 3,6 %, relativ +20 %, p-Wert etwa 0,001 – also signifikant. Was der Test nicht zeigt: ob Fragen generell besser funktionieren, ob mehr Klicks zu mehr Käufen führen und ob der Effekt bei anderen Themen hält.

Prüfe die Auswertung trotzdem. Zwei einfache Kontrollen genügen meist: Rechne die Klickraten selbst nach (Klicks geteilt durch Empfänger), und lass dir den verwendeten Python-Code anzeigen. Stimmen die Ausgangszahlen im Code mit deinen Daten überein?

!!! warning "Typische Falle"
    Wenn das Gesamtergebnis nicht signifikant ist, schlägt die KI gern vor, nach Segmenten zu suchen: „Bei mobilen Nutzern ist B signifikant besser!" Wer lange genug in Teilgruppen sucht, findet fast immer irgendwo einen „signifikanten" Unterschied – rein zufällig. Ein Segmentbefund aus einem Test ist eine **neue Hypothese** für den nächsten Test, kein Ergebnis.

| Auswertungsschritt | KI kann | Du prüfst |
|---|---|---|
| Raten berechnen | zuverlässig mit Python | Ausgangszahlen im Code |
| Signifikanz testen | passenden Test wählen und rechnen | ob die Fragestellung vorher festgelegt war |
| Ergebnis erklären | verständlich formulieren | ob die Erklärung über die Daten hinausgeht |
| Ursachen deuten | Vermutungen liefern | dass Vermutungen als solche markiert sind |
| Empfehlung ableiten | Vorschläge machen | ob Aufwand und Effekt in einem sinnvollen Verhältnis stehen |

---

## 16.6 Lernen dokumentieren und Grenzen kennen

Ein Test, dessen Ergebnis nur im Kopf einer Person steckt, ist nach drei Monaten vergessen. Ein **Testlog** – eine einfache Tabelle in Sheets, Excel oder Notion – macht aus Einzeltests Teamwissen.

| Feld | Beispiel |
|---|---|
| Datum, Kanal | 06.10.2026, Newsletter |
| Hypothese | Frage statt Aussage erhöht Klickrate, weil … |
| Varianten | A: „So wäschst du …" / B: „Wäschst du …?" |
| Zielmetrik, Dauer | Klickrate, 7 Tage |
| Stichprobe | je 19.000 |
| Ergebnis | A 3,0 %, B 3,6 %, p ≈ 0,001 |
| Erkenntnis | Frage-Betreff bei Ratgeber-Themen wirksam – bei Produkt-Themen noch nicht getestet |
| Nächster Schritt | Wiederholung mit Produkt-Newsletter |

KI kann das Testlog regelmäßig auswerten: „Fasse die letzten zwölf Tests zusammen. Welche Muster sind mehrfach bestätigt, welche nur einmal beobachtet?" So entstehen Regeln für eure Prompt-Bibliothek (Kap. 10) und den Styleguide – etwa „Bei Ratgeber-Newslettern Betreff als Frage". Wie du über A/B-Tests hinaus Kennzahlen auswertest, zeigt Kapitel 20.

Die Grenzen im Überblick:

- KI kann **keine Testergebnisse vorhersagen** – auch nicht mit Personas oder Benchmarks.
- Ein Gewinner gilt für **diese Zielgruppe, diesen Zeitpunkt, diesen Kanal**. Wiederhole wichtige Erkenntnisse.
- Mehr Klicks sind nicht automatisch mehr Umsatz. Sieh dir, wo möglich, auch nachgelagerte Kennzahlen an.
- Kleine Listen erlauben nur das Erkennen großer Unterschiede. Dann lieber seltener und mutiger testen.

---

## Zusammenfassung

- Ein **A/B-Test** misst, welche Variante bei **deiner** Zielgruppe besser wirkt; KI kann das Ergebnis nicht vorhersagen.
- Vor den Varianten steht eine **Hypothese** im Format „Wenn …, dann …, weil …" – sonst lernst du nichts Übertragbares.
- Varianten unterscheiden sich in **genau einer Variable**; das gehört als Modifier in den Prompt und wird selbst geprüft.
- **Kleine Effekte brauchen große Stichproben**; Testdauer und Auswertungszeitpunkt werden vorher festgelegt.
- Die **Datenanalyse** rechnet zuverlässig, aber du prüfst Ausgangszahlen, Fragestellung und Deutung – und nimmst Segmentfunde nur als neue Hypothese.
- Ein **Testlog** macht aus Einzeltests Teamwissen und liefert Regeln für Bibliothek und Styleguide.

---

## Kurzübungen

{{ task(file="tasks/k16_01.yaml") }}

{{ task(file="tasks/k16_02.yaml") }}

{{ task(file="tasks/k16_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k16.yaml") }}
