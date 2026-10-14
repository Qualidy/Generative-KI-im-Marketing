# Kapitel 2 – Generative KI: Chancen und Grenzen

{{ progress(2) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Bei welchen Aufgaben **generative KI** im Marketing wirklich stark ist – und warum
- Was **Halluzinationen** sind, wie sie entstehen und wie du sie im Alltag abfängst
- Wie **Bias** in Trainingsdaten zu Stereotypen in Texten und Bildern führt
- Warum der **Wissensstand** eines Modells begrenzt ist und was **Websuche** daran ändert – und was nicht
- Warum Ergebnisse **nicht konsistent** sind und wie du trotzdem eine einheitliche Markenstimme erreichst
- Welche Grundregeln für **Datenschutz und Vertraulichkeit** ab dem ersten Prompt gelten
</div>

---

## 2.1 Die Stärken: wofür generative KI gebaut ist

Aus Kapitel 1 weißt du: Ein Sprachmodell berechnet, welche Fortsetzung eines Textes wahrscheinlich ist. Das klingt nach einer Einschränkung, erklärt aber zugleich seine Stärken. Alles, was mit **Sprache, Form und Variation** zu tun hat, gelingt gut – weil das Modell Milliarden Beispiele dafür gesehen hat.

| Stärke | Warum sie funktioniert | Beispiel bei Fjordlicht |
|---|---|---|
| **Entwürfe und Rohfassungen** | Textmuster aller Gattungen sind gelernt | erster Entwurf für einen Blogartikel in „Draußen-Notizen" |
| **Varianten erzeugen** | Variation ist eingebaut | 15 Betreffzeilen für den Herbstnewsletter |
| **Umformen** | Inhalt bleibt, Form ändert sich | Blogartikel → LinkedIn-Post für Fjordlicht Business |
| **Zusammenfassen und Strukturieren** | Kernaussagen erkennen ist ein Sprachmuster | 300 Kundenbewertungen zu Themenclustern verdichten |
| **Ideen und Perspektiven** | breites Allgemeinwissen, schnelle Assoziation | Themenideen für den Redaktionsplan im Winter |
| **Übersetzen und Lokalisieren** | mehrsprachiges Training | Produkttexte für den niederländischen Markt |

Gemeinsam ist diesen Aufgaben: Das Ergebnis lässt sich **schnell beurteilen** und ein Fehler ist **günstig**. Ein schwacher Betreffzeilen-Vorschlag kostet zwei Sekunden Lesezeit. Genau dort liegt der realistische Nutzen – nicht im „Knopf, der die Kampagne macht", sondern im schnellen ersten Entwurf, den eine Fachperson verbessert. Welche Einsatzfelder sich daraus entlang der Customer Journey ergeben, zeigt Kapitel 3.

!!! info "Merksatz"
    Generative KI ist stark, wo **Form** zählt, und schwach, wo **Wahrheit** zählt. Je leichter du ein Ergebnis prüfen kannst und je billiger ein Fehler ist, desto besser eignet sich die Aufgabe.

---

## 2.2 Halluzination: überzeugend falsch

Als **Halluzination** bezeichnet man Aussagen, die sprachlich einwandfrei und selbstsicher formuliert, inhaltlich aber erfunden sind. Das ist kein seltener Defekt, sondern eine direkte Folge der Funktionsweise: Das Modell wählt, was **plausibel klingt**. Ob eine Studie existiert, eine Zahl stimmt oder ein Zertifikat vorliegt, prüft es dabei nicht.

Besonders häufig halluziniert werden:

- **Zahlen und Statistiken** („73 % der Outdoor-Fans achten auf Nachhaltigkeit")
- **Quellen und Zitate** – Studien, Autorinnen, Links, die es nicht gibt
- **Produkteigenschaften** – Materialien, Zertifikate, Testergebnisse
- **Nischenwissen** – lokale Ereignisse, interne Regelungen, kleine Unternehmen
- **Aktuelles** – Dinge nach dem Wissensstand des Modells (Abschnitt 2.4)

Warum sagt das Modell nicht einfach „Das weiß ich nicht"? Zum einen gibt es im Modell keine Stelle, an der „Wissen" und „Nichtwissen" sauber getrennt wären – es gibt nur mehr oder weniger wahrscheinliche Fortsetzungen. Zum anderen wurde es in der Feinabstimmung darauf trainiert, hilfreich zu antworten. Neuere Modelle räumen Unsicherheit zwar häufiger ein als frühere, aber verlassen kannst du dich darauf nicht. Gefährlich sind deshalb nicht die offensichtlich falschen Antworten, sondern die **fast richtigen**: Ein Text mit neun korrekten Angaben und einer erfundenen Zahl wirkt insgesamt glaubwürdig.

!!! warning "Typische Falle: Greenwashing per Halluzination"
    Du lässt einen Produkttext für das Fleece „Skog" schreiben und lieferst nur Name und Preis. Der Entwurf lobt „Fair-Trade-zertifizierte Produktion" und „klimaneutralen Versand". Beides klingt nach Fjordlicht, ist aber nirgends belegt. Für eine Marke, die nur belegbare Nachhaltigkeitsaussagen macht, ist das kein Schönheitsfehler: Unbelegte Umweltaussagen können als **irreführende Werbung** abgemahnt werden und beschädigen Vertrauen.

Gegenmittel, die sofort wirken:

```text
Nutze ausschließlich die Fakten im Abschnitt FAKTEN.
Erfinde keine Eigenschaften, Zahlen, Zertifikate oder Nachhaltigkeitsaussagen.
Wenn dir eine Angabe fehlt, schreibe [FEHLT] statt zu raten.

FAKTEN:
[Produktdaten einfügen]
```

Diese Anweisung senkt das Risiko deutlich, beseitigt es aber nicht. Deshalb gehört zu jedem veröffentlichten Text ein **Faktencheck**: Jede Zahl, jeder Claim, jede Quelle wird gegen eine verlässliche Quelle geprüft. Wie du das systematisch machst, vertiefen Kapitel 9 (Fehleranalyse) und Kapitel 15 (Faktencheck und Quellen).

---

## 2.3 Bias: die Schieflage der Trainingsdaten

Ein Modell lernt aus Texten und Bildern, die Menschen erzeugt haben – samt ihrer Klischees. **Bias** (Verzerrung) zeigt sich, wenn bestimmte Gruppen, Rollen oder Lebensentwürfe systematisch einseitig dargestellt werden.

| Wo Bias auftaucht | Beispiel | Risiko im Marketing |
|---|---|---|
| Personas und Zielgruppen | „Die typische Outdoor-Kundin" ist jung, schlank, sportlich | Zielgruppen 40+ oder Familien werden übersehen |
| Rollenbilder | Bei „Bergführer" entsteht ein Mann, bei „Familienplanerin" eine Frau | Kampagne wirkt altmodisch oder ausgrenzend |
| Bildgenerierung | „Familie beim Wandern" zeigt fast immer dieselbe Konstellation | fehlende Vielfalt, Kritik in den Kommentaren |
| Sprache und Kultur | englischsprachige Perspektive dominiert | Formulierungen und Beispiele passen nicht zum deutschen Markt |

Bias ist schwer zu erkennen, weil das Ergebnis „normal" aussieht – es entspricht ja dem Durchschnitt. Hilfreich sind drei Gewohnheiten: Zielgruppen **konkret** beschreiben statt das Modell raten zu lassen; Ergebnisse gezielt fragen „Wer fehlt hier?"; bei Personas und Bildern bewusst Vielfalt vorgeben. Vertieft wird das bei Kundenavataren (Kap. 18) und bei Bild-KI (Kap. 34).

!!! tip "Gegenprobe mit einem Satz"
    Hänge an Zielgruppen- oder Persona-Ergebnisse an: „Prüfe deine Antwort auf Stereotype zu Alter, Geschlecht, Herkunft und Körperbild. Nenne, welche Gruppen fehlen, und schlage eine ausgewogenere Fassung vor." Das ersetzt nicht dein Urteil, macht aber blinde Flecken sichtbar.

---

## 2.4 Wissensstand und Websuche

Jedes Modell hat einen **Wissensstand** (englisch „knowledge cutoff"): Ereignisse nach Abschluss des Trainingsmaterials kennt es nicht aus sich selbst heraus. Zwischen Wissensstand und Veröffentlichung liegen meist Monate. Ein Modell kann also nichts über die neue Kollektion der Konkurrenz, eine Gesetzesänderung von letzter Woche oder einen aktuellen Social-Media-Trend wissen.

Werkzeuge wie ChatGPT, Gemini, Copilot oder Perplexity können deshalb das **Web durchsuchen**. Technisch heißt das: Suchergebnisse werden ins Kontextfenster geladen, und das Modell formuliert seine Antwort auf dieser Grundlage – meist mit Quellenangaben. Für ausführlichere Recherchen gibt es Funktionen wie **Deep Research**, die viele Quellen nacheinander auswerten und einen Bericht erstellen (Kap. 17).

| | Ohne Websuche | Mit Websuche |
|---|---|---|
| Aktualität | bis zum Wissensstand | aktuell, soweit gefundene Seiten aktuell sind |
| Quellen | keine oder erfundene | verlinkte Quellen, nachprüfbar |
| Typischer Fehler | veraltete oder erfundene Fakten | falsch zusammengefasste oder schwache Quellen |
| Was du tust | Aktuelles selbst mitliefern | Quellen öffnen und Kernaussage gegenlesen |

Ob ein Werkzeug gerade sucht, erkennst du meist an einem Hinweis wie „Suche im Web" und an den Quellenangaben unter der Antwort. Fehlen diese, stammt die Antwort aus dem Training. Bei Recherchefragen lohnt es sich, die Suche ausdrücklich anzufordern und die Quellenlage gleich mitbewerten zu lassen:

```text
Recherchiere im Web, welche Kennzeichnungsregeln Instagram aktuell für
KI-generierte Bilder vorsieht. Nenne zu jeder Aussage die Quelle mit Datum.
Bevorzuge offizielle Seiten des Anbieters. Kennzeichne, wo die Quellenlage
unklar oder widersprüchlich ist.
```

!!! warning "Typische Falle"
    Eine Quellenangabe wirkt wie ein Gütesiegel. Tatsächlich kommt es vor, dass die verlinkte Seite die Aussage gar nicht enthält, eine Zahl falsch übernommen wurde oder die Quelle selbst unseriös ist. **Ein Link ist ein Prüfauftrag, kein Beweis.**

---

## 2.5 Konsistenz: jedes Mal ein bisschen anders

Weil Sprachmodelle Token mit etwas Zufall wählen, liefert derselbe Prompt nicht zweimal denselben Text. Für Ideen ist das ein Vorteil. Für Markenarbeit ist es ein Problem: Wenn fünf Personen im Team jeweils „schreib was im Fjordlicht-Stil" eingeben, entstehen fünf verschiedene Fjordlicht-Stile.

Hinzu kommen drei weitere Quellen von Inkonsistenz:

- **Lange Chats:** Vorgaben vom Anfang verblassen im Kontextfenster (Kap. 1).
- **Modellwechsel:** Anbieter tauschen Modelle regelmäßig aus. Ein Prompt, der im Frühjahr gut funktionierte, kann im Herbst anders reagieren. Ein Beispiel: Seit Oktober 2026 arbeitet ChatGPT mit einer neuen Modellgeneration.
- **Unterschiedliche Werkzeuge:** Claude, Gemini und ChatGPT interpretieren denselben Prompt verschieden.

Konsistenz entsteht deshalb nicht durch Hoffen, sondern durch **festgeschriebene Vorgaben**: eine kurze Beschreibung der Markenstimme, zwei bis drei echte Beispieltexte, eine Liste verbotener Formulierungen. Diese Vorgaben gehören in eine gemeinsame Prompt-Bibliothek (Kap. 10) oder dauerhaft in ein Projekt bzw. einen Assistenten (Kap. 7 und 23).

!!! example "Vorher/Nachher: Markenstimme festschreiben"
    Vorher, bei jeder Person anders:

    ```text
    Schreib einen Post im Fjordlicht-Stil über Herbstwanderungen.
    ```

    Nachher, für alle im Team gleich:

    ```text
    Markenstimme Fjordlicht: ruhig, ehrlich, naturverbunden, leicht
    nordisch-trocken. Du-Ansprache. Keine Superlative, keine Ausrufezeichen,
    keine Nachhaltigkeitsaussagen ohne Beleg.
    Beispiele für den Ton:
    [Beispielpost 1]
    [Beispielpost 2]
    Aufgabe: Schreibe einen Instagram-Post (maximal 80 Wörter) über
    Herbstwanderungen im Münsterland.
    ```

---

## 2.6 Datenschutz und Vertraulichkeit

Alles, was du in einen Prompt schreibst oder hochlädst, verlässt das Unternehmen und landet beim Anbieter. Bei kostenlosen und privaten Konten kann es – je nach Einstellung – auch zum Training künftiger Modelle verwendet werden. Für Marketing ist das besonders heikel, weil hier viele **personenbezogene Daten** anfallen: Newsletter-Listen, CRM-Exporte, Bewertungen mit Namen, Gewinnspiel-Teilnahmen.

Drei Grundregeln gelten ab dem ersten Prompt:

1. **Keine personenbezogenen Daten in private oder kostenlose KI-Konten.** Kundendaten nur in freigegebene Business- oder Enterprise-Tarife mit Auftragsverarbeitungsvertrag (AVV), in denen Eingaben nicht zum Training genutzt werden.
2. **Datenminimierung:** Gib nur das ein, was für die Aufgabe nötig ist. Für eine Sentiment-Analyse von Bewertungen braucht das Modell den Text, nicht Name und E-Mail-Adresse.
3. **Vertrauliches bleibt draußen:** unveröffentlichte Kampagnen, Preiskalkulationen, Vertragsdetails mit Partnern – es sei denn, die Nutzung ist im Unternehmen ausdrücklich freigegeben.

In der Praxis heißt das oft: erst aufbereiten, dann prompten. Wer 500 Kundenbewertungen auswerten will, entfernt vorher in der Tabelle die Spalten mit Namen, E-Mail-Adresse und Bestellnummer und lädt nur Bewertungstext, Sternezahl und Produkt hoch. Das Ergebnis der Auswertung ist dasselbe, das Risiko deutlich kleiner. Achte auch auf versteckte Personenbezüge im Freitext selbst, etwa „Ich bin Frau Meier aus Telgte und habe am Montag angerufen" – solche Stellen werden vor dem Upload geschwärzt oder durch Platzhalter ersetzt.

Eine praktische **Ampel** für Daten im Prompt, die Grundzüge der DSGVO und den EU AI Act behandelt Kapitel 4. Die Rechte am KI-Output selbst sind Thema von Kapitel 39.

---

## 2.7 Was KI gut kann, was nicht – die Übersicht

Fasst man die Grenzen zusammen, ergibt sich ein einfaches Raster für die Frage, wie viel du einer KI überlassen kannst:

| Kategorie | Typische Aufgaben | Umgang |
|---|---|---|
| **Gut delegierbar** | Ideen, Varianten, Rohentwürfe, Umformulieren, Kürzen, Gliedern | kurz prüfen, auswählen, verbessern |
| **Mit Prüfung** | Produkttexte, Zusammenfassungen, Übersetzungen, Recherche mit Quellen | Fakten und Ton gegen Quellen und Styleguide prüfen |
| **Nur mit Expertise** | Rechtliche Hinweise, Nachhaltigkeitsclaims, Zahlenauswertungen, Krisenkommunikation | Fachperson verantwortet Inhalt, KI höchstens als Entwurf |
| **Nicht delegieren** | finale Freigabe, Entscheidungen über Menschen, Umgang mit vertraulichen Kundendaten in ungeprüften Tools | bleibt beim Menschen |

!!! info "Merksatz"
    KI beschleunigt die Arbeit, sie übernimmt nicht die Verantwortung. Je größer die Reichweite und je höher die Fehlerfolgen, desto gründlicher die Prüfung – ein Newsletter an 38.000 Empfänger braucht mehr Sorgfalt als ein Brainstorming im Team.

---

## Zusammenfassung

- Generative KI ist stark bei **Entwürfen, Varianten, Umformen, Zusammenfassen und Ideen** – überall, wo Ergebnisse schnell prüfbar und Fehler billig sind.
- **Halluzinationen** sind eine Folge der Funktionsweise: Zahlen, Quellen, Produkteigenschaften und Nachhaltigkeitsaussagen werden plausibel erfunden. Gegenmittel: Fakten mitgeben, `[FEHLT]`-Regel, Faktencheck.
- **Bias** aus Trainingsdaten führt zu Stereotypen in Personas, Texten und Bildern – Zielgruppen konkret beschreiben und gezielt gegenprüfen.
- Modelle haben einen **Wissensstand**; Websuche bringt Aktualität und Quellen, aber **ein Link ist ein Prüfauftrag, kein Beweis**.
- Ergebnisse sind **nicht konsistent** – eine einheitliche Markenstimme entsteht nur durch festgeschriebene Vorgaben und Beispiele.
- **Personenbezogene und vertrauliche Daten** gehören nicht in private KI-Konten; Details zu Recht und Datenampel in Kapitel 4.

---

## Kurzübungen

{{ task(file="tasks/k02_01.yaml") }}

{{ task(file="tasks/k02_02.yaml") }}

{{ task(file="tasks/k02_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k02.yaml") }}
