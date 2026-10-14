# Kapitel 37 – KI-Musik & Audio für Social Media

{{ progress(37) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wo **Musik und Audio** im Social-Media-Marketing gebraucht werden und welche Bezugswege es gibt
- Welche **KI-Musikwerkzeuge** es gibt (Suno, Udio, ElevenLabs Music, Google Flow Music) und worin sie sich bei Lizenz und Nutzung unterscheiden
- Wie du **Musik promptest**: Genre, Stimmung, Tempo, Instrumente, Struktur und Länge
- Was **Sound-Branding** ist und wie KI beim Entwurf eines Sound-Logos helfen kann – und wo nicht
- Wie KI bei **Podcasts und Audiogrammen** Arbeit abnimmt
- Wie die **Lizenzlage** aussieht: Plattformbibliotheken, Nutzungsbedingungen der Tools, Schutzfähigkeit und die **GEMA-Urteile** des LG München I
</div>

---

## 37.1 Wo Musik im Social-Media-Marketing gebraucht wird

Ein Reel ohne Ton wirkt leer, ein TikTok-Clip lebt oft vom Sound. Dazu kommen Produktvideos im Webshop, Podcast-Intros, Hintergrundmusik für Erklärvideos (Kap. 36) und kurze Audiogramme für LinkedIn. Bisher gab es für Unternehmen vier Wege, an Musik zu kommen – KI ist der fünfte, nicht der einzige.

| Bezugsweg | Vorteil | Nachteil | Typischer Einsatz |
|---|---|---|---|
| **Plattformbibliothek** (Instagram, TikTok) | direkt in der App, Trends nutzbar | für Unternehmensaccounts oft nur die „Commercial Music Library"; nur auf dieser Plattform | spontane Reels und Stories |
| **Stock-Musik** (z. B. Epidemic Sound, Loudly) | klare Lizenz, große Auswahl | Abo-Kosten; andere Marken nutzen dieselben Tracks | Produktvideos, Werbeclips |
| **Auftragskomposition** | einzigartig, Rechte vertraglich geregelt | teuer, dauert | Sound-Logo, Kampagnen-Hauptmotiv |
| **Gemeinfreie Musik** | kostenlos | kleine Auswahl, Aufnahme kann trotzdem geschützt sein | Nischeneinsatz |
| **KI-Musik** | schnell, günstig, passgenau beschreibbar | Lizenz je Tool und Tarif verschieden, Rechtslage im Fluss | Hintergrundmusik, Varianten, Entwürfe |

!!! warning "Typische Falle"
    „Der Song ist doch in der Instagram-App verfügbar, also darf ich ihn nutzen." Für **private** Accounts ist das Angebot größer als für **Unternehmensaccounts**. Wer als Marke einen bekannten Charthit unter ein Reel legt, bewegt sich meist außerhalb der Lizenz – auch wenn die App es technisch zulässt. Und: Ein so lizenzierter Sound gilt nur dort. Exportierst du das Video für Webshop oder Newsletter, ist die Musik nicht mehr abgedeckt.

---

## 37.2 Die Werkzeuglandschaft (Stand: Oktober 2026)

KI-Musik ist der Bereich, in dem sich Geschäftsmodelle und Lizenzbedingungen 2025 und 2026 am stärksten verändert haben. Die folgende Übersicht ist eine Momentaufnahme – prüfe vor jeder kommerziellen Nutzung die aktuellen Bedingungen deines Tarifs.

| Werkzeug | Was es kann | Kommerzielle Nutzung | Besonderheit |
|---|---|---|---|
| **Suno** | komplette Songs mit Gesang und Text oder instrumental aus einem Textprompt | nur in Bezahlplänen, und zwar für Songs, die **während des Abos** erzeugt wurden | Verfahren GEMA ./. Suno (siehe 37.6) |
| **Udio** | Songs mit Gesang, feine Bearbeitung einzelner Abschnitte | nach Vergleichen mit Musiklabels im Umbau zur lizenzierten Plattform; Downloads zeitweise deaktiviert | aktuelle Bedingungen unbedingt prüfen |
| **ElevenLabs Music** | Musik aus Textprompt, auch für Werbung gedacht | in Bezahlplänen; Anbieter betont lizenzierte Trainingsgrundlage | gleicher Anbieter wie Sprecherstimmen (Kap. 36, 38) |
| **Google Flow Music** (Modellfamilie Lyria) | Musik und Klangflächen, Einbindung in Googles Kreativwerkzeuge | nach Google-Bedingungen | unsichtbares **SynthID-Wasserzeichen** |
| **Stock mit KI-Funktionen** (Loudly, Epidemic Sound) | Katalogmusik, teils KI-gestützt anpassbar (Länge, Stimmung) | im Abo geregelt | Lizenzlage am klarsten |

Für Hintergrundmusik in Social-Clips ist ein Stock-Abo oft die unspektakulärste und sicherste Lösung. KI-Musik spielt ihre Stärke aus, wenn du etwas **Passgenaues** brauchst: exakt 15 Sekunden, ein bestimmter Stimmungswechsel nach Sekunde 8, sechs Varianten desselben Motivs für eine Serie.

!!! info "Merksatz"
    Bei KI-Musik entscheidet nicht das Tool über die Nutzbarkeit, sondern der **Tarif zum Zeitpunkt der Erzeugung**. Dokumentiere deshalb für jeden verwendeten Track: Tool, Tarif, Datum, Prompt.

---

## 37.3 Musik-Prompting

Musik-Prompts folgen derselben Logik wie Text- und Bildprompts (Kap. 5, 30): Alles, was du nicht festlegst, entscheidet das Modell nach Wahrscheinlichkeit – und das Wahrscheinlichste ist austauschbarer Pop mit Gesang. Sechs Bausteine machen den Unterschied.

| Baustein | Was du festlegst | Beispiel |
|---|---|---|
| **Genre** | Stilrichtung, gern kombiniert | „Nordic Folk mit leichtem Ambient" |
| **Stimmung** | Gefühl und Entwicklung | „ruhig, weit, am Ende leicht aufbrechend" |
| **Tempo** | BPM oder Umschreibung | „ca. 85 BPM, gleichmäßiger Gehrhythmus" |
| **Instrumente** | Besetzung, auch was fehlen soll | „Akustikgitarre, Kontrabass, gestrichene Saiten, kein Schlagzeug" |
| **Gesang** | instrumental oder Stimme, Sprache, Text | „instrumental" oder „weibliche Stimme, Englisch, eigener Text" |
| **Struktur und Länge** | Aufbau, Dauer, Ende | „Intro 3 s, Steigerung, klares Ende bei 15 s, kein Fade-out" |

Ein Beispiel für Fjordlicht, Reel zur Regenjacke „Sølv" – zuerst der übliche Anfang, dann die präzise Fassung:

```text
Mach ruhige Musik für ein Outdoor-Video.
```

Ergebnis: eine generische Piano-Ballade oder ein Lagerfeuer-Pop-Song mit Fantasietext über Freiheit. Brauchbar ist das selten.

```text
Instrumental, keine Stimme.
Genre: Nordic Folk mit Ambient-Elementen.
Stimmung: ruhig, regnerisch, nachdenklich; ab der Mitte heller,
als ob die Wolken aufreißen.
Tempo: ca. 80 BPM.
Instrumente: Fingerpicking-Akustikgitarre, Kontrabass, leise
gestrichene Saiten, dezente Regengeräusche im Intro.
Kein Schlagzeug, keine Synthesizer-Flächen, kein Pathos.
Struktur: 2 s Regen, dann Gitarre; Steigerung ab Sekunde 8;
klares Ende bei 15 s ohne Fade-out.
Verwendung: Instagram-Reel, Sprache im Video wird darüber gelegt.
```

!!! tip "Lass dir den Musik-Prompt von ChatGPT schreiben"
    Musikalisches Vokabular fehlt vielen. Beschreibe ChatGPT (oder Claude, Gemini) die Szene, die Zielgruppe und die Markenstimme und lass dir drei Musik-Prompts in unterschiedlichen Richtungen formulieren. Du entscheidest danach mit den Ohren, nicht mit dem Fachbegriff.

    ```text
    Du bist Music Supervisor für Social-Media-Werbung.
    Szene: [Beschreibung des Videos, Länge, Schnittpunkte]
    Marke: [Markenstimme in drei Adjektiven]
    Zielgruppe: [Zielgruppe]
    Schreibe drei unterschiedliche Prompts für ein KI-Musikwerkzeug,
    je mit Genre, Stimmung, Tempo in BPM, Instrumenten, Struktur mit
    Sekundenangaben und dem, was ausdrücklich NICHT vorkommen soll.
    Nenne keine Künstler- oder Songnamen.
    ```

!!! warning "Typische Falle"
    „Klingt wie [bekannte Band]" oder „im Stil von [Songtitel]" ist der schnellste Weg zu einem Track, der einem geschützten Werk zu nahe kommt. Viele Tools blockieren Künstlernamen ohnehin. Beschreibe stattdessen die **Merkmale**, die dir gefallen: Tempo, Besetzung, Gesangsstil, Produktionsweise. Stil-Imitation ist nicht per se verboten, die Nachbildung konkreter Werke schon.

---

## 37.4 Sound-Branding: wie eine Marke klingt

**Sound-Branding** (auch Audio-Branding) heißt, einer Marke einen wiedererkennbaren Klang zu geben: ein **Sound-Logo** von zwei bis drei Sekunden, ein Klangcharakter für Hintergrundmusik, eine Sprecherstimme (Kap. 36, 38). Wer sechs Monate lang jedes Reel mit zufällig gewählter Musik unterlegt, hat am Ende keinen Klang, sondern Rauschen.

KI hilft dabei vor allem in der **Exploration**: Du kannst in einer Stunde dreißig Richtungen hören, wofür eine Agentur früher Tage brauchte. Für das endgültige Sound-Logo, das jahrelang auf allen Kanälen läuft, ist sie dagegen problematisch – rein KI-erzeugte Musik ist in Deutschland ohne menschliche schöpferische Leistung in der Regel **nicht urheberrechtlich geschützt** (§ 2 Abs. 2 UrhG). Ein Mitbewerber könnte die Tonfolge also übernehmen. Für ein Markenzeichen ist das ein ernstes Argument, das Ergebnis von einem Menschen ausarbeiten zu lassen und die Rechte vertraglich zu sichern.

!!! example "Audio-Leitbild für Fjordlicht"
    ```text
    AUDIO-LEITBILD FJORDLICHT (Entwurf)
    Klangcharakter: akustisch, warm, luftig, nordisch-ruhig
    Instrumente:    Akustikgitarre, Holzbläser, Streicher, Naturklänge
    Tempo:          60 bis 95 BPM, nie hektisch
    Vermeiden:      EDM-Drops, Trailer-Pathos, Ukulele-Fröhlichkeit
    Sound-Logo:     drei aufsteigende Töne, Gitarre plus Holz-Percussion,
                    max. 2,5 s, endet offen
    Sprache:        ruhige Stimme, kein Werbeton (siehe Kap. 38)
    ```

    Dieses Leitbild ist zugleich ein Prompt-Baustein: Du hängst es an jeden Musik-Prompt an und bekommst Varianten, die zueinander passen.

---

## 37.5 Podcasts und Audiogramme

Audio ist nicht nur Musik. Viele Marketingteams betreiben einen Podcast oder schneiden Interviews zu kurzen **Audiogrammen** – Audioausschnitt mit Wellenform und Untertiteln, gut für LinkedIn und Instagram. Hier nimmt KI an vielen Stellen Arbeit ab, ohne dass rechtlich Neuland betreten wird.

| Arbeitsschritt | Was KI übernimmt | Werkzeugbeispiele | Was du prüfst |
|---|---|---|---|
| Vorbereitung | Themenideen, Fragenkatalog, Gliederung | ChatGPT, Claude | Relevanz, Faktenlage |
| Aufnahme-Nachbearbeitung | Rauschen entfernen, Pegel angleichen, Füllwörter schneiden | Descript, Adobe Podcast | Natürlichkeit, Sinnentstellung |
| Transkript | Sprache zu Text, Sprecher trennen | ChatGPT, Descript | Namen, Fachbegriffe |
| Shownotes und Kapitel | Zusammenfassung, Zeitmarken, Links | ChatGPT | Zitate wörtlich korrekt? |
| Audiogramme | stärkste 30–60 s finden, Untertitel | ChatGPT plus Schnittwerkzeug | Kontext des Zitats erhalten |
| Intro, Jingle | Musik nach Audio-Leitbild | KI-Musik oder Stock | Lizenz, Markenpassung |

```text
Hier das Transkript unserer Podcastfolge: [Transkript]
Finde die drei Passagen, die sich am besten als Audiogramm
(30 bis 60 Sekunden) für LinkedIn eignen. Kriterien: eine klare
Aussage, ohne Vorwissen verständlich, kein Zitat aus dem Kontext
gerissen. Gib je Passage Zeitmarke, wörtliches Zitat und einen
Vorschlag für eine Caption mit max. 200 Zeichen aus.
```

Wichtig: Wer Gäste schneidet, kürzt oder Passagen mit KI-Stimme „repariert", verändert deren Aussage. Das gehört abgesprochen – mehr dazu im nächsten Kapitel zum Voice Cloning.

---

## 37.6 Lizenzlage, Plattformregeln und die GEMA-Urteile

Rund um KI-Musik laufen in Deutschland mehrere wichtige Verfahren. Die beiden für den Kurs zentralen hat die **GEMA** vor dem **Landgericht München I** geführt:

| Verfahren | Datum | Kern | Status |
|---|---|---|---|
| **GEMA ./. OpenAI** | 11.11.2025 | Liedtexte, die im Modell **memorisiert** sind und wiedergegeben werden können, gelten als Vervielfältigung | **nicht rechtskräftig** |
| **GEMA ./. Suno** | 31.07.2026 | GEMA erhält gegen den Musikgenerator **weitgehend Recht** | **nicht rechtskräftig** |

Beide Urteile betreffen zunächst die **Anbieter** der Modelle, nicht dich als Nutzerin. Sie sind aber ein deutliches Signal: Die Frage, ob KI-Musik auf rechtlich sauberer Grundlage entsteht, ist nicht geklärt, und höhere Instanzen können anders entscheiden. Für dich als Betreiber folgen daraus drei praktische Regeln.

1. **Tarif und Bedingungen dokumentieren.** Kommerzielle Nutzung nur im passenden Bezahlplan, Screenshot oder Kopie der Bedingungen mit Datum ablegen.
2. **Nichts erzeugen, was wie ein bekanntes Werk klingt.** Keine Künstler- oder Songnamen im Prompt, keine bekannten Liedtexte als Vorlage. Klingt ein Ergebnis auffällig vertraut, verwirfst du es.
3. **Für Langläufer auf sichere Wege setzen.** Sound-Logo, Kampagnen-Hymne, TV- oder Funkspot: Stock mit klarer Lizenz oder Auftragskomposition mit Rechteübertragung.

Auch die **Plattformregeln** gelten weiter: Für Unternehmensaccounts sind auf Instagram und TikTok oft nur Titel aus der Commercial Music Library freigegeben. Meta, TikTok und YouTube verlangen außerdem Labels für **realistische** KI-Inhalte – bei Instrumentalmusik im Hintergrund meist nicht relevant, bei einer KI-Stimme, die wie eine reale Person klingt, sehr wohl (Kap. 38). Nach dem EU AI Act ist reine KI-Hintergrundmusik in einem Werbeclip in der Regel nicht kennzeichnungspflichtig; die Pflicht zur maschinenlesbaren Markierung nach Art. 50 Abs. 2 trifft die **Anbieter** – SynthID bei Google ist ein Beispiel dafür. Die Details zur Kennzeichnung vertieft Kapitel 39.

!!! warning "Keine Rechtsberatung"
    Dieses Kapitel gibt Orientierung, keine Rechtsberatung. Die Rechtslage zu KI-Musik ist 2026 ausdrücklich im Fluss. Bei Kampagnen mit Reichweite oder Budget klärst du die Musiknutzung mit eurer Rechtsabteilung oder einer Anwältin für Medien- und Urheberrecht.

---

## Zusammenfassung

- Musik für Social Media kommt aus Plattformbibliotheken, Stock, Auftragskomposition oder KI – **Unternehmensaccounts** haben in den Apps oft nur die Commercial Music Library.
- Suno, Udio, ElevenLabs Music und Google Flow Music unterscheiden sich vor allem bei **Lizenz und Tarif**; kommerziell nutzbar ist KI-Musik meist nur im Bezahlplan.
- Gute Musik-Prompts legen **Genre, Stimmung, Tempo, Instrumente, Gesang und Struktur** fest – und nennen keine Künstler- oder Songnamen.
- **Sound-Branding** braucht Konsistenz; KI eignet sich für die Exploration, das finale Sound-Logo gehört wegen fehlender Schutzfähigkeit in menschliche Hand.
- Bei **Podcasts und Audiogrammen** spart KI viel Zeit bei Transkript, Schnitt und Shownotes, ohne rechtliches Neuland.
- Die Urteile des LG München I in **GEMA ./. OpenAI** (11.11.2025) und **GEMA ./. Suno** (31.07.2026) sind **nicht rechtskräftig**, zeigen aber: Dokumentation und Vorsicht sind Pflicht.

---

## Kurzübungen

{{ task(file="tasks/k37_01.yaml") }}

{{ task(file="tasks/k37_02.yaml") }}

{{ task(file="tasks/k37_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k37.yaml") }}
