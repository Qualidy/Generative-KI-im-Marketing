# Kapitel 20 – Datenbasierte Optimierung von Textinhalten

{{ progress(20) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Welche **KPIs** pro Kanal wirklich etwas über die Qualität eines Textes aussagen – und welche nicht
- Wie du Daten aus Newsletter-Tool, Social-Media-Statistik und **GA4** so exportierst, dass KI damit arbeiten kann
- Wie du mit der **Datenanalyse** in ChatGPT Muster findest, ohne programmieren zu können
- Wie du **Lesbarkeit und Verständlichkeit** messbar machst und gezielt verbesserst
- Wie eine **Optimierungsschleife** aussieht, die aus Zahlen konkrete Textentscheidungen macht
- Warum **Korrelation nicht Kausalität** ist und wie du dich vor Scheinbefunden schützt
</div>

---

## 20.1 Vom Bauchgefühl zur Kennzahl

Im Marketingalltag wird über Texte meist nach Geschmack entschieden: „Die Betreffzeile klingt gut", „Der Post wirkt zu lang". Das ist nicht falsch, aber es lässt sich nicht überprüfen. Datenbasierte Optimierung heißt: Du schaust, wie Texte **tatsächlich** gewirkt haben, suchst Muster und leitest daraus Hypothesen für die nächsten Texte ab.

KI hilft dabei an zwei Stellen. Erstens beim **Auswerten**: Die Datenanalyse in ChatGPT (ein eingebautes Python-Werkzeug, Kap. 6) rechnet mit hochgeladenen Tabellen, erstellt Diagramme und fasst Auffälligkeiten zusammen. Claude, Gemini und Microsoft Copilot bieten vergleichbare Funktionen. Zweitens beim **Umsetzen**: Aus einem Befund wie „Fragen im Betreff schneiden besser ab" werden neue Textvarianten – die du dann wieder testest (Kap. 16).

Wichtig ist die Reihenfolge. Zuerst klärst du, **welche Frage** du beantworten willst, dann **welche Kennzahl** sie beantwortet, und erst dann holst du Daten. Wer umgekehrt einen großen Export hochlädt und „Was fällt dir auf?" fragt, bekommt eine Liste von Beobachtungen, von denen die Hälfte Zufall ist.

!!! info "Merksatz"
    Daten beantworten nur Fragen, die du vorher gestellt hast. **Erst Frage, dann Kennzahl, dann Export** – nie umgekehrt.

---

## 20.2 KPIs je Kanal: Was misst eigentlich den Text?

Nicht jede Kennzahl sagt etwas über den Text. Die Öffnungsrate eines Newsletters hängt fast nur an Betreff, Preheader und Absender – über den Inhalt sagt sie nichts. Die Klickrate dagegen misst, ob der Text zum Weiterlesen bewegt. Die folgende Tabelle ordnet die wichtigsten Kennzahlen dem Textelement zu, das sie beeinflusst.

| Kanal | Kennzahl | Was sie über den Text verrät | Vorsicht |
|---|---|---|---|
| Newsletter | Öffnungsrate | Wirkung von Betreff und Preheader | durch Apple Mail Privacy Protection künstlich erhöht, nur als Trend nutzen |
| Newsletter | Klickrate (CTR), Klick-zu-Öffnungsrate | Wirkung von Inhalt, Aufbau, Call-to-Action | hängt auch am Angebot, nicht nur am Text |
| Newsletter | Abmelderate | Passung von Ton und Frequenz | einzelne Ausreißer nicht überbewerten |
| Instagram/TikTok | Verweildauer, Saves, Shares | ob der Hook trägt und der Inhalt nützlich ist | Reichweite hängt stark am Algorithmus |
| LinkedIn | Interaktionsrate, Kommentare | ob der Beitrag eine Diskussion anstößt | Netzwerk der Person zählt mit |
| Blog (GA4) | Engagement-Rate, durchschnittliche Engagement-Zeit | ob der Text gelesen wird | Engagement-Zeit ist ein Mittelwert, Ausreißer verzerren |
| Blog (GA4) | Conversions, z. B. Newsletter-Anmeldung | ob der Text zum nächsten Schritt führt | kleine Zahlen schwanken stark |
| Webshop | Conversion-Rate der Produktseite | Überzeugungskraft der Produkttexte | Preis, Bilder, Lieferzeit wirken mit |

!!! warning "Typische Falle"
    **Eitelkeitskennzahlen** wie Likes oder Seitenaufrufe sehen gut aus, sagen aber wenig darüber, ob ein Text sein Ziel erreicht. Ein Blogartikel mit 10.000 Aufrufen und zehn Sekunden Lesezeit hat schlechter funktioniert als einer mit 800 Aufrufen und 40 Newsletter-Anmeldungen. Leg pro Textsorte **eine Hauptkennzahl** fest, die zum Zweck passt.

---

## 20.3 Daten exportieren und vorbereiten

Die meisten Werkzeuge bieten einen CSV- oder Excel-Export: Newsletter-Tools (z. B. Brevo, CleverReach, Mailchimp) pro Kampagne, die Meta Business Suite und LinkedIn-Seitenstatistiken pro Beitrag, GA4 über „Berichte" oder „Explorative Datenanalysen" pro Seite. Für die Textanalyse brauchst du in jeder Zeile **den Text selbst** (oder zumindest Betreff, Hook, Überschrift) und die Kennzahlen. Fehlt der Text im Export, ergänzt du ihn per Hand oder über eine eindeutige ID.

| Schritt | Was du tust | Warum |
|---|---|---|
| 1. Zeitraum wählen | z. B. die letzten 6–12 Monate | genug Fälle, aber noch vergleichbare Bedingungen |
| 2. Spalten reduzieren | Datum, Text, Merkmale, Kennzahlen | weniger Rauschen, weniger Fehldeutungen |
| 3. Personenbezug entfernen | keine E-Mail-Adressen, Namen, Kunden-IDs | DSGVO (Kap. 4), aggregierte Daten genügen |
| 4. Merkmale ergänzen | z. B. „Frage im Betreff: ja/nein", Länge, Thema | damit die Analyse Muster überhaupt sehen kann |
| 5. Prüfen | Stichprobe von zehn Zeilen gegen das Original | Exportfehler früh erkennen |

!!! tip "Merkmale von der KI vorschlagen lassen"
    Schritt 4 ist der eigentliche Hebel. Lade die Tabelle hoch und frage: „Welche Merkmale der Betreffzeilen könnten mit der Öffnungsrate zusammenhängen? Schlage maximal acht vor, die sich eindeutig mit ja/nein oder einer Zahl erfassen lassen." Die KI ergänzt diese Spalten dann selbst – du prüfst stichprobenartig, ob sie richtig zugeordnet hat.

Bei GA4 lohnt ein kurzer Blick auf die Begriffe, bevor du exportierst: Eine Sitzung gilt dort als „mit Interaktion", wenn sie länger als zehn Sekunden dauert, ein Conversion-Ereignis auslöst oder mindestens zwei Seitenaufrufe umfasst. Die **Engagement-Rate** ist der Anteil solcher Sitzungen. Für Blogartikel ist das aussagekräftiger als die alte Absprungrate, aber immer noch grob: Zehn Sekunden reichen nicht, um einen Ratgeber zu lesen. Wenn ihr Scrolltiefe oder Klicks auf interne Links als Ereignisse erfasst, kannst du genauer sehen, wo Leserinnen aussteigen – und genau diese Stelle im Text überarbeiten.

Für Fjordlicht reichen für einen ersten Blick auf den Newsletter wenige Spalten: Versanddatum, Betreff, Thema, Öffnungsrate, Klickrate, Abmeldungen. Bei rund 38.000 Abonnenten und einem Versand pro Woche entstehen so etwa 50 Zeilen pro Jahr – genug für Tendenzen, zu wenig für harte Beweise.

---

## 20.4 Analyse mit ChatGPT: Muster finden, Befunde prüfen

Ein guter Analyse-Prompt folgt dem P.R.O.M.P.T.-Framework (Kap. 5). Besonders wichtig sind hier **Purpose** (welche Entscheidung soll die Analyse stützen?) und **Modifier** (welche Regeln gelten für vorsichtige Aussagen?).

```text
Persona: Du bist Datenanalystin im Content-Marketing und erklärst
Ergebnisse so, dass ein Team ohne Statistikkenntnisse sie versteht.
Request: Analysiere die angehängte Tabelle mit 52 Newsletter-Versänden.
Prüfe, welche Merkmale der Betreffzeile mit Öffnungsrate und Klickrate
zusammenhängen.
Output: 1) Tabelle der Merkmale mit Mittelwert je Ausprägung und Anzahl
Fälle, 2) ein Diagramm, 3) maximal fünf Befunde in Stichpunkten,
4) drei Hypothesen für künftige A/B-Tests.
Modifier: Nenne bei jedem Befund die Anzahl der Fälle. Kennzeichne
Befunde mit weniger als 10 Fällen pro Gruppe als "unsicher".
Formuliere Zusammenhänge, keine Ursachen. Erfinde keine Werte.
Purpose: Wir wollen entscheiden, welche Betreffzeilen-Muster wir im
nächsten Quartal gezielt testen.
Tone: sachlich, nüchtern, ohne Übertreibungen.
```

Danach kommt der Teil, den viele auslassen: die **Plausibilitätsprüfung**. Lass dir den Rechenweg zeigen („Zeige mir den Code und die Zwischenergebnisse"), prüfe einen Mittelwert per Hand in Excel und frage gezielt nach Gegenerklärungen: „Welche anderen Faktoren könnten diesen Unterschied erklären?" Die Datenanalyse rechnet zuverlässig – aber sie interpretiert genauso selbstbewusst wie ein Sprachmodell formuliert, und gelegentlich liest sie eine Spalte falsch ein (Dezimalkomma, Prozentzeichen, Datumsformat).

!!! example "Fjordlicht: ein Befund und seine Prüfung"
    Die Analyse meldet: „Betreffzeilen mit Produktnamen haben 4,1 Prozentpunkte niedrigere Öffnungsraten." Auf Nachfrage zeigt sich: Alle Produkt-Betreffzeilen wurden im Sommer verschickt, wenn die Öffnungsraten generell sinken. Vergleicht man nur Versände desselben Quartals, schrumpft der Unterschied auf 0,8 Punkte – kaum mehr als Zufall. Der Befund wird zur **Hypothese**, nicht zur Regel.

---

## 20.5 Lesbarkeit und Verständlichkeit messen

Neben Reaktionsdaten gibt es eine zweite Datenquelle: den Text selbst. Lesbarkeit lässt sich näherungsweise messen – über Satzlänge, Wortlänge und Fachwortdichte. Bekannt ist der **Flesch-Lesbarkeitsindex** in der deutschen Anpassung nach Amstad (höher = leichter lesbar) und die **Wiener Sachtextformel**. Online-Prüfer und Schreibwerkzeuge berechnen solche Werte; die KI kann sie in der Datenanalyse ebenfalls ausrechnen, wenn du sie ausdrücklich darum bittest. Schätzt sie den Wert nur „aus dem Bauch", ist er wertlos.

| Merkmal | Richtwert für Marketingtexte an Endkunden | Wie KI hilft |
|---|---|---|
| Satzlänge | im Schnitt unter 15 Wörtern, Ausreißer über 25 vermeiden | lange Sätze markieren und teilen lassen |
| Fach- und Fremdwörter | nur, wenn die Zielgruppe sie kennt | Liste erstellen, Alternativen vorschlagen |
| Nominalstil | Verben statt „Durchführung der Prüfung" | Passagen in Verbalstil umformulieren |
| Aufbau | Kernaussage zuerst, Zwischenüberschriften | Gliederung prüfen und vorschlagen |
| Aktiv statt Passiv | „Wir nähen" statt „Es wird genäht" | Passivsätze auflisten |

Formeln messen Oberfläche, nicht Verständnis. Ein Text kann kurze Sätze haben und trotzdem unklar sein. Ergänze deshalb einen **Verständnistest**: Gib der KI den Text und den Kundenavatar (Kap. 18) und lass sie die drei Fragen formulieren, die eine Leserin danach noch hätte. Für B2B-Texte von Fjordlicht Business gelten andere Richtwerte als für Instagram – Einkäufer erwarten Fachbegriffe wie „Arbeitsschutznorm" oder „Rahmenvertrag".

!!! warning "Typische Falle"
    Lesbarkeitswerte werden schnell zum Selbstzweck. Wer jeden Text auf maximalen Flesch-Wert trimmt, verliert die Markenstimme – bei Fjordlicht etwa den ruhigen, leicht nordisch-trockenen Ton. Nutze Werte als **Warnsignal** für Ausreißer, nicht als Ziel.

---

## 20.6 Die Optimierungsschleife – und die Grenze der Daten

Aus Daten wird erst dann Optimierung, wenn ein Befund eine Handlung auslöst und diese Handlung wieder gemessen wird. Diese Schleife läuft bei Fjordlicht einmal pro Quartal:

```mermaid
flowchart LR
    A([Frage festlegen]) --> B([Daten exportieren])
    B --> C([Analyse mit KI])
    C --> D([Befund prüfen])
    D --> E([Hypothese formulieren])
    E --> F([Varianten texten und testen])
    F --> G([Ergebnis dokumentieren])
    G --> A
```

Der entscheidende Schritt ist **D**: Befund prüfen. Hier steckt die wichtigste statistische Regel des Kapitels: **Korrelation ist nicht Kausalität.** Dass zwei Dinge gemeinsam auftreten, heißt nicht, dass das eine das andere verursacht. Typische Störfaktoren im Content-Marketing:

| Scheinbarer Befund | Mögliche andere Erklärung |
|---|---|
| „Lange Blogartikel ranken besser." | Lange Artikel behandeln wichtigere Themen und werden häufiger verlinkt. |
| „Posts mit Emojis bekommen mehr Likes." | Sie wurden vor allem zu Gewinnspielen veröffentlicht. |
| „Dienstags-Newsletter werden öfter geöffnet." | Dienstags lagen zufällig die Rabattaktionen. |
| „Du-Ansprache bringt mehr Klicks." | Die Du-Texte liefen nur an die junge, aktivere Zielgruppe. |

Kausalität belegt nur ein kontrollierter Test, bei dem sich genau **eine** Variable unterscheidet – dafür gibt es das A/B-Testing (Kap. 16). Die Datenanalyse liefert also keine Wahrheiten, sondern **gute Kandidaten für Tests**. Dokumentiere jede Hypothese mit Datum, Befund, Testergebnis und Konsequenz; nach einem Jahr hast du ein Lernarchiv, das mehr wert ist als jede einzelne Auswertung.

!!! info "Merksatz"
    Die Analyse sagt dir, **wo** du hinschauen solltest. Ob eine Änderung wirkt, sagt dir erst der **Test**.

---

## Zusammenfassung

- Datenbasierte Optimierung beginnt mit einer **Frage**, nicht mit einem Export; pro Textsorte gibt es eine passende Hauptkennzahl.
- Nicht jede Kennzahl misst den Text: Öffnungsrate misst Betreff und Preheader, Klickrate den Inhalt, **Eitelkeitskennzahlen** wenig.
- Exporte werden reduziert, **ohne Personenbezug** vorbereitet und um Merkmale wie Länge, Frage ja/nein oder Thema ergänzt.
- Die **Datenanalyse** in ChatGPT rechnet zuverlässig, interpretiert aber selbstbewusst – Rechenweg zeigen lassen, Stichproben prüfen, Gegenerklärungen einfordern.
- **Lesbarkeitswerte** sind Warnsignale für Ausreißer, kein Selbstzweck; ein Verständnistest mit dem Kundenavatar ergänzt sie.
- **Korrelation ist nicht Kausalität**: Analysen liefern Hypothesen, erst ein A/B-Test liefert Belege.

---

## Kurzübungen

{{ task(file="tasks/k20_01.yaml") }}

{{ task(file="tasks/k20_02.yaml") }}

{{ task(file="tasks/k20_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k20.yaml") }}
