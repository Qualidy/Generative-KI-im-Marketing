# Kapitel 18 – Kundenavatar entwickeln und nutzen

{{ progress(18) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Worin sich **Persona** und **Kundenavatar** unterscheiden – und warum die Begriffe in der Praxis durcheinandergehen
- Wie du aus deiner Zielgruppenanalyse einen belastbaren **Avatar-Steckbrief** baust
- Wie du den Avatar als festen **Prompt-Baustein** im P.R.O.M.P.T.-Framework einsetzt
- Was **simulierte Interviews** und **synthetische Personas** leisten – und wo sie gefährlich werden
- Wie du Texte mit einem **Avatar-Check** aus Sicht der Zielperson prüfst
- Wie du Avatare **pflegst**, damit sie nicht zur Fiktion werden
</div>

---

## 18.1 Persona oder Avatar?

Die Begriffe werden in Agenturen, Büchern und Online-Kursen unterschiedlich verwendet, oft sogar synonym. Für diesen Kurs gilt eine einfache Arbeitsunterscheidung:

| | Persona | Kundenavatar |
|---|---|---|
| Zweck | gemeinsames Bild eines Segments im Team und in der Strategie | Arbeitsmittel beim Schreiben und Prüfen konkreter Texte |
| Detailgrad | eher breit: Ziele, Verhalten, Kanäle | sehr konkret: Situation, Worte, Einwände, Entscheidungsmoment |
| Herkunft | UX-Design und Marktforschung | Direktmarketing und Copywriting |
| typische Frage | „Wen wollen wir erreichen?" | „Was denkt diese Person, wenn sie genau diesen Text liest?" |
| Lebensdauer | länger, strategisch | wird mit jeder Kampagne geschärft |

Beide beruhen auf derselben Grundlage: der Zielgruppenanalyse aus Kap. 17. Ein Avatar ohne Datenbasis ist ein Fantasieprodukt, das nur die Vorurteile des Teams bestätigt. Pro Segment genügt in der Regel **ein** Avatar; Fjordlicht arbeitet mit drei: Stadtmensch, Familie, B2B-Einkauf.

!!! info "Merksatz"
    Eine Persona sagt, **wen** du ansprichst. Ein Avatar sagt, **wie** diese Person deinen Text liest. Beide sind nur so gut wie die Daten, aus denen sie entstehen.

---

## 18.2 Der Avatar-Steckbrief

Ein guter Steckbrief beschreibt nicht das Leben einer Person, sondern genau die Merkmale, die für eure Kommunikation einen Unterschied machen. Lieblingsfarbe und Sternzeichen gehören nicht hinein – Kaufauslöser und Einwände schon.

| Feld | Inhalt | Beispiel „Jana" (Segment Stadtmensch) |
|---|---|---|
| Name und Kurzbild | ein Satz, damit das Team den Avatar erinnert | Jana, 34, Projektmanagerin, wohnt in Münster |
| Situation | Lebens- und Nutzungssituation | radelt täglich ins Büro, am Wochenende Tagestouren im Münsterland und Sauerland |
| Job-to-be-done | Aufgabe, die das Produkt erledigt | trocken und ordentlich ankommen, eine Jacke für Alltag und Ausflug |
| Pain Points | Ärger, Risiken, Zweifel | misstraut Öko-Versprechen, hat schon zwei Jacken gekauft, die nach einem Winter durch waren |
| Gains | erhoffte Vorteile | weniger, aber bessere Kleidung; kein „Funktionslook" im Büro |
| Kundensprache | wörtliche Formulierungen | „nicht nach Expedition aussehen", „hält, was draufsteht" |
| Einwände vor dem Kauf | was sie zögern lässt | Preis, Passform bei Bestellung online |
| Informationsverhalten | Kanäle und Momente | Instagram abends, Newsletter am Wochenende, liest Bewertungen gründlich |
| Was sie abschreckt | No-Gos in der Ansprache | Superlative, „klimaneutral" ohne Beleg, Influencer-Ton |
| Evidenz | Quellen und Stufe je Feld | Bewertungen (gestützt), 4 Kundengespräche (bestätigt), Informationsverhalten (Hypothese) |

Die letzte Zeile ist die wichtigste. Sie macht sichtbar, welche Teile des Avatars auf Daten beruhen und welche auf Annahmen (Kap. 17.6). Wer später einen Text mit dem Avatar prüft, weiß damit, wie viel Gewicht ein Urteil hat.

**Besonderheit im B2B:** Bei „Fjordlicht Business" entscheidet selten eine einzelne Person. Die Geschäftsführung achtet auf Außenwirkung und Budget, der Einkauf auf Lieferzeit und Nachbestellbarkeit, die Mitarbeitenden, die die Kleidung tragen, auf Passform und Bequemlichkeit. Man spricht vom **Buying Center**. Für den Avatar heißt das: Lege fest, wen dein Text in erster Linie erreichen soll, und ergänze ein Feld „Wer entscheidet mit?" mit den Einwänden der anderen Beteiligten. Eine Angebotsmail an den Einkauf, die nur über Markenwirkung spricht, verfehlt ihr Ziel, auch wenn sie sprachlich gelungen ist.

!!! tip "Steckbrief mit KI entwerfen"
    Gib der KI dein Zielgruppenbriefing und lass einen ersten Entwurf in genau dieser Feldstruktur erstellen – mit der Regel, dass jedes Feld eine Quellenangabe trägt und Unbelegtes als `[HYPOTHESE]` markiert wird. Das Ergebnis ist ein Entwurf, den das Team diskutiert und korrigiert, nicht das fertige Produkt.

---

## 18.3 Der Avatar als Prompt-Baustein

Im P.R.O.M.P.T.-Framework (Kap. 5) gehört der Avatar in den Baustein **Purpose**: Er beantwortet „für wen" so konkret, dass das Modell nicht auf den Durchschnitt ausweicht. Den vollständigen Steckbrief brauchst du dafür nicht. Eine **Kurzfassung** von 80 bis 120 Wörtern reicht und lässt sich in jeden Prompt kopieren.

**Vorher – Purpose als Floskel**

```text
Schreibe einen Instagram-Post zur Regenjacke Sølv für unsere
Zielgruppe. Ton: locker.
```

Ergebnis: „Egal ob Stadtdschungel oder Bergabenteuer – mit Sølv bist du für jedes Wetter gewappnet!" Austauschbar, mit Superlativ-Tendenz, ohne Bezug zu echten Situationen.

**Nachher – Avatar im Purpose**

```text
Persona: Du bist Social-Media-Texterin von Fjordlicht.
Request: Schreibe einen Instagram-Post zur Regenjacke Sølv.
Output: Caption mit max. 80 Wörtern, erste Zeile als Hook, 3 Hashtags.
Modifier: Keine Superlative, keine Nachhaltigkeitsaussage ohne Beleg.
Nutze Formulierungen aus der Kundensprache, wo es passt.
Purpose: Ziel ist ein Klick auf die Produktseite. Der Post richtet sich an:
"""
Jana, 34, radelt täglich ins Büro in Münster, am Wochenende Tagestouren.
Will trocken und ordentlich ankommen und eine Jacke für Alltag und
Ausflug. Misstraut Öko-Versprechen, hatte schon Jacken, die nach einem
Winter durch waren. Sagt Sätze wie "nicht nach Expedition aussehen".
Zögert wegen Preis und Passform beim Onlinekauf.
"""
Tone: ruhig, ehrlich, leicht nordisch-trocken, Du-Ansprache.
```

Das Ergebnis setzt an einer echten Situation an („Montag, 7:40 Uhr, Nieselregen auf der Promenade"), greift den Einwand auf und verzichtet auf Pathos. Der Unterschied entsteht nicht durch geschicktere Formulierungen, sondern durch **besseres Material**.

!!! tip "Avatar dauerhaft hinterlegen"
    Statt die Kurzfassung jedes Mal einzufügen, legst du sie als Datei in einem **Projekt** ab oder in den benutzerdefinierten Anweisungen (Kap. 7). Für mehrere Avatare eignet sich eine Datei pro Avatar mit klarer Benennung. In einem eigenen Assistenten wie dem Content-Assistenten von Fjordlicht werden Avatare zur Wissensdatei (Kap. 24, Kap. 26).

---

## 18.4 Simulierte Interviews und synthetische Personas

Ein naheliegender Gedanke: Wenn das Modell den Avatar kennt, kann es ihn auch **spielen**. Du lässt dich von „Jana" interviewen, stellst ihr Fragen zu einer Kampagnenidee oder lässt zehn KI-Personen eine Umfrage beantworten. Man spricht dann von **synthetischen Personas** oder synthetischen Nutzern.

```text
Du spielst Jana (Steckbrief unten). Bleib in der Rolle und antworte so,
wie sie es vermutlich tun würde - knapp, skeptisch, ohne Marketingsprache.
Wenn eine Frage etwas betrifft, wozu der Steckbrief nichts sagt,
antworte mit "Dazu kann ich aus dem Steckbrief nichts ableiten."
Ich stelle dir gleich Fragen zu einer Kampagnenidee.
Steckbrief: """ [Steckbrief einfügen] """
```

Die Rückfall-Regel am Ende ist wichtig: Ohne sie erfindet das Modell bereitwillig Vorlieben, Erlebnisse und Meinungen, die durch nichts gedeckt sind.

| Gut geeignet für | Ungeeignet für |
|---|---|
| Einwände sammeln, an die das Team nicht gedacht hat | Belegen, dass eine Idee ankommt |
| Interviewleitfäden testen, bevor echte Gespräche stattfinden | Kaufbereitschaft, Preisakzeptanz, Prozentwerte |
| unverständliche Formulierungen in einem Text aufspüren | Ersatz für echte Kundengespräche |
| Perspektivwechsel im Brainstorming (Kap. 7, Kap. 12) | Gruppen, über die wenig Daten vorliegen – dort wird fast alles erfunden |

!!! warning "Typische Falle"
    Synthetische Personas sind **gefällig**. Sie antworten plausibel, zeigen kaum Widersprüche, neigen zu Zustimmung und spiegeln Stereotype aus den Trainingsdaten (Kap. 2). Zehn KI-Interviews sind keine Stichprobe, sondern **zehnmal derselbe Durchschnitt** mit leicht verändertem Wortlaut. Wer daraus „80 Prozent der Befragten finden die Idee gut" macht, betreibt Selbsttäuschung.

Nutze simulierte Interviews daher als **Vorbereitung**: Sie liefern Fragen, Hypothesen und Formulierungen, die du anschließend mit echten Menschen prüfst.

---

## 18.5 Der Avatar-Check für Texte

Die zweite starke Anwendung ist die **Prüfung** fertiger Entwürfe. Statt „Ist der Text gut?" fragst du: „Wie liest Jana diesen Text – und wo steigt sie aus?" Das schärft das Feedback, weil es an einer konkreten Person gemessen wird statt an allgemeinem Geschmack.

```text
Lies den folgenden Newsletter-Entwurf aus Sicht von Jana (Steckbrief unten).
Bewerte in einer Tabelle:
1. Hook: Würde Jana nach der ersten Zeile weiterlesen? Warum (nicht)?
2. Relevanz: Welche Stelle trifft ihre Situation, welche nicht?
3. Einwände: Welcher ihrer Einwände bleibt unbeantwortet?
4. Abschreckung: Wo stößt sie auf etwas, das sie nicht mag?
5. Handlung: Ist klar, was sie als Nächstes tun soll?
Begründe jeden Punkt mit einem Bezug zum Steckbrief.
Schlage zum Schluss die drei wirksamsten Änderungen vor.
Steckbrief: """ [Kurzfassung] """
Entwurf: """ [Text] """
```

| Prüfpunkt | Gutes Zeichen | Warnsignal |
|---|---|---|
| Hook | knüpft an eine Alltagssituation an | allgemeine Wetter- oder Abenteuerfloskel |
| Einwände | Preis und Passform werden aufgegriffen | nur Produkteigenschaften |
| Sprache | Formulierungen aus der Kundensprache | Fachbegriffe, Superlative |
| Belege | Nachhaltigkeit mit konkretem Nachweis | „umweltfreundlich" ohne Angabe |

Der Avatar-Check ersetzt keinen A/B-Test (Kap. 16) und keine Freigabe. Er ist ein schneller Filter **vor** dem Test: Varianten, die schon am Avatar scheitern, musst du nicht ins Feld schicken.

!!! example "Zwei Avatare, ein Text"
    Prüfe denselben Text nacheinander mit zwei Avataren, etwa Jana und dem Familien-Avatar „Tobias, 41, zwei Kinder". Wenn beide ihn gut finden, ist er oft zu allgemein. Wenn beide ihn schlecht finden, fehlt meist der Bezug zu einer konkreten Situation. Das Ergebnis zeigt dir, ob du **einen** Text für beide brauchst oder zwei Varianten.

---

## 18.6 Avatare pflegen

Avatare altern. Märkte verändern sich, neue Produkte ziehen neue Kundschaft an, und was vor zwei Jahren ein Einwand war, ist heute vielleicht gelöst. Ein nie überarbeiteter Avatar wird schleichend zur Fiktion – und weil er im Prompt steckt, wirkt er weiter, ohne dass es jemand bemerkt.

| Anlass | Was du prüfst |
|---|---|
| halbjährlich | neue Bewertungen, Kundenservice-Themen, Kanalnutzung – passt der Steckbrief noch? |
| nach jedem A/B-Test | bestätigt oder widerlegt das Ergebnis eine Annahme im Avatar? |
| neues Produkt oder neuer Kanal | braucht es einen neuen Avatar oder nur ein ergänztes Feld? |
| Social-Listening-Auffälligkeiten (Kap. 19) | tauchen neue Themen, Begriffe oder Kritikpunkte auf? |

!!! warning "Typische Falle"
    Der Avatar wird zum **Wunschkunden**. Mit jeder Überarbeitung rutschen Eigenschaften hinein, die das Team gern hätte – mehr Budget, mehr Begeisterung für Nachhaltigkeit, weniger Preissensibilität. Prüfe deshalb bei jeder Änderung: Welche Quelle stützt das? Ein unbequemer Einwand im Steckbrief ist wertvoller als ein sympathisches Detail.

Führe zu jedem Avatar eine **Versionsangabe** und ein Änderungsprotokoll, so wie bei Prompts in der Bibliothek (Kap. 10). Wenn ein Feld von „Hypothese" auf „bestätigt" springt oder gestrichen wird, gehört das mit Datum und Quelle dazu.

---

## Zusammenfassung

- **Persona** beschreibt ein Segment für das Team, der **Kundenavatar** ist ein konkretes Arbeitsmittel zum Schreiben und Prüfen – beide brauchen Daten aus der Zielgruppenanalyse.
- Ein guter **Steckbrief** enthält nur kommunikationsrelevante Felder und weist für jedes Feld die **Evidenz** aus.
- Als Kurzfassung gehört der Avatar in den **Purpose** des P.R.O.M.P.T.-Frameworks; dauerhaft hinterlegt in Projekten oder Assistenten.
- **Synthetische Personas** helfen beim Sammeln von Einwänden und Fragen, ersetzen aber keine echten Gespräche und liefern keine Zahlen.
- Der **Avatar-Check** prüft Entwürfe gezielt auf Hook, Relevanz, Einwände, Abschreckung und Handlung.
- Avatare werden regelmäßig **überprüft und versioniert**, sonst wirken veraltete Annahmen unbemerkt in jedem Prompt weiter.

---

## Kurzübungen

{{ task(file="tasks/k18_01.yaml") }}

{{ task(file="tasks/k18_02.yaml") }}

{{ task(file="tasks/k18_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k18.yaml") }}
